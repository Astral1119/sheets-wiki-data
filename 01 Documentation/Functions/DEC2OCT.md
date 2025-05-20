The DEC2OCT function converts a decimal number to signed octal format.

### Sample Usage

`DEC2OCT("100",8)`

`DEC2OCT(A2)`

### Syntax

`DEC2OCT(decimal_number, [significant_digits])`

* `decimal_number` - The decimal value to be converted to signed octal, provided as a string.

  + For this function, this value has a maximum of 536870911 if positive, and a minimum of -53687092 if negative.
  + If `decimal_number` is provided as a valid decimal number, it will automatically be converted to the appropriate string input. For example, `DEC2OCT(199)` and `DEC2OCT("199")` yield the same result: `307`.
* `significant_digits` - **[** OPTIONAL **]** The number of significant digits to ensure in the result.

  + If this is greater than the number of significant digits in the result, the result is left-padded with zeros until the total number of digits reaches `significant_digits`.
  + This value is ignored if `decimal_number` is negative.

### Notes

* If the number of digits required is greater than the specified `significant_digits`, the `#NUM!` error is returned.
* Ensure that any calculations using the result of DEC2OCT take into account that it is in octal. Results will be silently converted by Google Sheets; thus if cell `A2` contains `111`, the octal equivalent of the decimal value `73`, and `B2` contains a formula such as `=A2+9`, the result will be `120`, which is incorrect in octal calculation.

### See Also

[[OCT2HEX]]: The OCT2HEX function converts a signed octal number to signed hexadecimal format.

[[OCT2DEC]]: The OCT2DEC function converts a signed octal number to decimal format.

[[OCT2BIN]]: The OCT2BIN function converts a signed octal number to signed binary format.

[[HEX2OCT]]: The HEX2OCT function converts a signed hexadecimal number to signed octal format.

[[HEX2DEC]]: The HEX2DEC function converts a signed hexadecimal number to decimal format.

[[HEX2BIN]]: The HEX2BIN function converts a signed hexadecimal number to signed binary format.

[[DEC2HEX]]: The DEC2HEX function converts a decimal number to signed hexadecimal format.

[[DEC2BIN]]: The DEC2BIN function converts a decimal number to signed binary format.

[[BIN2OCT]]: The BIN2OCT function converts a signed binary number to signed octal format.

[[BIN2HEX]]: The BIN2HEX function converts a signed binary number to signed hexadecimal format.

[[BIN2DEC]]: The BIN2DEC function converts a signed binary number to decimal format.
