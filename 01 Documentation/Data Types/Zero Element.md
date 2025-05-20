> [!WARNING]
> Zero elements are not an officially recognized feature and may be a [[bug]].

Zero elements are a type of [[array]] with zero width or zero height.
## Syntax

| Dimensions | Formula               |
| ---------- | --------------------- |
| 0 x 1      | `TOCOL(,1)`           |
| 1 x 0      | `TOROW(,1)`           |
| 0 x 0      | `ARRAY_CONSTRAIN(,,)` |
## Notes
- Zero elements can be used in [[REDUCE]] or [[LAMBDA recursion]] formulae to effectively skip the initial value when using [[VSTACK]] or [[Array#Array Literals|array literals]] on the accumulator.