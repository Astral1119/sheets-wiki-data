---
tags:
  - general
  - terminology
---

Google Sheets has two calculation limits for each formula:

1.  Function calls
2. Recursion calls

These limits are separate. If either one is reached, the formula will stop calculating and output `#ERROR!`.

### Function Calls

The function call limit is approximately `2,000,000` (`2e6`) function calls per cell. The exact value is currently unknown as there is variance in the results of the functions used to reach that limit.

### Stack Limit

The stack limit is `10,000` (`1e4`) function calls. This limit is the same when used in [[LAMBDA Recursion]] and [[iterative calculation]].
[Church-encoded lists](https://en.wikipedia.org/wiki/Church_encoding#Church_lists_%E2%80%93_right_fold_representation) implemented in Google Sheets (see: [[LIST]]) appear to violate this property, potentially a result of how [closures](https://en.wikipedia.org/wiki/Closure_(computer_programming)) are handled.

### Further Reading

- [Calculation Limits](https://docs.google.com/spreadsheets/d/160UfdYEOoplAaKzm4Cx4rF0NNWwd6b2KC3LH3xAr-jk/edit#gid=0)
	- This spreadsheet contains a number of formulae at each calculation limit to demonstrate this phenomenon.
