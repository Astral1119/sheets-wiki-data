Returns the number of rows in a specified array or range.

ROWS for BigQuery

Returns the number of rows in a data column.

### Sample Usage

`ROWS(table_name!fruits)`

Syntax
------

`ROWS(column)`

* `column` - The data column whose row count will be returned.

**Tip:** Null values are counted as well.

### Sample Usage

`ROWS(A9:A62)`

`ROWS({1;2;3;4;5})`

### Syntax

`ROWS(range)`

* `range` - The range whose row count will be returned

### See Also

[[ROW]]: Returns the row number of a specified cell.

[[COLUMNS]]: Returns the number of columns in a specified array or range.

[[COLUMN]]: Returns the column number of a specified cell, with `A=1`.

### Examples

Returns the number of rows in a reference or array.