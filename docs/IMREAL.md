---
tags:
  - function
  - generated
  - engineering
---

Returns the real coefficient of a complex number.

### Sample Usage

`IMREAL("4+5i")`

`IMREAL("4j")`

### Syntax

`IMREAL(complex_number)`

* `complex_number` - The complex number, in the a+bi or a+bj format.

### See also

* [[COMPLEX]]: The COMPLEX function creates a complex number, given real and imaginary coefficients.
* [[IMAGINARY]]: Returns the imaginary coefficient of a complex number.

### Examples

| 2 | Formula | Result |
| --- | --- | --- |
| **3** | `=IMREAL("3+5i")` | 3 |
| **4** | `=IMREAL("4j")` | 0 |