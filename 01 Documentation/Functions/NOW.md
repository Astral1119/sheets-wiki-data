Returns the current date and time as a date value.

### Sample Usage

`NOW()`

### Syntax

`NOW()`

### Notes

* Note that `NOW` is a volatile function, updating on every edit made to the spreadsheet, and can hurt spreadsheet performance.
* `NOW` provides the current date and time. To create a date without the current time, use [[TODAY]].
* `NOW` will always represent the current date and time the last time the spreadsheet was recalculated, rather than remaining at the date and time when it was first entered.
* The time or date component of NOW may be hidden by changing the number formatting on the cell. If either the date or time is not appearing, [[change the number formatting]].

### See Also

[[TODAY]]: Returns the current date as a date value.

[[DATEVALUE]]: Converts a provided date string in a known format to a date value.

[[DATE]]: Converts a year, month, and day into a date.

### Examples

Returns the computer system date and time.