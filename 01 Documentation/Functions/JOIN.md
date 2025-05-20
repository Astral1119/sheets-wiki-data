Concatenates the elements of one or more one-dimensional arrays using a specified delimiter.

### Sample Usage

`JOIN(" and-a ",{1,2,"1 2 3 4"})`

`JOIN(",",{1,2,3},{4;5;6})`

`JOIN("-",A1:A100)`

### Syntax

`JOIN(delimiter, value_or_array1, [value_or_array2, ...])`

* `delimiter` - The character or string to place between each concatenated value.

  + `delimiter` may be specified as blank, e.g. `JOIN(,{1,2,3})`.
* `value_or_array1` - The value or values to be appended using `delimiter`.
* `value_or_array2, ...` - **[** OPTIONAL **]** - Additional value or array to be appended using `delimiter`.

### Notes

* When `delimiter` is omitted, the result of `JOIN` is similar to that of `CONCATENATE`.

### See Also

[[SPLIT]]: Divides text around a specified character or string, and puts each fragment into a separate cell in the row.

[[CONCATENATE]]: Appends strings to one another.

### Examples