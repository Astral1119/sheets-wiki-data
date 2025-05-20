Returns the first argument if it is not an error value, otherwise returns the second argument if present, or a blank if the second argument is absent.

Examples
--------

[Make a copy](https://docs.google.com/spreadsheets/d/1caTrAGwfvNVVS-ig0ATtUIpIYlJve59o3qorg6cJC3M/copy)

**Note**: Each example is in its own tab.

### Sample Usage

`IFERROR(A1,"Error in cell A1")`

`IFERROR(A2)`

### General usage

Returns a blank if `test` is an error and `value` is null; returns the `value` if `test` is an error and `value` is not null; returns the `test` if it is not an error.

### Unit price

Returns the value "0" when calculating the `unit price` where `Quantity` is null.

### Student grades

Returns the specified error message when searching the student `Grade` where `Student ID` does not exist.

### Syntax

`IFERROR(value, [value_if_error])`

* `value` - The value to return if `value` itself is not an error.
* `value_if_error` - **[** OPTIONAL - blank by default **]** - The value the function returns if `value` is an error.

### Notes

* `IFERROR(exp1,exp2)` is logically equivalent to `IF(NOT(ISERROR(exp1)),exp1,exp2)`. Ensure that this is the desired behavior.

### See Also

[[ISNA]]: Checks whether a value is the error `#N/A`.

[[ISERROR]]: Checks whether a value is an error.

[[ISERR]]: Checks whether a value is an error other than `#N/A`.

[[IF]]: Returns one value if a logical expression is `TRUE` and another if it is `FALSE`.