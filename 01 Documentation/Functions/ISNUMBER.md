Checks whether a value is a number.

### Sample Usage

`ISNUMBER(A2)`

`ISNUMBER(4)`

### Syntax

`ISNUMBER(value)`

* `value` - The value to be verified as a number.

  \*`ISNUMBER` returns `TRUE` if this is a number or a reference to a cell containing a numeric value and `FALSE` otherwise.

### Notes

* This function is most often used in conjunction with `IF` in conditional statements.
* Note that supplying a number enclosed in a string (e.g. `ISNUMBER("123")`) will cause this function to return `FALSE`.

### See Also

[[ISTEXT]]: Checks whether a value is text.

[[ISREF]]: Checks whether a value is a valid cell reference.

[[ISODD]]: Checks whether the provided value is odd.

[[ISNONTEXT]]: Checks whether a value is non-textual.

[[ISNA]]: Checks whether a value is the error `#N/A`.

[[ISLOGICAL]]: Checks whether a value is `TRUE` or `FALSE`.

[[ISEVEN]]: Checks whether the provided value is even.

[[ISERROR]]: Checks whether a value is an error.

[[ISERR]]: Checks whether a value is an error other than `#N/A`.

[[ISBLANK]]: Checks whether the referenced cell is empty.

[[IF]]: Returns one value if a logical expression is `TRUE` and another if it is `FALSE`.

### Examples