# `HLOOKUP()`

Horizontal lookup. Like `VLOOKUP()`, but Looks for val in topmost row of table, returns val in same col from row specified.

Same params as `VLOOKUP()` but cols and rows swapped. See [VLOOKUP](VLOOKUP.md) for details.

## Example

```excel
=HLOOKUP($B$3,'Master Inventory List'!$A$2:$G$5,3,FALSE)
```

## Dynamic Row Lookup

Above example specifies static row, cannot drag formula to auto-fill other cells. Combine with other lookup functions like `MATCH()` to make it more dynamic:

```excel
=HLOOKUP($B$3,'Master Inventory List'!$A$2:$G$5,MATCH(LEFT($A5,11),'Master Inventory List'!$A$2:$A$5,0),FALSE)
```
