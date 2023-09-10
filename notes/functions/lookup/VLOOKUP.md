# `VLOOKUP()`

Vertical lookup. Looks for value in table's leftmost column, returns value in same row at specified column. By default, table must be sorted in ascending order.

```excel
VLOOKUP(lookup_value,table_array,col_index_num,range_lookup)
```

* **lookup_value**: Value to be found in 1st column of table. Can be value, ref, or text.
* **table_array**: Table of text, numbers, or logical values, in which data is retrieved; can be range ref or name.
* **col_index_num**: Column number in **table_array** from which matching value should be returned. 1st column is 1.
* **range_lookup**: Logical value, to find closest match in 1st column (sorted in ascending order) = `TRUE` or omitted; find exact match = `FALSE`.

## Example

```excel
=VLOOKUP($B3,'Emp List'!$A$1:$I$38,4,FALSE)
```
