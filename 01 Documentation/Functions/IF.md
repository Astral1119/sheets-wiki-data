Returns one value if a logical expression is `TRUE` and another if it is `FALSE`.

### Sample Usage

`IF(A2 = "foo","A2 is foo")`

`IF(A2,"A2 was true","A2 was false")`

`IF(TRUE,4,5)`

### Syntax

`IF(logical_expression, value_if_true, value_if_false)`

* `logical_expression` - An expression or reference to a cell containing an expression that represents some logical value, i.e. `TRUE` or `FALSE`.
* `value_if_true` - The value the function returns if `logical_expression` is `TRUE`.
* `value_if_false` - **[** OPTIONAL - blank by default **]** - The value the function returns if `logical_expression` is `FALSE`.

### Notes

* Ensure that `value_if_true` and `value_if_false` are provided to the function in the correct order - this is the single most common source of problems with `IF`.

### See Also

* [[IFERROR]]: Returns the first argument if it is not an error value, otherwise returns the second argument if present, or a blank if the second argument is absent.
* [[IFS]]: Evaluates multiple conditions and returns a value that corresponds to the first true condition.

### Examples

Specifies a logical test to be performed.

[Make a copy](https://docs.google.com/spreadsheets/d/1ct3jW2PPGdUErLQWFFZ3Pk1X521M_z6Rm8qeMonR_iE/copy)