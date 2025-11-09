---
tags:
  - theory
  - terminology
---

> [!WARNING]
> This article uses [[unofficial terminology]].

A **dependency** is a directed relationship between two [[term|terms]] in a spreadsheet, where one term's value depends on another's.  
Dependencies form the underlying structure that determines evaluation order and recalculation behavior in Google Sheets.

### Overview

Every formula defines one or more *dependencies* through cell references, named ranges, or function calls.  
For example:

```gse
=A1 + B1
```

In this formula, the cell depends on the values of `A1` and `B1`.  
If either `A1` or `B1` changes, the formula will automatically recalculate.

### Circular Dependencies

A **circular dependency** arises when a term depends—directly or indirectly—on itself.  
For example:

```gse
=A1 + B1  
=B1 + A1
```

Google Sheets detects such cycles and raises a [[#REF!]] error.  
Iterative calculation can sometimes be enabled to handle controlled cycles, though this is rarely used for ordinary modeling.

### Dependency Propagation

When an input changes, Sheets performs **dependency propagation**: it traverses the dependency graph from the modified node and recalculates all affected formulas.  
This mechanism ensures consistency while minimizing redundant computation.

Certain operations, such as array expansion or [[LAMBDA recursion]], can multiply dependency relationships—making recalculation slower or more complex.

### Volatile Dependencies

Some functions introduce *volatile* dependencies.  
Volatile functions (e.g. `RAND()`, `NOW()`, `RANDBETWEEN()`) cause dependent formulas to recalculate even if their inputs have not changed.  
These can introduce performance overhead in large models.

### See Also
- [[Calculation limits]] — boundaries on recursion, dependency depth, and evaluation time.  
- [[Circular dependency]] — errors resulting from cyclic references.  
- [[Evaluation order]] — how Sheets resolves dependencies during recalculation.
