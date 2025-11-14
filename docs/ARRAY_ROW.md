---
tags:
  - function
  - array
  - undocumented
---

Constructs a vertical [[Array#Vectors|vector]].

### Sample Usage

```gse
ARRAY_ROW(1, 2, A1)
```

### Syntax

```gse
ARRAY_ROW(value1, [value2, ...])
```

- `value1` - The first value in the vector.
- `value2, ...` - **[** OPTIONAL **]** - Additional values to add to the vector.

### Notes

- Each `value` must either be a [[Data type#Scalar types|scalar type]] or a vertical vector.

### See Also

- [[ARRAY_LITERAL]]
- [[ARRAY_CONSTRAIN]]
- [[HSTACK]]
- [[VSTACK]]