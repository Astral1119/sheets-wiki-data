---
tags:
  - function
  - generated
  - modified
---

Converts a number to Thai text with the suffix [Baht](https://en.wikipedia.org/wiki/Thai_baht) for integer values and Satang for decimal values.

### Sample Usage

```gse
BAHTTEXT(12)
BAHTTEXT(120.75)
```

### Syntax

```gse
BAHTTEXT(value)
```

- `value` - The [[number]] to convert to Thai text.

### Notes
- This function is sometimes used in conjunction with [[GOOGLETRANSLATE]] to convert [[number|numbers]] to their text representations (e.g. `13` to `thirteen`).
