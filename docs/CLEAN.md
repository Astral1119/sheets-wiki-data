---
tags:
  - function
  - generated
  - text
---

Returns the text with the non-printable ASCII characters removed.

### Sample Usage

`CLEAN("AF"&CHAR(31))`

### Syntax

`CLEAN(text)`

* `text` - The text whose non-printable characters are to be removed.

### Notes

* This function only removes non-printable ASCII characters. Non-printable Unicode characters that aren’t found in ASCII are not removed.
* Google Sheets does not show non-printable characters in the UI, so using this function will typically not result in any visible changes.

### See Also

[[CHAR]]: Convert a number into a character according to the current Unicode table.

[[TRIM]]: Removes leading, trailing, and repeated spaces in text.

[[SUBSTITUTE]]: Replaces existing text with new text in a string.