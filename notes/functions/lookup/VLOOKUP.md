# `VLOOKUP()`

Vertical lookup. Looks for value in leftmost column of table, returns value in same row from column specified. By default, table must be sorted in ascending order.

```excel
VLOOKUP(lookup_value,table_array,col_index_num,range_lookup)
```

* **Lookup_value**: value to be found in first column of table; can be value, reference, or text string.
* **Table_array**: table of text, numbers, or logical values, in which data is retrieved. Can be reference to a range or range name.
* **Col_index_num**: column number in table_array from which matching value should be returned. First column is 1.
* **Range_lookup**: logical value, to find closest match in first column (sorted in ascending order) = `TRUE` or omitted; find exact match = `FALSE`.

## Example

```excel
=VLOOKUP($B3,'Emp List'!$A$1:$I$38,4,FALSE)
```
