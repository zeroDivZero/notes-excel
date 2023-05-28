# `VLOOKUP()`

Vertical lookup. Looks for val in leftmost col of table, returns val in same row at specified col. By default, table must be sorted in ascending order.

```excel
VLOOKUP(lookup_value,table_array,col_index_num,range_lookup)
```

* **lookup_value**: Val to be found in 1st col of table. Can be val, ref, or text.
* **table_array**: Table of text, numbers, or logical vals, in which data is retrieved; can be range ref or name.
* **col_index_num**: Col num in **table_array** from which matching val should be returned. 1st col is 1.
* **range_lookup**: Logical val, to find closest match in 1st col (sorted in ascending order) = `TRUE` or omitted; find exact match = `FALSE`.

## Example

```excel
=VLOOKUP($B3,'Emp List'!$A$1:$I$38,4,FALSE)
```
