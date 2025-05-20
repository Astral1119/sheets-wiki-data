Calculates the yield of a US Treasury Bill based on price.

### Sample Usage

`TBILLYIELD(DATE(2010,1,2), DATE(2010,12,31), 98.45)`

`TBILLYIELD(A2,B2,C2)`

### Syntax

`TBILLYIELD(settlement, maturity, price)`

* `settlement` - The settlement date of the security, the date after issuance when the security is delivered to the buyer.
* `maturity` - The maturity or end date of the security, when it can be redeemed at face or par value.
* `price` - The price at which the security is bought.

### Notes

* `TBILLYIELD` requires the maturity date to be no more than a year after the settlement date.
* `settlement` and `maturity` should be entered using `DATE`, `TO_DATE` or other date parsing functions rather than by entering text.
* `TBILLYIELD` is equivalent to using `YIELDDISC` with US Treasury Bill conventions for the absent parameters.

### See Also

[[YIELDDISC]]: Calculates the annual yield of a discount (non-interest-bearing) security, based on price.

[[YIELD]]: Calculates the annual yield of a security paying periodic interest, such as a US Treasury Bond, based on price.

### Examples