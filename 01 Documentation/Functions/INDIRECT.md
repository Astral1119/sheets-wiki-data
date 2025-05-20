Returns a cell reference specified by a string.

Examples
--------

[Make a copy](https://docs.google.com/spreadsheets/d/1cbh9wUeE0UtIMPSEv51GE7qYix-qwOm_er0wW4LhuK0/copy)

**Note**: Each example is in its own tab.

### Sample Usage

`INDIRECT("Sheet2!"&B10)`

`INDIRECT("A2")`

`INDIRECT("R2C3", FALSE)`

### Student info

Student Info data as a separate sheet in the spreadsheet.

### Student grades

Returns the contents of the reference which can be a cell or an area.

### Syntax

`INDIRECT(cell_reference_as_string, [is_A1_notation])`

* `cell_reference_as_string` - A cell reference, written as a string with surrounding quotation marks.
* `is_A1_notation` - **[**OPTIONAL - `TRUE` by default**]** - Indicates if the cell reference is in A1 notation or R1C1 notation.

**Tip**: You can't use table references in =INDIRECT yet. Try [[IMPORTRANGE]] instead.