# `Range.Sort`

Sorts range (including columns) of values.

```vba
Public Sub CategorySort()
    'sorts list by Category
    Columns("A:F").Sort key1:=Range("B2"), order1:=xlAscending, Header:=xlYes
End Sub
```

Can add two additional keys and order types to further sort.
