Identifies the language used in text within the specified range.

### Sample Usage

`DETECTLANGUAGE(A2:A7)`

`DETECTLANGUAGE("Bonjour")`

`DETECTLANGUAGE(A2)`

### Syntax

`DETECTLANGUAGE(text_or_range)`

* `text_or_range` - The text or reference to cells containing text to evaluate.

  + If `text_or_range` is specified as a range, it must be a one-dimensional column range.

### Notes

* If the range specified contains multiple languages, the first text found will be evaluated.

### See Also

[[GOOGLETRANSLATE]]: Translates text from one language into another.

