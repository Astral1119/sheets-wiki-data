---
tags:
  - function
  - generated
  - financial
---

Calculates the present value of an annuity investment based on constant-amount periodic payments and a constant interest rate.

### Sample Usage

`PV(2,12,100)`

`PV(A2,B2,C2,D2,1)`

### Syntax

`PV(rate, number_of_periods, payment_amount, [future_value], [end_or_beginning])`

* `rate` - The interest rate.
* `number_of_periods` - The number of payments to be made.
* `payment_amount` - The amount per period to be paid.
* `future_value` - **[** OPTIONAL **]** - The future value remaining after the final payment has been made.
* `end_or_beginning` - **[** OPTIONAL - `0` by default **]** - Whether payments are due at the end (`0`) or beginning (`1`) of each period.

### Notes

* Ensure that consistent units are used for `rate`, `number_of_periods`, and `payment_amount​`. For example, a car loan for 36 months may be paid monthly, in which case the annual percentage rate should be divided by 12 and the number of payments is 36. On the other hand, a different type of loan of the same length might be paid quarterly, in which case the annual percentage rate should be divided by 4 and the number of payments would be 12.

### See Also

[[PPMT]]: The PPMT function calculates the payment on the principal of an investment based on constant-amount periodic payments and a constant interest rate.

[[PMT]]: The PMT function calculates the periodic payment for an annuity investment based on constant-amount periodic payments and a constant interest rate.

[[NPER]]: The NPER function calculates the number of payment periods for an investment based on constant-amount periodic payments and a constant interest rate.

[[IPMT]]: The IPMT function calculates the payment on interest for an investment based on constant-amount periodic payments and a constant interest rate.

[[FVSCHEDULE]]: The FVSCHEDULE function calculates the future value of some principal based on a specified series of potentially varying interest rates.

[[FV]]: The FV function calculates the future value of an annuity investment based on constant-amount periodic payments and a constant interest rate.

### Examples

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdFVmbWVWSDdwMXA2NEdGMVlIRGlyd1E&amp;output=html" width="500"></iframe>