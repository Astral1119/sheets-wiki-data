Calculates the negative inverse of the one-tailed TDIST function.

### Sample Usage

`T.INV(0.35, 1)`

`T.INV(A1, A2)`

### Syntax

`T.INV(probability, degrees_freedom)`

* `probability` - The probability associated with the t-distribution.

  + Must be greater than `0` and less than `1`.
* `degrees_freedom` - The number of degrees of freedom.

  + Truncated to an integer in the calculation if a non-integer is provided as an argument.
  + Must be greater than or equal to `1`.

### Notes

* `T.INV` is to be used for the negative inverse of the one-tailed  `TDIST` function.
* Both arguments to `T.INV` must be numeric or a destination cell whose value is numeric.

### See Also

[[TDIST]]: Calculates the probability for Student's t-distribution with a given input (x).

[[TINV]]: Calculates the inverse of the two-tailed TDIST function.

### Examples

In this example, `T.INV` uses a `probability` value of `0.05757` and `degrees_freedom` of `45` to compute the result.