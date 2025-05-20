This function creates a new array from the selected columns in the existing range.

Sample Usage
------------

`CHOOSECOLS(A1:E5, 1, 3, 1)`

`CHOOSECOLS(A1:E5, -1, -2, -3)`

Syntax
------

`CHOOSECOLS(array, col_num1, [col_num2])`

* `array`: The array that contains the columns to be returned.
* `col_num1`: The column number of the first column to be returned.
* `col_num2…`: **[** OPTIONAL **]** The column number(s) of additional column(s) to be returned.

Examples
--------

### Simple data extraction operation with CHOOSECOLS

**Example data:**

|  | **A** | **B** | **C** | **D** | **E** |
| --- | --- | --- | --- | --- | --- |
| **1** | **Student** | **Math** | **History** | **Science** | **Gym** |
| **2** | Harry | 95 | 70 | 82 | 78 |
| **3** | Jenny | 85 | 91 | 100 | 80 |
| **4** | Lily | 76 | 88 | 80 | 95 |
| **5** | Sunny | 60 | 77 | 89 | 80 |

**Example:** Input this formula in G1: `=CHOOSECOLS(A1:E5, 1, 3, 2)`

**Result:**

|  | **G** | **H** | **I** |
| --- | --- | --- | --- |
| **1** | Student | History | Math |
| **2** | Harry | 70 | 95 |
| **3** | Jenny | 91 | 85 |
| **4** | Lily | 88 | 76 |
| **5** | Sunny | 77 | 60 |

[Make a Copy](https://docs.google.com/spreadsheets/d/1rBlIiOQJDThG1KvNix1xC5OuJWO-O3lbQp7FRXgauSw/copy)

### Simple data extraction with CHOOSECOLS selecting columns from the right side

**Example data:**

|  | **A** | **B** | **C** | **D** | **E** |
| --- | --- | --- | --- | --- | --- |
| **1** | **Student** | **Math** | **History** | **Science** | **Gym** |
| **2** | Harry | 95 | 70 | 82 | 78 |
| **3** | Jenny | 85 | 91 | 100 | 80 |
| **4** | Lily | 76 | 88 | 80 | 95 |
| **5** | Sunny | 60 | 77 | 89 | 80 |

**Example:** Input this formula in G1: `=CHOOSECOLS(A1:E5, 1, -1, -2)`

**Result:**

|  | **G** | **H** | **I** |
| --- | --- | --- | --- |
| **1** | Student | Gym | Science |
| **2** | Harry | 78 | 82 |
| **3** | Jenny | 80 | 100 |
| **4** | Lily | 95 | 80 |
| **5** | Sunny | 80 | 89 |

[Make a Copy](https://docs.google.com/spreadsheets/d/1rBlIiOQJDThG1KvNix1xC5OuJWO-O3lbQp7FRXgauSw/copy#gid=907400634)

Related functions
-----------------

* [[CHOOSEROWS]]