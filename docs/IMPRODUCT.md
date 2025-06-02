---
tags:
  - function
  - generated
  - engineering
---

Returns the result of multiplying a series of complex numbers together.

### Sample Usage

`IMPRODUCT(A2:A100)`

`IMPRODUCT("1+2i",3,"4i")`

`IMPRODUCT("1+2i","3+5i",A2:A50)`

### Syntax

`IMPRODUCT(factor1, [factor2, ...])`

* `factor1` - The first complex number or range to calculate for the product.
* `factor2`, ... - [ OPTIONAL ] - More complex numbers to multiply by.

### Notes

* The product of two complex numbers is defined as follows:
  + (a+bi)(c+di) = (ac-bd) + (ad+bc)i
* You can multiply complex numbers only if they have the same suffix (i or j). For example, you can't do `IMPRODUCT("4+3i", "1+2j")`.

### See also

* [[COMPLEX]]: The COMPLEX function creates a complex number, given real and imaginary coefficients.
* [[IMREAL]]: Returns the real coefficient of a complex number.
* [[IMAGINARY]]: Returns the imaginary coefficient of a complex number.
* [[IMDIV]]: Returns one complex number divided by another.
* [[IMSUM]]: Returns the sum of a series of complex numbers or cells or both.

### Examples

| 2 | Formula | Result |
| --- | --- | --- |
| **3** | `=IMPRODUCT(COMPLEX(3, 4), 2)` | 6+8i |
| **4** | `=IMPRODUCT("3+4i", "2i", "2i")` | -12-16i |