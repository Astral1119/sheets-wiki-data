---
tags:
  - function
  - generated
  - text
---
> [!INFO]
> This page was originally generated from [official documentation](https://support.google.com/docs/answer/9367697?hl=en).

The RIGHTB function returns the right portion of a string up to a certain number of bytes.

### Syntax
```gse
RIGHTB(string, num_of_bytes)
```

| Part | Description |
| --- | --- |
| `string` | The string from which the right portion will be returned. |
| `num_of_bytes` | (Optional) The number of bytes to return from the right side of `string`. |

### Notes

- `RIGHTB` returns the same value as `RIGHT` if the input string has only single byte characters
- `num_of_bytes` must be greater than or equal to zero.
- If `num_of_bytes` is greater than the length of text in bytes, `RIGHTB` returns all of text.
- If `num_of_bytes` is omitted, it is assumed to be 1.

### Examples

| A | B | C |
| --- | --- | --- |
| **1** | **Input** | **Formula** | **Output** |
| **2** | Aeñ | `=RIGHTB(A2, 2)` | eñ |
| **3** | Aeñ | `=RIGHT(A3,2)` | eñ |
| **4** | `熊本` | `=RIGHTB(A4, 2)` | 本 |
| **5** | `熊本` | `=RIGHT(A5,2)` | 熊本 |

### Related functions

- [[MIDB]]:The MIDB function returns a section of a string starting at a given character and up to a specified number of bytes.
- [[LEFTB]]: The LEFTB function returns the left portion of a string up to a certain number of bytes.
- [[LENB]]: The LENB function returns the length of a string in bytes.