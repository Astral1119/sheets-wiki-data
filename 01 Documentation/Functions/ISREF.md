Checks whether a value is a valid cell reference.

### Sample Usage

`ISREF(A2)`

### Syntax

`ISREF(value)`

* `value` - The value to be verified as a cell reference.

  \*`ISREF` returns `TRUE` if this is a valid cell reference, and `FALSE` otherwise.

  + Providing a string containing a valid cell reference (e.g. "A2") for `value` returns `FALSE` as the input is a string, not a reference.

### Notes

* This function is most often used in conjunction with `IF` in conditional statements.

### See Also

[[ISTEXT]]: Checks whether a value is text.

[[ISODD]]: Checks whether the provided value is odd.

[[ISNUMBER]]: Checks whether a value is a number.

[[ISNONTEXT]]: Checks whether a value is non-textual.

[[ISNA]]: Checks whether a value is the error `#N/A`.

[[ISLOGICAL]]: Checks whether a value is `TRUE` or `FALSE`.

[[ISEVEN]]: Checks whether the provided value is even.

[[ISERROR]]: Checks whether a value is an error.

[[ISERR]]: Checks whether a value is an error other than `#N/A`.

[[ISBLANK]]: Checks whether the referenced cell is empty.

[[IF]]: Returns one value if a logical expression is `TRUE` and another if it is `FALSE`.

### Examples