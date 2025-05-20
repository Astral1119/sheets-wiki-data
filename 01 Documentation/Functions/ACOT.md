The ACOT function returns the inverse cotangent of a value in radians.

## Syntax

`ACOT(value)`

|          |                                                         |                            |
| -------- | ------------------------------------------------------- | -------------------------- |
| **Part** | **Description**                                         | **Notes**                  |
| `value`  | The value for which to calculate the inverse cotangent. | * Values must be a number. |

## Notes

* ACOT returns results that are between 0 and π (pi).
* ACOT is sometimes written as "arccot" or "cot-1(x)" in mathematics or other programs.
* Use the DEGREES function to convert the result of ACOT from radians to degrees.

Examples
--------

This example shows the inverse cotangent of numbers in radians:

|       |             |               |
| ----- | ----------- | ------------- |
|       | **A**       | **B**         |
| **1** | **Formula** | **Result**    |
| **2** | =ACOT(4)    | 0.2449786631  |
| **3** | =ACOT(-4)   | -0.2449786631 |
| **4** | =ACOT(0)    | 1.570796327   |

This example shows the inverse cotangent of numbers converted to degrees:

|       |          |                    |              |
| ----- | -------- | ------------------ | ------------ |
|       | **A**    | **B**              | **C**        |
| **1** | **Data** | **Formula**        | **Result**   |
| **2** | 4        | =DEGREES(ACOT(A2)) | 14.03624347  |
| **3** | -4       | =DEGREES(ACOT(A3)) | -14.03624347 |
| **4** | 0        | =DEGREES(ACOT(A4)) | 90           |



## Related Functions

* [[ACOTH]]: The ACOTH function returns the inverse hyperbolic cotangent of a value in radians.
* [[COT]]: The COT function returns the cotangent of an angle provided in radians.
* [[COTH]]: The COTH function returns the hyperbolic cotangent of any real number.
* [[ATANH]]: The ATANH function returns the inverse hyperbolic tangent of a number.
* [[ATAN]]: The ATAN function returns the inverse tangent of a value in radians.
* [[ASINH]]: The ASINH function returns the inverse hyperbolic sine of a number.
* [[ASIN]]: The ASIN function returns the inverse sine of a value in radians.
* [[ACOSH]]: The ACOSH function returns the inverse hyperbolic cosine of a number.
* [[ACOS]]: The ACOS function returns the inverse cosine of a value in radians.
* [[DEGREES]]: The DEGREES function converts an angle value in radians to degrees.
* [[RADIANS]]: The RADIANS function converts an angle value in degrees to radians.
* [[PI]]: The PI function returns the value of pi to 9 decimal places.