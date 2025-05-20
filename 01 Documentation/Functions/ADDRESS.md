Returns a cell reference as a string.

### Sample Usage

`ADDRESS(1,2)`

`ADDRESS(1,2,4,FALSE)`

`ADDRESS(1,2,,,"Sheet2")`

### Syntax

`ADDRESS(row, column, [absolute_relative_mode], [use_a1_notation], [sheet])`

* `row` - The row number of the cell reference
* `column` - The column number (not name) of the cell reference. `A` is column number `1`.
* `absolute_relative_mode` - **[** OPTIONAL - `1` by default **]** - An indicator of whether the reference is row/column absolute. `1` is row and column absolute (e.g. $A$1), `2` is row absolute and column relative (e.g. A$1), `3` is row relative and column absolute (e.g. $A1), and `4` is row and column relative (e.g. A1).
* `use_a1_notation` - **[** OPTIONAL - `TRUE` by default **]** - A boolean indicating whether to use `A1` style notation (TRUE) or `R1C1` style notation (FALSE).
* `sheet` - **[** OPTIONAL - absent by default **]** - A string indicating the name of the sheet into which the address points.

### Notes

* When using optional parameters such as `sheet`, ensure that commas are inserted to indicate which parameter is being set.

### See Also

[[OFFSET]]: Returns a range reference shifted a specified number of rows and columns from a starting cell reference.

[[MATCH]]: Returns the relative position of an item in a range that matches a specified value.

[[01 Documentation/Functions/INDEX|INDEX]]: Returns the content of a cell, specified by row and column offset.
