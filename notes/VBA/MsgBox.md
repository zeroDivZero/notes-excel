# `MsgBox`

Displays message in dialog box, waits for user to click button, and returns Integer indicating which button was clicked.

## Displays Info Only

```vba
MsgBox (ActiveSheet.Range("A1").Value)
```

## Yes/No

Needs to store user input.

```vba
Dim tryAgain As Integer
tryAgain = MsgBox("Invalid value. Try again?", vbYesNo)
If tryAgain = 6 Then  'yes
    'do something
End If
```
