---
tags:
  - function
  - generated
  - array
---

Flattens all the values from one or more ranges into a single column.

### Parts of a FLATTEN function

=FLATTEN(range1, [range2, …])

| Part | Description |
| --- | --- |
| range1 | The first range to flatten. |
| range2 | [optional] repeatable  Additional ranges to flatten. |

### Sample formulas

=FLATTEN(A1:B2)

=FLATTEN("top", A1:B2, "middle", B3:B4, "bottom")

### Notes

* Values are ordered by argument, then row, then column. So, the entire first row of an input is added before the second row (also known as **row-major order**).
* Empty values are not skipped; the FILTER function can be used to remove those.

### Examples

[Make a copy](https://docs.google.com/spreadsheets/d/1hfr9gx1BAaq5RjPc1VpSfgajJ2sWkrPxrErgPIwiBR4/copy)

Flatten will append arguments in the order they are included in the formula. Arguments need not be range references.

| A | B | C | D |
| --- | --- | --- | --- |
| **1** | 1 | 2 | **Formula in D1:**  **=FLATTEN(A1:B2, "sample middle", B3:B4)** | 1 |
| **2** | 3 | 4 |  | 2 |
| **3** |  | 5 |  | 3 |
| **4** |  | 6 |  | 4 |
| **5** |  |  |  | sample middle |
| **6** |  |  |  | 5 |
| **7** |  |  |  | 6 |

A more complex example, using the CONCAT (&) operator and SPLIT to do a simple **cross join** or **Cartesian product** on two lists.

| A | B | C | D | E |
| --- | --- | --- | --- | --- |
| **1** | A | 1 | **Formula in D1: =ArrayFormula(SPLIT(FLATTEN(A1:A3 & "|" & TRANSPOSE(B1:B2)), "|"))** | A | 1 |
| **2** | B | 2 |  | A | 2 |
| **3** | C |  |  | B | 1 |
| **4** |  |  |  | B | 2 |
| **5** |  |  |  | C | 1 |
| **6** |  |  |  | C | 2 |

### Related functions

* [[SPLIT]]
* [[TRANSPOSE]]
* [[SORT]]
* [[UNIQUE]]
* [[FILTER]]