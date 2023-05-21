# `VLOOKUP()`

Vertical lookup. Looks for val in leftmost col of table, returns val in same row from col specified. By default, table must be sorted in ascending order.

```excel
VLOOKUP(lookup_value,table_array,col_index_num,range_lookup)
```

* **Lookup_value**: val to be found in first column of table; can be val, ref, or text.
* **Table_array**: table of text, numbers, or logical vals, in which data is retrieved; can be range ref or name.
* **Col_index_num**: col num in **table_array** from which matching val should be returned; 1st col is 1.
* **Range_lookup**: logical val, to find closest match in 1st col (sorted in ascending order) = `TRUE` or omitted; find exact match = `FALSE`.

## Example

```excel
=VLOOKUP($B3,'Emp List'!$A$1:$I$38,4,FALSE)
```
