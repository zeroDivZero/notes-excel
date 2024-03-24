# `Range.End` property

`Range` representing cell at end of region containing source range.

```vba
'select cell at end of row 2 in region containing A2
Range("A2").End(xlToRight).Select
```

```vba
'select column starting from active cell
Range(ActiveCell, ActiveCell.End(xlDown)).Select
```
