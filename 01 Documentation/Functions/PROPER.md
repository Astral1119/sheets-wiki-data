Capitalizes each word in a specified string.

### Sample Usage

`PROPER("united states")`

`PROPER(A2)`

### Syntax

`PROPER(text_to_capitalize)`

* `text_to_capitalize` - The text which will be returned with the first letter of each word in uppercase and all other letters in lowercase.

### Notes

* `PROPER` is useful for proper nouns, such as names of people or geographic locations.
* `PROPER` capitalizes each word in `text_to_capitalize` rather than the beginning of each sentence, and is therefore likely not the correct tool to use for paragraphs or other blocks of text.
* `PROPER` will convert all characters not at the beginning of words to lowercase, which may cause problems with certain strings. For example, using `PROPER("mcLeod")` to capitalize the surname McLeod results in "Mcleod" instead.

### See Also

[[UPPER]]: Converts a specified string to uppercase.

[[SUBSTITUTE]]: Replaces existing text with new text in a string.

[[LOWER]]: Converts a specified string to lowercase.

### Examples