Returns the absolute value of a complex number.

### Sample Usage

`IMABS("3+4i")`

`IMABS("6j")`

### Syntax

`IMABS(number)`

* `number` - The complex number to calculate the absolute value of.

### Notes

* The absolute value (or modulus) is defined as follows:
  + ​![IMABS Equation](//lh3.googleusercontent.com/l6uM1G4H0G_MMHVFb9bnKG78-hG7RwtzgBn_E3vk_coFFIAWbqgjcAOhVAdwT2Hxijs=w139)

### See also

* [[COMPLEX]]: The COMPLEX function creates a complex number, given real and imaginary coefficients.
* [[IMREAL]]: Returns the real coefficient of a complex number.
* [[IMAGINARY]]: Returns the imaginary coefficient of a complex number.

### Examples

| **1** | A | B |
| --- | --- | --- |
| 2 | **Formula** | **Result** |
| 3 | `=IMABS("3+4i")` | 5 |
| 4 | `=IMABS(COMPLEX(3, 4, "j"))` | 5 |