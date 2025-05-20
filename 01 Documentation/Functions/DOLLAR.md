Formats a number into the locale-specific currency format.

### Sample Usage

`DOLLAR(1.2351,4)`

`DOLLAR(2.35)`

### Syntax

`DOLLAR(number, [number_of_places])`

* `number` - The value to be formatted.
* `number_of_places` - **[** OPTIONAL - `2` by default **]** - The number of decimal places to display.

### Notes

* The currency format used by `DOLLAR` is specific to your spreadsheet locale.
* `DOLLAR` differs from the related function `TO_DOLLARS` in that `DOLLAR` outputs text rather than applying a cell format to a number.

### See Also

[[TO_DOLLARS]]: Converts a provided number to a dollar value.
