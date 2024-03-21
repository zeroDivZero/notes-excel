# `Worksheets`

`Worksheets` collection contains all `Worksheet` objects in workbook.

Similarly, `Sheets` collection contains `Chart` and `Worksheet` objects in workbook.

```vba
'loop through all worksheets
Dim ws As Worksheet
For Each ws In Worksheets
    ws.Select
    'do something with ActiveSheet
Next ws
```

```vba
'get worksheet of name
Worksheets("MySheet").Select

'refer to name of worksheet
count = Worksheets(ws.Name).Cells.Count
```
