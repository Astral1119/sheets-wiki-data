---
tags:
  - function
  - generated
  - statistical
---

Returns the rank of a specified value in a dataset. If there is more than one entry of the same value in the dataset, the top rank of the entries will be returned.

### Sample Usage

`RANK.EQ(A10, A1:A100, TRUE)`

`RANK.EQ(B32, B8:B47, FALSE)`

`RANK.EQ(A10, A1:A100)`

### Syntax

`RANK.EQ(value, data, [is_ascending])`

* `value` - The value whose rank will be determined.
* `data` - The array or range containing the dataset to consider.
* `is_ascending` - **[** OPTIONAL - default is descending (`FALSE`) **]** - Whether to consider the values in data in descending or ascending order.

### See Also

[[RANK]]: Returns the rank of a specified value in a dataset.

[[RANK.AVG]]: Returns the rank of a specified value in a dataset. If there is more than one entry of the same value in the dataset, the average rank of the entries will be returned.