# RANGE SELECT

```vba
Range("A3").Select
```

After this, `ActiveCell` refers to currently selected cell.

If selected section:

```vba
Range("A3:F3").Select
```

`Selection` refers to active selection.

## Contiguous Content

From current selection to end of contiguous content (no empty cell) in one of 4 directions (`xlUp`, `xlDown`, `xlRight`, `xlLeft`):

```vba
Range(Selection, Selection.End(xlDown)).Select
```
