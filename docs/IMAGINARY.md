---
tags:
  - function
  - generated
  - engineering
---

Returns the imaginary coefficient of a complex number.

### Sample Usage

```gse
IMAGINARY("4+5i")
IMAGINARY("2j")
```

### Syntax

```gse
IMAGINARY(complex_number)
```

- `complex_number` - The complex number, in the a+bi or a+bj format.

### See also

- [[COMPLEX]]: The COMPLEX function creates a complex number, given real and imaginary coefficients.
- [[IMREAL]]: Returns the real coefficient of a complex number.

### Examples

| 2 | Formula | Result |
| --- | --- | --- |
| **3** | `=IMAGINARY("3+5i")` | 5 |
| **4** | `=IMAGINARY("4j")` | 4 |
| **5** | `=IMAGINARY("45")` | 0 |