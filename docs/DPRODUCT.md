---
tags:
  - function
  - generated
  - database
---

Returns the product of values selected from a database table-like array or range using a SQL-like query.

### Sample Usage

`DPRODUCT(A2:F20,G2,A22:D23)`

`DPRODUCT(A2:F20,"price",{"Ticker";"Google"})`

### Syntax

`DPRODUCT(database, field, criteria)`

* `database` - The array or range containing the data to consider, structured in such a way that the first row contains the labels for each column's values.
* `field` - Indicates which column in `database` contains the values to be extracted and operated on.

  + `field` may either be a text label corresponding to a column header in the first row of `database` or a numeric index indicating which column to consider, where the first column has the value `1`.
* `criteria` - An array or range containing zero or more criteria to filter the `database` values by before operating.

### Notes

* Detailed information about database functions and constructing queries around criteria can be found in the [Database Functions help article](https://support.google.com/docs/answer/173497).

### See Also

[[PRODUCT]]: Returns the result of multiplying a series of numbers together.

[[DVARP]]: Returns the variance of an entire population selected from a database table-like array or range using a SQL-like query.

[[DVAR]]: Returns the variance of a population sample selected from a database table-like array or range using a SQL-like query.

[[DSUM]]: Returns the sum of values selected from a database table-like array or range using a SQL-like query.

[[DSTDEVP]]: Returns the standard deviation of an entire population selected from a database table-like array or range using a SQL-like query.

[[DSTDEV]]: Returns the standard deviation of a population sample selected from a database table-like array or range using a SQL-like query.

[[DMIN]]: Returns the minimum value selected from a database table-like array or range using a SQL-like query.

[[DMAX]]: Returns the maximum value selected from a database table-like array or range using a SQL-like query.

[[DGET]]: Returns a single value from a database table-like array or range using a SQL-like query.

[[DCOUNTA]]: Counts values, including text, selected from a database table-like array or range using a SQL-like query.

[[DCOUNT]]: Counts numeric values selected from a database table-like array or range using a SQL-like query.

[[DAVERAGE]]: Returns the average of a set of values selected from a database table-like array or range using a SQL-like query.

### Examples

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdFpqbUNCcnVxUHZlOTFzTHQ3bmgwQ0E&amp;output=html" width="500"></iframe>