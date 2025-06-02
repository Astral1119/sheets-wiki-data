---
tags:
  - function
  - generated
  - financial
---

The PPMT function calculates the payment on the principal of an investment based on constant-amount periodic payments and a constant interest rate.

### Sample Usage

`PPMT(0.05/12, 1, 30*12, 100000)`

`PPMT(2,5,12,100)`

`PPMT(A2,B2,C2,D2,E2,1)`

### Syntax

`PPMT(rate, period, number_of_periods, present_value, [future_value, end_or_beginning])`

* `rate` - The interest rate.
* `period` - The amortization period, in terms of number of periods.

  + `period` must be at least `1` and at most `number_of_periods`.
* `number_of_periods` - The number of payments to be made.
* `present_value` - The current value of the annuity.
* `future_value` - **[** OPTIONAL **]** - The future value remaining after the final payment has been made.
* `end_or_beginning` - **[** OPTIONAL - `0` by default **]** - Whether payments are due at the end (`0`) or beginning (`1`) of each period.

### Notes

* Ensure that consistent units are used for `rate` and `number_of_periods`. For example, a car loan for 36 months may be paid monthly, in which case the annual percentage rate should be divided by 12 and the number of payments is 36. On the other hand, a different type of loan of the same length might be paid quarterly, in which case the annual percentage rate should be divided by 4 and the number of payments would be 12.

### See Also

[[PV]]: Calculates the present value of an annuity investment based on constant-amount periodic payments and a constant interest rate.

[[PMT]]: The PMT function calculates the periodic payment for an annuity investment based on constant-amount periodic payments and a constant interest rate.

[[NPER]]: The NPER function calculates the number of payment periods for an investment based on constant-amount periodic payments and a constant interest rate.

[[IPMT]]: The IPMT function calculates the payment on interest for an investment based on constant-amount periodic payments and a constant interest rate.

[[FVSCHEDULE]]: The FVSCHEDULE function calculates the future value of some principal based on a specified series of potentially varying interest rates.

[[FV]]: The FV function calculates the future value of an annuity investment based on constant-amount periodic payments and a constant interest rate.

### Examples

General usage

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdFR1aTNoMmFlSVdMSW4tWnVIOFRHdVE&amp;output=html" width="500"></iframe>

Principal payment on a mortgage

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdFR1aTNoMmFlSVdMSW4tWnVIOFRHdVE&amp;gid=6&amp;single=true&amp;widget=true&amp;output=html" width="500"></iframe>