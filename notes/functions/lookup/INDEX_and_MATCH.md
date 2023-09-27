# `INDEX()` and `MATCH()`

`VLOOKUP()` (and `HLOOKUP()`) limitations:

* lookup value must be in 1st col/row
* col/row index must be > 0
* slow

## `INDEX()`

Returns val in range, given row and col.

```excel
INDEX(array, row_num, [col_num])
```

* **array**: Range of cells or array constant.
* **row_num**: Selects row in array to return val. If omitted, `col_num` is required.
* **col_num**: Selects col in array to return val. If omitted, `row_num` required.

E.g.:

```excel
=INDEX('Emp List'!A1:I40,10,3)
```

Typically not useful by itself.

## `MATCH()`

Returns position in range, given val. Reverse of `INDEX()`.

```excel
MATCH(lookup_value,lookup_array,match_type)
```

* **lookup_value**: Val to match in array.
* **lookup_array**: Range of cells containing lookup vals.
* **match_type**: 1, 0, or -1 indicating how to match (1 is largest <= val, 0 is exact, -1 is smallest >= val).

E.g.:

```excel
=MATCH(A1,'Emp List'!$A$1:$A$40,0)
```

## Combine `INDEX()` and `MATCH()`

`INDEX()` returns val based on pos, `MATCH()` returns pos based on val, so to look up val B (pos unknown) based on matching val A, can first find pos of val A with `MATCH()`, and pass it as pos to `INDEX()`:

```excel
=INDEX('Emp List'!$C$1:$C$38,MATCH(B4,'Emp List'!$D$1:$D$38,0))
```

Like `VLOOKUP()` and `HLOOKUP()`, but val A doesn't need to be at 1st col/row, and more performant.

Can do `MATCH()` for both row and col, only type formula once and apply to whole range:

```excel
=INDEX('Master Emp List'!$A$1:$I$38,MATCH($B10,'Master Emp List'!$A$1:$A$38,0),MATCH(D$2,'Master Emp List'!$A$1:$I$1,0))
```
