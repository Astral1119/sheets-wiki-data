The DDB function calculates the depreciation of an asset for a specified period using the double-declining balance method.

### Sample Usage

`DDB(100,50,10,2)`

`DDB(A2,A3,A4,A5,2.25)`

### Syntax

`DDB(cost, salvage, life, period, [factor])`

* `cost` - The initial cost of the asset.
* `salvage` - The value of the asset at the end of depreciation.
* `life` - The number of periods over which the asset is depreciated.
* `period` - The single period within `life` for which to calculate depreciation.
* `factor` - **[** OPTIONAL - `2` by default **]** - The factor by which depreciation decreases.

### Notes

* `life` and `period` must be measured in the same units.
* While `DDB` calculates double-declining depreciation by default, use of `factor` allows specification of other methods.

### See Also

[[SYD]]: The SYD function calculates the depreciation of an asset for a specified period using the sum of years digits method.

[[SLN]]: The SLN function calculates the depreciation of an asset for one period using the straight-line method.

[[DB]]: The DB function calculates the depreciation of an asset for a specified period using the arithmetic declining balance method.
