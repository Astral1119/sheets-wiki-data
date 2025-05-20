Converts a provided date/time, percentage, currency or other formatted numeric value to a pure number without formatting.
### Syntax

`TO_PURE_NUMBER(value)`

* `value` - The argument or reference to a cell to be converted to a pure number.

  + If `value` is a number or a reference to a cell containing a numeric value, `TO_PURE_NUMBER` returns `value` with all formatting and interpretation removed.
  + If `value` is not a number or a reference to a cell containing a numeric value, `TO_PERCENT` returns `value` without modification.

### Notes

* `TO_PURE_NUMBER` is similar to applying Format -> Number -> Normal from the menu bar, except that the Normal format includes commas denoting thousands, millions, etc.
* `TO_PURE_NUMBER` is similar to `N`, except that `N` returns `0` for non-numeric values except for `TRUE` which returns `1`, whereas `TO_PURE_NUMBER` returns the value passed without modification for all non-numeric types.

### See Also

[[TO_TEXT]]: Converts a provided numeric value to a text value.

[[TO_PERCENT]]: Converts a provided number to a percentage.

[[TO_DOLLARS]]: Converts a provided number to a dollar value.

[[TO_DATE]]: Converts a provided number to a date.

[[N]]: Returns the argument provided as a number.

### Examples