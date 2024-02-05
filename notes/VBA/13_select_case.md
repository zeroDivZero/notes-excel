# `Select Case`

Similar to `If ElseIf Else`, but more performant and terse.

```vba
Select Case ActiveCell.Value
  Case Is > 90
      MsgBox (">90")
  Case 21 To 90
      MsgBox (">=21")
  Case Else
      MsgBox ("Not allowed!")
End Select
```
