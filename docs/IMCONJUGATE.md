---
tags:
  - function
  - generated
  - engineering
---

Returns the complex conjugate of a number.

### Sample Usage

`IMCONJUGATE("3+4i")`

`IMCONJUGATE("-2i")`

### Syntax

`IMCONJUGATE(number)`

* `number` - The complex number to calculate the conjugate for.

### Notes

* The complex conjugate is defined as follows:
  + ![IMCONJUGATE Equation](https://lh3.googleusercontent.com/G-3CYkTX1itwNRCfgr7WX3E1yW6Df-qw5nE0JQfDPiUwhREvYz2xvLM77JR2xblzSkE=w116)

### See also

* [[COMPLEX]]: The COMPLEX function creates a complex number, given real and imaginary coefficients.
* [[IMREAL]]: Returns the real coefficient of a complex number.
* [[IMAGINARY]]: Returns the imaginary coefficient of a complex number.

### Examples

| **1** | A | B |
| --- | --- | --- |
| 2 | **Formula** | **Result** |
| 3 | `=IMCONJUGATE("3+4i")` | 3-4i |
| 4 | `=IMCONJUGATE(COMPLEX(-2, -5, "j"))` | -2+5j |