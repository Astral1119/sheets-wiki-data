Bad practice is a set of techniques, especially common ones, that result in [[Good practice|otherwise avoidable]] adverse effects.

### Using INDEX+MATCH instead of modern alternatives
While `INDEX+MATCH` is a common pattern in Excel, it is often a bad practice in Google Sheets because `INDEX` does not support array arguments for its row or column indices. This prevents the formula from "broadcasting" results when used inside an `ARRAYFORMULA`. Use `XLOOKUP` or `VLOOKUP` instead, as they are more concise and natively support array outputs.

### Using LEN for blank cell detection
Using `LEN(A1)` to check if a cell is empty is less efficient and less semantically clear than `ISBLANK(A1)`. Additionally, `LEN` returns 0 for cells containing empty strings `""`, which are not truly blank/null values.

### Runaway ARRAYFORMULA without controls
Using [[ARRAYFORMULA]] without output control can generate 50,000 rows of results, severely degrading sheet performance. Always use control structures:
- `IF(ISBLANK(...))` to limit expansion
- [[ARRAY_CONSTRAIN]] to cap output size

### Storing numbers or dates as text
Storing numeric data as text prevents mathematical operations, proper sorting, and date/time arithmetic. Convert text to proper types using `VALUE()`, `DATEVALUE()`, or `TIMEVALUE()`.

### See Also
- [[Good practice]] — recommended techniques
- [[Array-enabled functions]] — proper ARRAYFORMULA usage
- [[Type coercion]] — how types are converted