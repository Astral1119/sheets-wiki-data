---
tags:
  - function
  - generated
  - text
---

Returns a substring from the beginning of a specified string.

### Sample Usage

`LEFT(A2,2)`

`LEFT("lorem ipsum")`

### Syntax

`LEFT(string, [number_of_characters])`

* `string` - The string from which the left portion will be returned.
* `number_of_characters` - **[** OPTIONAL - `1` by default **]** - The number of characters to return from the left side of `string`.

### Notes

* `0` is a valid input for `number_of_characters` and will cause `LEFT` to return the empty string.

### See Also

[[SUBSTITUTE]]: Replaces existing text with new text in a string.

[[SPLIT]]: Divides text around a specified character or string, and puts each fragment into a separate cell in the row.

[[RIGHT]]: Returns a substring from the end of a specified string.

[[MID]]: Returns a segment of a string.

### Examples

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdEFMVHdjWkZzQVNDcXM0LTM5WWVLREE&amp;output=html" width="500"></iframe>