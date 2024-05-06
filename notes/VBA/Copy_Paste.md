# `Copy`, `Paste`

For example, copy current selection and paste it to different worksheet:

```vba
Selection.Copy
Worksheets("Consolidated Report").Select
ActiveSheet.Paste
```
