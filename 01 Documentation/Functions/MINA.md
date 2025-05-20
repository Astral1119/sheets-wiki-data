Returns the minimum numeric value in a dataset.

### Sample Usage

`MINA(A2:A100,B2:B100,4,26)`

`MINA(1,2,3,4,5,C6:C20)`

### Syntax

`MINA(value1, [value2, ...])`

* `value1` - The first value or range to consider when calculating the minimum value.
* `value2, ...` - **[** OPTIONAL **]** - Additional values or ranges to consider when calculating the minimum value.

### Notes

* Although `MINA` is specified as taking a maximum of 30 arguments, Google Sheets supports an arbitrary number of arguments for this function.
* Any text value in any of the `value` arguments will be assigned the numeric value `0` for the purpose of this function; ensure that the actual minimum value is either less than 0 or remove text from `data` to calculate the correct answer.

### See Also

[[SMALL]]: Returns the nth smallest element from a data set, where n is user-defined.

[[RANK]]: Returns the rank of a specified value in a dataset.

[[QUARTILE]]: Returns a value nearest to a specified quartile of a dataset.

[[PERCENTRANK]]: Returns the percentage rank (percentile) of a specified value in a dataset.

[[PERCENTILE]]: Returns the value at a given percentile of a dataset.

[[MIN]]: Returns the minimum value in a numeric dataset.

[[MEDIAN]]: Returns the median value in a numeric dataset.

[[MAXA]]: Returns the maximum numeric value in a dataset.

[[MAX]]: Returns the maximum value in a numeric dataset.

[[LARGE]]: Returns the nth largest element from a data set, where n is user-defined.

[[AVERAGEA]]: Returns the numerical average value in a dataset.

[[AVERAGE]]: The AVERAGE function returns the numerical average value in a dataset, ignoring text.

### Examples