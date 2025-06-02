---
tags:
  - function
  - generated
  - text
---

Returns the position at which a string is first found within text counting each double-character as 2.

### Sample Usage

`SEARCHB("新", "农历新年", 2)`

### Syntax

`SEARCHB(search_for, text_to_search, [starting_at])`

* `search_for` - The string to look for within `text_to_search`.
* `text_to_search` - The text to search for the first occurrence of `search_for`.
* `starting_at` - **[** OPTIONAL - `1` by default **]** - The character position within `text_to_search` at which to start the search.

### Notes

* If `search_for` is not found, the `#VALUE!` error value is returned.
* Ensure that `search_for` and `text_to_search` are not supplied in reverse order, or the `#VALUE!` error will likely be returned. The arguments are supplied in a different order than other text functions such as `SPLIT` and `SUBSTITUTE`.
* It's recommended to use a function such as `IFERROR` to check for cases when there aren't matches to the search.
* You can use the wildcard characters: question mark (?) and asterisk (\*), in `search_for`. A question mark matches any single character; an asterisk matches any sequence of characters. If you want to find an actual question mark or asterisk, type a tilde (~) before the character, or see `FINDB`.
* Use `SEARCH` for standard character sets, and `SEARCHB` for double-byte character sets such as Japanese, Chinese (Simplified), Chinese (Traditional), and Korean.

### See Also

[[SEARCH]]: Returns the position at which a string is first found within text, ignoring case.

[[REPLACE]]: Replaces part of a text string with a different text string.

[[REGEXREPLACE]]: Replaces part of a text string with a different text string using regular expressions.

[[REGEXMATCH]]: Whether a piece of text matches a regular expression.

[[SUBSTITUTE]]: Replaces existing text with new text in a string.

[[SPLIT]]: Divides text around a specified character or string, and puts each fragment into a separate cell in the row.

[[FIND]]: Returns the position at which a string is first found within text, case-sensitive.

[[FINDB]]: Returns the position at which a string is first found within text counting each double-character as 2.