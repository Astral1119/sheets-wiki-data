---
tags:
  - function
  - generated
  - array
---

Transposes the rows and columns of an array or range of cells.

### Sample Usage

`TRANSPOSE({1,2;3,4;5,6})`

`TRANSPOSE(A2:F9)`

### Syntax

`TRANSPOSE(array_or_range)`

* `array_or_range` - The array or range whose rows and columns will be swapped.

### Notes

* Transposition operates such that the value in the nth row and mth column will become the value in the mth row and nth column. E.g. the value in the fourth row and second column will be put into the second row and fourth column. The result of a transposition on a range of size m rows by n columns is therefore n rows by m columns.

### Examples

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdDdtbXpRYWxGUXVudWpORjdoSzNrZEE&amp;output=html" width="500"></iframe>