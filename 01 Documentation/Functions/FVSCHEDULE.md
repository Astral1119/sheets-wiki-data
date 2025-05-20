The FVSCHEDULE function calculates the future value of some principal based on a specified series of potentially varying interest rates.

### Sample Usage

`FVSCHEDULE(10000,A2:A100)`

`FVSCHEDULE(10000,{0.1,0.95,0.9,0.85})`

`FVSCHEDULE(A2,B2:B20)`

### Syntax

`FVSCHEDULE(principal, rate_schedule)`

* `principal` - The amount of initial capital or value to compound against.
* `rate_schedule` - A series of interest rates to compound against the `principal`.

  + `rate_schedule` must be either a range or array containing the interest rates to compound, in sequence. These should be expressed either as decimals or as percentages using `UNARY_PERCENT`, i.e. `0.09` or `UNARY_PERCENT(9)` rather than `9`.

### See Also

[[PV]]: Calculates the present value of an annuity investment based on constant-amount periodic payments and a constant interest rate.

[[PPMT]]: The PPMT function calculates the payment on the principal of an investment based on constant-amount periodic payments and a constant interest rate.

[[PMT]]: The PMT function calculates the periodic payment for an annuity investment based on constant-amount periodic payments and a constant interest rate.

[[NPER]]: The NPER function calculates the number of payment periods for an investment based on constant-amount periodic payments and a constant interest rate.

[[IPMT]]: The IPMT function calculates the payment on interest for an investment based on constant-amount periodic payments and a constant interest rate.

[[FV]]: The FV function calculates the future value of an annuity investment based on constant-amount periodic payments and a constant interest rate.

### Examples