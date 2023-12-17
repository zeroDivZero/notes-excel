# `INDEX()` and `MATCH()`

`VLOOKUP()` (and `HLOOKUP()`) limitations:

* lookup value must be in 1st col/row
* col/row index must be > 0
* slow

## `INDEX()`

Returns value in range, given row/col.

```excel
INDEX(array, row_num, [col_num])
```

* **array**: Cell range or array constant.
* **row_num**: Selects row in array to return value. If omitted, `col_num` required.
* **col_num**: Selects column in array to return value. If omitted, `row_num` required.

E.g.:

```excel
=INDEX('Emp List'!A1:I40,10,3)
```

Typically not useful by itself.

## `MATCH()`

Returns position in range, given value. Reverse of `INDEX()`.

```excel
MATCH(lookup_value,lookup_array,match_type)
```

* **lookup_value**: Value to match in array.
* **lookup_array**: Cell range containing lookup values.
* **match_type**: 1, 0, or -1 indicating how to match (1 is largest <= value, 0 is exact, -1 is smallest >= value).

E.g.:

```excel
=MATCH(A1,'Emp List'!$A$1:$A$40,0)
```

## Combine `INDEX()` and `MATCH()`

`INDEX()` returns value based on position, `MATCH()` returns position based on value, so to look up value B (position unknown) based on matching value A, can first find position of value A with `MATCH()`, and pass it as position to `INDEX()`:

```excel
=INDEX('Emp List'!$C$1:$C$38,MATCH(B4,'Emp List'!$D$1:$D$38,0))
```

Like `VLOOKUP()` and `HLOOKUP()`, but value A doesn't need to be at 1st col/row, and more performant.

Can do `MATCH()` for both row and column, only type formula once and applies to whole range:

```excel
=INDEX('Master Emp List'!$A$1:$I$38,MATCH($B10,'Master Emp List'!$A$1:$A$38,0),MATCH(D$2,'Master Emp List'!$A$1:$I$1,0))
```
