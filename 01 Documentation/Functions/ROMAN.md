Formats a number in Roman numerals.

### Sample Usage

`ROMAN(499,0)`

`ROMAN(A2)`

### Syntax

`ROMAN(number, [rule_relaxation])`

* `number` - The number to format, between 1 and 3999, inclusive.
* `rule_relaxation` - **[** OPTIONAL - 0 by default **]** - The degree to which traditional syntax rules may be relaxed, between `0` and `4` inclusive.

  + `0` indicates strict precedence rules, where `I` may only precede `V` and `X`, `V` may only precede `X`, `X` may only precede `L` and `C`, `L` may only precede `C`, and `C` may only precede `D` and `M`. Therefore `ROMAN(499,0)` is `CDXCIX`.
  + `1` indicates a relaxation where `V` may precede `L` and `C` and `L` may precede `D` and `M`. Therefore `ROMAN(499,1)` is `LDVLIV`.
  + `2` indicates a further relaxation where `I` may precede `L` and `C`, and `X` may precede `D` and `M`. Therefore `ROMAN(499,2)` is `XDIX`.
  + `3` indicates a further relaxation where `V` may precede `D` and `M`. Therefore `ROMAN(499,3)` is `VDIV`.
  + `4` indicates a further relaxation where `I` may precede `D` and `M`. Therefore `ROMAN(499,4)` is `ID`.

### See Also

[[ARABIC]]: Computes the value of a Roman numeral.

### Examples