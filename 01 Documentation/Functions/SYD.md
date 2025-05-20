The SYD function calculates the depreciation of an asset for a specified period using the sum of years digits method.

### Sample Usage

`SYD(100,50,10,2)`

`SYD(A2,A3,A4,A5)`

### Syntax

`SYD(cost, salvage, life, period)`

* `cost` - The initial cost of the asset.
* `salvage` - The value of the asset at the end of depreciation.
* `life` - The number of periods over which the asset is depreciated.
* `period` - The single period within `life` for which to calculate depreciation.

### Notes

* `life` and `period` must be measured in the same units.

### See Also

[[SLN]]: The SLN function calculates the depreciation of an asset for one period using the straight-line method.

[[DDB]]: The DDB function calculates the depreciation of an asset for a specified period using the double-declining balance method.

[[DB]]: The DB function calculates the depreciation of an asset for a specified period using the arithmetic declining balance method.

### Examples