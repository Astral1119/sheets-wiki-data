---
tags:
  - function
  - generated
  - math
description: Returns the result of the modulo operator, the remainder after a division operation.
---
> [!INFO]
> This page was originally generated from [official documentation](https://support.google.com/docs/answer/3093497?hl=en).

Returns the result of the modulo operator, the remainder after a division operation.

### Sample Usage

```gse
MOD(10,4)
MOD(A2,B2)
```

### Syntax

```gse
MOD(dividend, divisor)
```

- `dividend` - The number to be divided to find the remainder.
- `divisor` - The number to divide by.

### Notes

The `MOD` function also applies on non-integer numbers but may result in an approximate result due to the use of floating point arithmetic. You can use the `ROUND` function to round the output up or down to get the expected result.

### Examples

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdE9wbTV5RkQ5MXZLaE4xaGp6R1RqOXc&amp;output=html" width="500"></iframe>