---
tags:
  - datatype
---

> [!WARNING]
> This article uses [[Unofficial terminology]].

Each [[term]] in Google Sheets has a [type](https://en.wikipedia.org/wiki/Type_system) that determines which operations can be performed on it.

### Overview

Google Sheets uses a [dynamic](https://developer.mozilla.org/en-US/docs/Glossary/Dynamic_typing), [weakly](https://en.wikipedia.org/wiki/Type_safety) typed system. Types are not declared by the user; they are inferred at runtime from cell content and context. This allows flexible formulas but can produce inconsistent behavior, as type coercion is handled differently across functions.

Sheets recognizes the following core types:

| Type        | Description                                                                         |
| ----------- | ----------------------------------------------------------------------------------- |
| [[Number]]  | Numeric values such as integers, decimals, and scientific notation.                 |
| [[String]]  | Text values enclosed in quotes or inferred from literal input.                      |
| [[Boolean]] | Logical values `TRUE` and `FALSE`.                                                  |
| [[Null]]    | Empty cells or expressions that return no value.                                    |
| [[Array]]   | Two-dimensional collections of values that may spill across multiple cells.         |
| [[Lambda]]  | Executable terms created using `LAMBDA` or related constructs.                      |
| [[Error]]   | Runtime signals representing failed evaluation. Propagate through most expressions. |
| [[Null value|Null]] | A special value denoting the lack of a type. |

Higher-level constructs such as [[LAMBDA UDT|LAMBDA UDTs]] and [[Data structures]] are derived from these base types.

### Dynamic typing

A term’s type may change depending on how it is used. For example:

```gse
="1"&1       → "11"
=IF("","X","Y") → "Y"
```

Such conversions are governed by [[Type coercion]].

### Scalar types

These are single-cell values that represent indivisible data within a formula. Scalar types form the basic units of computation in Sheets and contrast with compound structures such as arrays or lambdas. They include [[Number]] , [[String]], [[Boolean]], [[Null]], and [[Error]].

Scalar types participate directly in type coercion and function arguments, and they do not produce spill ranges or encapsulate multiple values.

### Structural types

Some expressions encapsulate multiple values or behaviors:
- [[Array]] terms hold multiple values in two dimensions.
- [[Lambda]] terms hold executable expressions.
- [[LAMBDA UDT|LAMBDA UDTs]] simulate user-defined structures.

These may be considered compound types, though Sheets does not support type introspection.

### Type errors

If a value cannot be coerced into the expected type, evaluation produces an error such as #VALUE! or #N/A.

### See Also
- [[Type coercion]] — conversion rules between types.
- [[Number]], [[String]], [[Boolean]], [[Null]], [[Array]], [[Lambda]] — type-specific behavior.
- [[LAMBDA data structures]] — compound types built from LAMBDA.

