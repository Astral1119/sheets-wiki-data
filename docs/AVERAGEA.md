---
tags:
  - function
  - generated
  - statistical
---

Returns the numerical average value in a dataset.

### Sample Usage

`AVERAGEA(A2:A100,B2:B100,4,26)`

`AVERAGEA(1,2,3,4,5,C6:C20)`

### Syntax

`AVERAGEA(value1, [value2, ...])`

* `value1` - The first value or range to consider when calculating the average value.
* `value2, ...` - **[** OPTIONAL **]** - Additional values or ranges to consider when calculating the average value.

### Notes

* Although `AVERAGEA` is specified as taking a maximum of 30 arguments, Google Sheets supports an arbitrary number of arguments for this function.
* Any text encountered in the `value` arguments will be set to `0` and included in calculation. To have text values ignored, use `AVERAGE`.
* `AVERAGEA` returns the mean of the combined `value` arguments; that is, the sum of the values in the `value` arguments divided by the number of such values. To calculate the median use `MEDIAN`.

### See Also

[[TRIMMEAN]]: Calculates the mean of a dataset excluding some proportion of data from the high and low ends of the dataset.

[[SMALL]]: Returns the nth smallest element from a data set, where n is user-defined.

[[RANK]]: Returns the rank of a specified value in a dataset.

[[QUARTILE]]: Returns a value nearest to a specified quartile of a dataset.

[[PERCENTRANK]]: Returns the percentage rank (percentile) of a specified value in a dataset.

[[PERCENTILE]]: Returns the value at a given percentile of a dataset.

[[MINA]]: Returns the minimum numeric value in a dataset.

[[MIN]]: Returns the minimum value in a numeric dataset.

[[MEDIAN]]: Returns the median value in a numeric dataset.

[[MAXA]]: Returns the maximum numeric value in a dataset.

[[LARGE]]: Returns the nth largest element from a data set, where n is user-defined.

[[HARMEAN]]: Calculates the harmonic mean of a dataset.

[[GEOMEAN]]: Calculates the geometric mean of a dataset.

[[AVERAGE]]: The AVERAGE function returns the numerical average value in a dataset, ignoring text.

### Examples

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdFdrSlRKWUxodnN2b1VPeGRsZ2stWnc&amp;output=html" width="500"></iframe>