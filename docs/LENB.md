---
tags:
  - function
  - generated
  - text
---

The LENB function returns the length of a string in bytes.

Parts of a LENB function
------------------------

`LENB(string)`

| Part | Description |
| --- | --- |
| `string` | The string to get the length in bytes |

Notes
-----

`LENB` returns the same value as `LEN` if the input string has only single byte characters.

Examples
--------

| A | B | C |
| --- | --- | --- |
| **1** | **Input** | **Formula** | **Output** |
| **2** | Aeñ | `=LENB(A2)` | 3 |
| **3** | Aeñ | `=LEN(A3)` | 3 |
| **4** | `熊本` | `=LENB(A4)` | 4 |
| **5** | `熊本` | `=LEN(A5)` | 2 |

Related functions
-----------------

* [[MIDB]]: ​The MIDB function returns a section of a string starting at a given character and up to a specified number of bytes.
* [[LEFTB]]: The LEFTB function returns the left portion of a string up to a certain number of bytes.
* [[RIGHTB]]: The RIGHTB function returns the right portion of a string up to a certain number of bytes.