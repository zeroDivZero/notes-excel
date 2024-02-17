# `Do While`

```vba
Public Sub FunWithLoops()
    Do While ActiveCell.Value <> ""
        'do something with active cell
        ActiveCell.Offset(1, 0).Select
    Loop
End Sub
```
