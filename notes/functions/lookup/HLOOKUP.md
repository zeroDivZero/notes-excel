# `HLOOKUP()`

Horizontal lookup. Very similar to `VLOOKUP()`, but Looks for value in topmost row of table, returns value in same column from row specified.

Same params as VLOOKUP but swap columns and rows. See [VLOOKUP](VLOOKUP.md) for details.

## Example

```excel
=HLOOKUP($B$3,'Master Inventory List'!$A$2:$G$5,3,FALSE)
```
