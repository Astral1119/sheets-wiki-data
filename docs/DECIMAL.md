---
tags:
  - function
  - generated
  - math
---

The DECIMAL function converts the text representation of a number in another base, to base 10 (decimal).

Parts of a DECIMAL formula
--------------------------

`DECIMAL(value, base)`

| Part | Description | Notes |
| --- | --- | --- |
| `value` | The unsigned value to be converted to decimal, provided as a string. |  |
| `base` | The base (or radix) to convert the number into. | The base is an integer from 2 to 36. |

Sample formula
--------------

`DECIMAL(101,2)`

Notes
-----

* The string representation of the value is used, which should only contain numeric characters (i.e. scientific notation isn't permitted). The text of a string should be no longer than 255 characters.
* The DECIMAL function only converts to positive integers.

Example
-------

| A | B |
| --- | --- |
| **1** | **Formula** | **Result** |
| **2** | =DECIMAL(101,2) | 5 |

Related functions
-----------------

* [[BASE]]: The BASE function converts a decimal number into a text representation in another base.
* [[BIN2DEC]]: The BIN2DEC function converts a signed binary number to decimal format.
* [[BIN2HEX]]: The BIN2HEX function converts a signed binary number to signed hexadecimal format.
* [[BIN2OCT]]: The BIN2OCT function converts a signed binary number to signed octal format.
* [[OCT2BIN]]: The OCT2BIN function converts a signed octal number to signed binary format.
* [[OCT2DEC]]: The OCT2DEC function converts a signed octal number to decimal format.
* [[OCT2HEX]]: The OCT2HEX function converts a signed octal number to signed hexadecimal format.
* [[DEC2BIN]]: The DEC2BIN function converts a decimal number to signed binary format.
* [[DEC2OCT]]: The DEC2OCT function converts a decimal number to signed octal format.
* [[DEC2HEX]]: The DEC2HEX function converts a decimal number to signed hexadecimal format.
* [[HEX2DEC]]: The HEX2DEC function converts a signed hexadecimal number to decimal format.
* [[HEX2BIN]]: The HEX2BIN function converts a signed hexadecimal number to signed binary format.
* [[HEX2OCT]]: The HEX2OCT function converts a signed hexadecimal number to signed octal format.