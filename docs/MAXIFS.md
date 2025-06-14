---
tags:
  - function
  - generated
  - statistical
---

Returns the maximum value in a range of cells, filtered by a set of criteria.

MAXIFS for BigQuery

Returns the maximum value in a filtered data column, filtered by a set of criteria applied to additional data columns.

### Sample Usage

`MAXIFS(table_name!price, table_name!fruits,”Apple”, table_name!inventory, “<30”)`

Syntax
------

`MAXIFS(column, criteria_column1, criterion1, criteria_column2, criterion2)`

* `column`: The data column from which the maximum will be determined.
* `criteria_column1`: The data column over which to evaluate `criterion1`.
* `criterion1`: The pattern or test to apply to `criteria\_column1`, such that each cell that evaluates to `TRUE` will be included in the filtered set.
* `creteria_column2`: Additional data columns over which to evaluate the additional criteria. The filtered set will be the intersection of the sets produced by each criterion-column pair.
* `criterion2`: The pattern or test to apply to `criteria\_column2`.

Sample Usage
------------

`MAXIFS(A1:A3, B1:B3, 1, C1:C3, “A”)`

`MAXIFS(D4:E5, F4:G5, “>5”, F6:G7, “<10”)`

Syntax
------

`MAXIFS(range, criteria_range1, criterion1, [criteria_range2, criterion2, …])`

* `range` - The range of cells from which the maximum will be determined.
* `criteria_range1` - The range of cells over which to evaluate `criterion1`.
* `criterion1` - The pattern or test to apply to `criteria_range1`.
* `criteria_range2, criterion2, …` **Optional:** Additional ranges and their associated criteria. Note that filtering will result in the intersection of these.

Notes
-----

* `MAXIFS` will return `0` if none of the criterion are satisfied.
* `range` and all of the criterion ranges must be the same size. If they aren't, `MAXIFS` will return a `#VALUE` error.

See Also
--------

[[MINIFS]]:

Returns the minimum value in a range of cells, filtered by a set of criteria.

[[SUMIFS]]: Returns the sum of a range depending on multiple criteria.

[[IFS]]:

Evaluates multiple conditions and returns a value that corresponds to the first true condition.

Example
-------

|  | A | B | C |
| --- | --- | --- | --- |
| 1 | **ID** | **Score** | **Section** |
| 2 | 123 | 30 | B |
| 3 | 102 | 28 | A |
| 4 | 157 | 29 | A |
| 5 | 189 | 19 | B |
| 6 |  |  |  |
| 7 | **Solution** | **Formula** | |
| 8 | 157 | = MAXIFS(A2:A5, B2:B5, ">25", C2:C5, “A”) | |
| 9 | 123 | = MAXIFS(A2:A5, B2:B5, ">25", C2:C5, “B”) | |
| 10 | 189 | = MAXIFS(A2:A5, B2:B5, "<35", C2:C5, “B”) | |
| 11 | 0 | = MAXIFS(A2:A5, B2:B5, ">35", C2:C5, “B”) | |