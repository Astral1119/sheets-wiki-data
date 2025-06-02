---
tags:
  - theory
  - terminology
---

> [!WARNING]
> This article uses [[Unofficial terminology]].

A [term](https://en.wikipedia.org/wiki/Language_construct) is a syntactic element of a formula. Each term has a [[data type]] that defines what operations can be performed on it.

### Lambda terms
*Main article: [[Lambda terms]]*

Lambda terms are [first-class](https://en.wikipedia.org/wiki/First-class_function). They can be passed as arguments to other functions, returned from other functions, and be assigned to variables. They are comprised of [[literal||literals]] and [[LAMBDA]] functions.

### Primitive functions

Primitive functions are not first-class and comprise every default function. The only operation that can be performed on primitive functions is [application](https://en.wikipedia.org/wiki/Function_application) (e.g. applying it to lambda terms, such as `SUM(1, 2, 3)`).