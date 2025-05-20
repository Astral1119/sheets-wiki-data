Returns the number of numeric values in a dataset.

### Syntax

`COUNT(column)`

* `column`: The data column to consider when counting.

**Tip:**

* COUNT for BigQuery counts both numeric and non-numeric values.
* Counting multiple columns is not supported

[Learn more about numeric columns in BigQuery](https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types#numeric_types)

### Sample Usage

`COUNT(A2:A100,B2:B100,4,26)`

`COUNT(1,2,3,4,5,C6:C20)`

### Syntax

`COUNT(value1, [value2, ...])`

* `value1` - The first value or range to consider when counting.
* `value2, ...` - **[** OPTIONAL **]** - Additional values or ranges to consider when counting.

### Notes

* Although `COUNT` is specified as taking a maximum of 30 arguments, Google Sheets supports an arbitrary number of arguments for this function.
* `COUNT` counts all numeric values in a dataset, including those which appear more than once. To count unique values, use `COUNTUNIQUE`.
* `COUNT` counts *only* numeric values; text values are ignored.

### See Also

[[MODE]]: Returns the most commonly occurring value in a dataset.

[[DCOUNTA]]: Counts values, including text, selected from a database table-like array or range using a SQL-like query.

[[DCOUNT]]: Counts numeric values selected from a database table-like array or range using a SQL-like query.

[[COUNTUNIQUE]]: Counts the number of unique values in a list of specified values and ranges.

[[COUNTIF]]: Returns a conditional count across a range.

[[COUNTBLANK]]: Returns the number of empty cells in a given range.

[[COUNTA]]:

Returns the number of values in a dataset.