---
tags:
  - theory
  - terminology
---

> [!WARNING]
> This article uses [[Unofficial terminology]].

A [term](https://en.wikipedia.org/wiki/Language_construct) is a syntactic element of a formula. Each term has a [[data type]] that defines what operations can be performed on it.

### Terms and Values

In evaluation, a **term** represents *syntax*, while a **value** represents *result*.  
A formula such as:

```gse
=SUM(1, 2)
```

contains the term `SUM(1, 2)`, which evaluates to the value 3. Note that the term `SUM(1, 2)` is recursively defined, containing the primitive `SUM` and the [[number]] literals `1` and `2`.
All values originate from terms, but not all terms reduce to values. For instance, terms that produce [[Crash bug|crash bugs]] do not reduce to values. Note however that [[Error|errors]] are still values.

### Lambda term
*Main article: [[Lambda term]]

Lambda terms are [first-class](https://en.wikipedia.org/wiki/First-class_function). They can be passed as arguments to other functions, returned from other functions, and be assigned to variables. They are comprised of [[literal||literals]] and [[LAMBDA]] functions.

### Primitive function

Primitive functions are not first-class and comprise every default function. The only operation that can be performed on primitive functions is [application](https://en.wikipedia.org/wiki/Function_application) (e.g. applying them to lambda terms, such as `SUM(1, 2, 3)`).
