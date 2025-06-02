---
tags:
  - function
  - generated
  - math
---

The `IMPOWER` function returns a complex number raised to a power.

### Parts of a IMPOWER formula

The `IMPOWER` formula is formatted as `=IMPOWER(complex_base, exponent).`

| **Part** | **Description** | **Notes** |
| `complex_base` | The complex number to raise to the exponent power. | * May be written as a ∓ bi or a ∓ bj. |
| `exponent` | The exponent to raise complex\_base to. | * Must be a number. |

### Sample formulas

`IMPOWER("4-3i",0.5)`

`IMPOWER(A2,B2)`

`IMPOWER("2j",-7)`



### Notes

* The exponentiation of a complex number is defined as follows:
  + (a+bi)n = rn(cosθ + isinθ), where
  + r = √(x2 + y2) and θ = arctan(b/a)

### Examples

|  | A | B |
| --- | --- | --- |
| 1 | **Formula** | **Result** |
| 2 | `=IMPOWER("5+2i", 3)` | 65+142i |
| 3 | `=IMPOWER("-1-j", -1)` | -0.5+0.5j |
| 4 | `=IMPOWER("0.732-5.349i", -0.138)` | 0.776914096672106+0.155872432042838i |

### Related functions

[[COMPLEX]]: The COMPLEX function creates a complex number, given real and imaginary coefficients.

[[IMREAL]]: Returns the real coefficient of a complex number.

[[IMAGINARY]]: Returns the imaginary coefficient of a complex number.

[[POWER]]: Returns a number raised to a power.