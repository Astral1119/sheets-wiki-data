---
tags:
  - function
  - generated
  - financial
---

The DB function calculates the depreciation of an asset for a specified period using the arithmetic declining balance method.

### Sample Usage

`DB(100,50,10,2)`

`DB(A2,A3,A4,A5,10)`

### Syntax

`DB(cost, salvage, life, period, [month])`

* `cost` - The initial cost of the asset.
* `salvage` - The value of the asset at the end of depreciation.
* `life` - The number of periods over which the asset is depreciated.
* `period` - The single period within `life` for which to calculate depreciation.
* `month` - **[** OPTIONAL - `12` by default **]** - The number of months in the first year of depreciation.

### Notes

* `life` and `period` must be measured in the same units.

### See Also

[[SYD]]: The SYD function calculates the depreciation of an asset for a specified period using the sum of years digits method.

[[SLN]]: The SLN function calculates the depreciation of an asset for one period using the straight-line method.

[[DDB]]: The DDB function calculates the depreciation of an asset for a specified period using the double-declining balance method.

### Examples

<iframe height="300" src="https://docs.google.com/spreadsheet/pub?key=0As3tAuweYU9QdFVENTJwRVNmWEx2YmtYcmFEWF9Rb3c&amp;output=html" width="500"></iframe>