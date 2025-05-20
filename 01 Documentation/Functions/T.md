Returns string arguments as text.

### Sample Usage

`T(A2)`

`T("cat")`

### Syntax

`T(value)`

* `value` - The argument to be converted to text.

  + If `value` is text, `T` returns `value`.
  + If `value` is a reference to a cell containing text, `T` returns the contents of `value`.
  + If `value` is an error or a cell containing an error, `T` returns the error.
  + Otherwise, `T` returns an empty string.

### Notes

* This function is rarely necessary as Google Sheets automatically converts between most formats appropriately. It is provided primarily for compatibility with formulas used in other spreadsheet packages.

### See Also

[[N]]: Returns the argument provided as a number.

### Examples