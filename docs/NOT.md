---
tags:
  - function
  - generated
  - logical
---

Returns the opposite of a logical value - `NOT(TRUE)` returns `FALSE`; `NOT(FALSE)` returns `TRUE`.

### Sample Usage

`NOT(A2)`

`NOT(ISERR(A2))`

### Syntax

`NOT(logical_expression)`

* `logical_expression` - An expression or reference to a cell holding an expression that represents some logical value, i.e. `TRUE` or `FALSE`.

### Notes

* Because `0` has a logical value of `FALSE` and any non-zero numeric value has a logical value of `TRUE`, `NOT(0)` returns `TRUE` and `NOT(6)` returns `FALSE`. However, when non-numeric values are input into `NOT`, the function returns the error `#VALUE!`.

### See Also

[[FALSE]]: Returns the logical value `FALSE`.

[[TRUE]]: Returns the logical value `TRUE`.

### Examples

Reverses the logical value.

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdF9QTjRYWWgxSnJwTXJsTWVod092VXc&amp;single=true&amp;gid=0&amp;output=html&amp;widget=true" width="500"></iframe>