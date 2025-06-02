---
tags:
  - function
  - generated
  - statistical
---

Calculates the inverse of the right-tailed chi-squared distribution.

### Sample Usage

`CHISQ.INV.RT(0.42, 2)`

`CHISQ.INV.RT(A2, B2)`

### Syntax

`CHISQ.INV.RT(probability, degrees_freedom)`

* `probability` - The probability associated with the right-tailed chi-squared distribution.

  + Must be greater than `0` and less than `1`.
* `degrees_freedom` - The number of degrees of freedom of the distribution.

### Notes

* `degrees_freedom` is truncated to an integer if a non-integer is provided.
* `degrees_freedom` must be at least `1`.
* All arguments must be numeric.
* `CHISQ.INV.RT` is synonymous with `CHIINV`.

### See Also

[[CHIDIST]]: Calculates the right-tailed chi-squared distribution, often used in hypothesis testing.

[[CHIINV]]: Calculates the inverse of the right-tailed chi-squared distribution.

[[CHISQ.INV]]: Calculates the inverse of the left-tailed chi-squared distribution.

[[CHITEST]]: Returns the probability associated with a Pearson’s chi-squared test on the two ranges of data. Determines the likelihood that the observed categorical data is drawn from an expected distribution.

[[F.INV]]: Calculates the inverse of the left-tailed F probability distribution. Also called the Fisher-Snedecor distribution or Snedecor’s F distribution.

[[T.INV]]: Calculates the negative inverse of the one-tailed TDIST function.

### Example

Suppose you want to find the cutoff for the chi-squared statistic associated with a p-value of `0.05`. With `4` degrees of freedom, you can consider any chi-squared statistic larger than `3.36` to be statistically significant.

| 1 | Probability | Degrees freedom | Solution |
| --- | --- | --- | --- |
| **2** | 0.05 | 4 | 9.487729037 |
| **3** | 0.05 | 4 | =CHISQ.INV.RT(0.05, 4) |
| **4** | 0.05 | 4 | =CHISQ.INV.RT(A2, B2) |