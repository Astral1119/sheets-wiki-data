Returns the "value not available" error, `#N/A`.

### Sample Usage

`NA()`

### Syntax

`NA()`

### Notes

* `#N/A` is an error, so both the [[ISNA]] and [[ISERROR]] functions will return `TRUE`. Use [[ISERR]] to find errors which are not `#N/A`.
* Typing `=NA()` into a cell is equivalent to directly entering the error value `#N/A`.
* `#N/A` is used to mark missing information and to indicate to functions operating on ranges or cells containing such values to halt calculation. For instance, if cell `B2` contained the result of an `IF` statement: `=IF(ISBLANK(A1),0,A1)` and `B2` was subsequently involved in a sum or other formula, that formula would assume that `B2` held the correct information. By altering the formula in `B2` to `=IF(ISBLANK(A1),NA(),A1)`, any subsequent operation on `B2` would halt upon encountering the `#N/A` error, and return that error.
* `#N/A` errors indicate missing information and signal functions to cease calculation. Use the `#N/A` value instead of `0` or the cell's results. For example, if `A1` contains the value `#N/A` or `=NA()`, the formula `=A1+A2` will evaluate to `#N/A`.

### See Also

[[ISNA]]: Checks whether a value is the error `#N/A`.

[[ISERROR]]: Checks whether a value is an error.

[[ISERR]]: Checks whether a value is an error other than `#N/A`.

### Examples

Checks the validity of the data before further computing, in order to avoid mis-calculation.