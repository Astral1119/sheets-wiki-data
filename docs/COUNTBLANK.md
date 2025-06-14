---
tags:
  - function
  - generated
  - math
---

Returns the number of empty cells in a given range.

COUNTBLANK for BigQuery

Returns the number of empty values in a data column.

### Sample Usage

`COUNTBLANK(table_name!fruits)`

### Syntax

`COUNTBLANK(column)`

* `column`: The data column in which to count the number of nulls.

**Tip:** Counting blanks in multiple columns is not supported.

### Sample Usage

`COUNTBLANK(A2:C100)`

### Syntax

`COUNTBLANK(value1, [value2,...])`

* value1 - The first value or range in which to count the number of blanks.
* value2 - [OPTIONAL ] - Additional values or ranges in which to count the number of blanks.

### Notes

* `COUNTBLANK` considers cells with no content and cells containing an empty string (`""`) to be blank cells.

### See Also

[[DCOUNTA]]: Counts values, including text, selected from a database table-like array or range using a SQL-like query.

[[DCOUNT]]: Counts numeric values selected from a database table-like array or range using a SQL-like query.

[[COUNTUNIQUE]]: Counts the number of unique values in a list of specified values and ranges.

[[COUNTIF]]: Returns a conditional count across a range.

[[COUNTA]]: Returns the number of values in a dataset.

[[COUNT]]: Returns the number of numeric values in a dataset.

### Examples

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdGx0cE1lQVRwNXhEb1pIT1EyeE8wWWc&amp;output=html" width="500"></iframe>