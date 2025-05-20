Returns the column number of a specified cell, with `A=1`.

### Sample Usage

`COLUMN(A9)`

### Syntax

`COLUMN([cell_reference])`

* `cell_reference` - **[** OPTIONAL - By default, the cell containing the formula **]** - The cell whose column number will be returned. Column `A` corresponds to `1`.

  + if `cell_reference` is a range more than one cell wide and the formula is not used as an array formula, the position of the first column in `cell_reference` is returned.

### See Also

[[ROWS]]: Returns the number of rows in a specified array or range.

[[ROW]]: Returns the row number of a specified cell.

[[COLUMNS]]: Returns the number of columns in a specified array or range.
