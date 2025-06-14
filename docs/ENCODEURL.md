---
tags:
  - function
  - generated
  - web
---

Encodes text so it can be used in the query string of a URL.

Parts of an ENCODEURL function
------------------------------

`ENCODEURL(text)`

| Part | Description |
| --- | --- |
| `text` | The text to be encoded as a URL. |

Sample formulas
---------------

`ENCODEURL(“hello world!”)`

`ENCODEURL(A10)`

Notes
-----

This function is useful for passing in URL arguments to functions that make web requests, like IMPORTHTML.

Examples
--------

Encode the text “hello, world!” into a URL-friendly format.

| 1 | Formula | Result |
| --- | --- | --- |
| **2** | =ENCODEURL(“hello, world!”) | hello%2C%20world%21 |

Use ENCODEURL to create a hyperlink.

| 1 | Formula | Result |
| --- | --- | --- |
| **2** | =HYPERLINK("http://google.com?q=" & ENCODEURL("hello world")) | http://google.com?q=hello%20world |

Related functions
-----------------

* [[IMPORTHTML]]:  Imports data from a table or list within an HTML page.
* [[CLEAN]]:  Returns the text with the non-printable ASCII characters removed.
* [[REPLACE]]:  Replaces part of a text string with a different text string.