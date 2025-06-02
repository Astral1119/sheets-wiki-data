---
tags:
  - function
  - generated
  - lookup
---

Returns an element from a list of choices based on index.

### Sample Usage

`CHOOSE(2,"A","B","C")`

### Syntax

`CHOOSE(index, choice1, [choice2, ...])`

* `index` - Which choice (of the up to 29 provided) to return.

  + If `index` is zero, negative, or greater than the number of choices provided, the `#NUM!` error is returned.
* `choice1` - A potential value to return. Required. May be a reference to a cell or an individual value.
* `choice2, ...` - Additional values among which to choose.

### See Also

[[OFFSET]]: Returns a range reference shifted a specified number of rows and columns from a starting cell reference.

### Examples

Uses an `index` to return a value from the specified list of up to 30 values.

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdHJkb3NhRDF5MWhyNGQyemdwZ2YwM1E&amp;single=true&amp;gid=0&amp;output=html&amp;widget=true" width="500"></iframe>