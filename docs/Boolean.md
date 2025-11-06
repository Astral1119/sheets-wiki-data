---
tags:
  - datatype
---

[Booleans](https://en.wikipedia.org/wiki/Boolean_data_type) represent logical values that can only be `TRUE` or `FALSE`. They are fundamental to conditional logic in Google Sheets formulas.

Other data types can behave like Booleans in certain contexts. Such values are known as ["truthy" and "falsy"](https://developer.mozilla.org/en-US/docs/Glossary/Truthy). While not genuine Booleans, these values can be [[Type coercion|coerced]] to logical equivalents.

When Booleans participate in mathematical operations, they are automatically converted to numbers:  
- `TRUE` becomes `1`  
- `FALSE` becomes `0`

When used in text operations, Booleans convert to their string representations:  
- `TRUE` becomes `"TRUE"`  
- `FALSE` becomes `"FALSE"`

For a complete reference of how Sheets coerces types, see [[Type Coercion]].

In Google Sheets, checkboxes correspond directly to Boolean values by default—checked for `TRUE`, and unchecked for `FALSE`.
