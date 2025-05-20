Returns a value nearest to a specified quartile of a dataset.

### Sample Usage

`QUARTILE(A2:A100,3)`

`QUARTILE(A2:A100,B2)`

### Syntax

`QUARTILE(data, quartile_number)`

* `data` - The array or range containing the dataset to consider.
* `quartile_number` - Which quartile value to return.

  + `0` returns the minimum value in `data` (0% mark).
  + `1` returns the value in `data` closest to the first quartile (25% mark).
  + `2` returns the value in `data` closest to the median (50% mark).
  + `3` returns the value in `data` closest to the third quartile (75% mark).
  + `4` returns the maximum value in `data` (100% mark).

### See Also

[[SMALL]]: Returns the nth smallest element from a data set, where n is user-defined.

[[RANK]]: Returns the rank of a specified value in a dataset.

[[PERCENTRANK]]: Returns the percentage rank (percentile) of a specified value in a dataset.

[[PERCENTILE]]: Returns the value at a given percentile of a dataset.

[[MINA]]: Returns the minimum numeric value in a dataset.

[[MIN]]: Returns the minimum value in a numeric dataset.

[[MEDIAN]]: Returns the median value in a numeric dataset.

[[MAXA]]: Returns the maximum numeric value in a dataset.

[[MAX]]: Returns the maximum value in a numeric dataset.

[[LARGE]]: Returns the nth largest element from a data set, where n is user-defined.

[[AVERAGEA]]: Returns the numerical average value in a dataset.

[[AVERAGE]]: The AVERAGE function returns the numerical average value in a dataset, ignoring text.

### Examples