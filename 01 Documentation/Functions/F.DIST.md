Calculates the left-tailed F probability distribution (degree of diversity) for two data sets with given input x. Alternately called Fisher-Snedecor distribution or Snedecor's F distribution.

### Sample Usage

`F.DIST(15.35, 7, 6, TRUE)`

`F.DIST(A2, B2, C2, FALSE)`

### Syntax

`F.DIST(x, degrees_freedom1, degrees_freedom2, cumulative)`

* `x` - The input to the F probability distribution function. The value at which to evaluate the function.

  + Must be a positive number.
* `degrees_freedom1` - The numerator degrees of freedom.
* `degrees_freedom2` - The denominator degrees of freedom.
* `cumulative` - Logical value that determines the form of the function. Default value is `FALSE`.

  + If `TRUE`: `F.DIST` returns the cumulative distribution function.
  + If `FALSE`: `F.DIST` returns the probability density function.

### Notes

* Both `degrees_freedom1` and `degrees_freedom2` are truncated to an integer in the calculation if a non-integer is provided as an argument.
* Both `degrees_freedom1` and `degrees_freedom2` must be greater than `1` and may not exceed `10^10`.
* `x`, `degrees_freedom1`, and `degrees_freedom2` must be numeric.

### See Also

[[FDIST]]: Calculates the right-tailed F probability distribution (degree of diversity) for two data sets with given input x. Alternately called Fisher-Snedecor distribution or Snedecor's F distribution.

[[TDIST]]: Calculates the probability for Student's t-distribution with a given input (x).

[[T.INV]]: Calculates the negative inverse of the one-tailed TDIST function.