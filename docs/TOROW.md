---
tags:
  - function
  - generated
  - array
---

This function transforms an array or range of cells into a single row. TOROW can scan values:

* By column, top to bottom
* By row, left to right

The `scan_by_column` argument is a boolean value that controls how TOROW reads values from the source array.

Sample Usage
------------

`TOROW(A1:C3)`: A `TOROW` function that keeps all values and scans by row.

`TOROW(A1:C3, 1, TRUE)`: A `TOROW` function that ignores blanks and scans by column.

Syntax
------

`TOROW(array_or_range, [ignore], [scan_by_column])`

* `array_or_range`: The array or range of cells to return as a row.
* `[ignore]`: By default, no values are ignored. Specify one of these values:
  + **0:** Keep all values
  + **1:** Ignore blanks
  + **2:** Ignore errors
  + **3:** Ignore blanks and errors
* `[scan_by_column]`: The boolean value of `scan_by_column` determines how the array is scanned. By default, the `TOROW` function scans the array by row.
  + **True:** scans the array by column
  + **False:** scans the array by row

Examples
--------

### Use simple data transformation operation with TOROW

**Example data:**

|  | **A** | **B** | **C** |
| --- | --- | --- | --- |
| **1** | Ben | Peter | Mary |
| **2** | John | Hillary | Jenny |
| **3** | Agnes | Harry | Felicity |

**Example:** Input this formula in `E1: =TOROW(A1:C3)`

**Result:**

|  | **E** | **F** | **G** | **H** | **I** | **J** | **K** | **L** | **M** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **1** | Ben | Peter | Mary | John | Hillary | Jenny | Agnes | Harry | Felicity |

[Make a Copy](https://docs.google.com/spreadsheets/d/1km45-ev3eD7ZS_J3PeSA7PLykpV71_98CqXq58vnXt8/copy)

### Ignore blanks with TOROW

**Example data:**

|  | **A** | **B** | **C** |
| --- | --- | --- | --- |
| **1** | Ben | Peter | Mary |
| **2** | John |  | Jenny |
| **3** | Agnes | Harry | Felicity |

**Example:** Input this formula in `E1: =TOROW(A1:C3, 1)`

**Result:**

|  | **E** | **F** | **G** | **H** | **I** | **J** | **K** | **L** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **1** | Ben | Peter | Mary | John | Jenny | Agnes | Harry | Felicity |

[Make a Copy](https://docs.google.com/spreadsheets/d/1km45-ev3eD7ZS_J3PeSA7PLykpV71_98CqXq58vnXt8/copy#gid=1425143757)

### Scan by column with TOROW

**Example data:**

|  | **A** | **B** | **C** |
| --- | --- | --- | --- |
| **1** | Ben | Peter | Mary |
| **2** | John | Hillary | Jenny |
| **3** | Agnes | Harry | Felicity |

**Example:** Input this formula in `E1: =TOROW(A1:C3, 0, TRUE)`

**Result:**

|  | **E** | **F** | **G** | **H** | **I** | **J** | **K** | **L** | **M** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **1** | Ben | John | Agnes | Peter | Hillary | Harry | Mary | Jenny | Felicity |

[Make a Copy](https://docs.google.com/spreadsheets/d/1km45-ev3eD7ZS_J3PeSA7PLykpV71_98CqXq58vnXt8/copy#gid=312714135)

Related functions
-----------------

* [[TOCOL]]: This function transforms an array or range of cells into a single column.