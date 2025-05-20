Appends strings to one another.

### Sample Usage

`CONCATENATE("Welcome", " ", "to", " ", "Sheets!")`

`CONCATENATE(A1,A2,A3)`

`CONCATENATE(A2:B7)`

### Syntax

`CONCATENATE(string1, [string2, ...])`

* `string1` - The initial string.
* `string2 ...` - **[** OPTIONAL **]** - Additional strings to append in sequence.

### Notes

* When a range with both width and height greater than 1 is specified, cell values are appended across rows rather than down columns. That is, `CONCATENATE(A2:B7)` is equivalent to `CONCATENATE(A2,B2,A3,B3, ... , A7,B7)`.

### See Also

[[SPLIT]]: Divides text around a specified character or string, and puts each fragment into a separate cell in the row.

[[JOIN]]: Concatenates the elements of one or more one-dimensional arrays using a specified delimiter.
