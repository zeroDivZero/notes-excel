# `HLOOKUP()`

Horizontal lookup. Like `VLOOKUP()`, but Looks for val in topmost row of table, returns val in same col from row specified.

Same params as `VLOOKUP` but cols and rows swapped. See [VLOOKUP](VLOOKUP.md) for details.

## Example

```excel
=HLOOKUP($B$3,'Master Inventory List'!$A$2:$G$5,3,FALSE)
```
