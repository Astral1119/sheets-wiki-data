This function appends ranges vertically and in sequence to return a larger array.

Sample Usage
------------

`VSTACK(A2:C4; A6:C8)`

Syntax
------

`VSTACK(range1; [range2, …])`

* `range1`: The first range to append.
* `range2, …`: **[** OPTIONAL **]** Additional ranges to add to range1.

Examples
--------

### Simple append operation with VSTACK

**Example data:**

|  | **A** | **B** | **C** |
| --- | --- | --- | --- |
| **1** | **Warehouse A Item** | **Warehouse A Color** | **Warehouse A Quantity** |
| **2** | Jeans | Blue | 100 |
| **3** | T-shirt | Pink | 110 |
| **4** | Shorts | Red | 120 |
| **5** | **Warehouse B Item** | **Warehouse B Color** | **Warehouse B Quantity** |
| **6** | Skirt | Pink | 150 |
| **7** | T-shirt | Black | 100 |
| **8** | Shoes | Grey | 50 |

**Example:** Input this formula in `E2: =VSTACK(A2:C4;A6:C8)`

**Result:**

|  | **E** | **F** | **G** |
| --- | --- | --- | --- |
| **1** | **Warehouse Item** | **Warehouse Color** | **Warehouse Quantity** |
| **2** | Jeans | Blue | 100 |
| **3** | T-shirt | Pink | 110 |
| **4** | Shorts | Red | 120 |
| **5** | Skirt | Pink | 150 |
| **6** | T-shirt | Black | 100 |
| **7** | Shoes | Grey | 50 |

[Make a Copy](https://docs.google.com/spreadsheets/d/1ziuOJPL93SxBq0aF5KiQ4vhntnqg2BgvdUYWOedjdnE/copy)

Related functions
-----------------

* [[HSTACK]]