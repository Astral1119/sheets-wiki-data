Checks whether a value is an error.

### Sample Usage

`ISERROR(A2)`

`ISERROR(A1/A2)`

`IF(ISERROR(VLOOKUP(B1, A1:A100, 1, FALSE)), "Result not found", VLOOKUP(B1, A1:A100, 1, FALSE))`

### Syntax

`ISERROR(value)`

* `value` - The value to be verified as an error type.

  + `ISERROR` returns `TRUE` if `value` is any error, including `#DIV/0!`, `#N/A`, `#NAME?`,`#NULL!`, `#NUM!`, `#VALUE!`, and `#REF!`.

### Notes

* `ISERROR` returns `TRUE` on any error, unlike [[ISERR]], which returns `TRUE` on all errors except for `#N/A`. Ensure that the correct call is used.
* This function is most often used in conjunction with `IF` in conditional statements.

### See Also

[[ISTEXT]]: Checks whether a value is text.

[[ISREF]]: Checks whether a value is a valid cell reference.

[[ISODD]]: Checks whether the provided value is odd.

[[ISNUMBER]]: Checks whether a value is a number.

[[ISNONTEXT]]: Checks whether a value is non-textual.

[[ISNA]]: Checks whether a value is the error `#N/A`.

[[ISLOGICAL]]: Checks whether a value is `TRUE` or `FALSE`.

[[ISEVEN]]: Checks whether the provided value is even.

[[ISERR]]: Checks whether a value is an error other than `#N/A`.

[[ISBLANK]]: Checks whether the referenced cell is empty.

[[IF]]: Returns one value if a logical expression is `TRUE` and another if it is `FALSE`.

### Examples