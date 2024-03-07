# `InputBox()`

Displays dialog box prompt, waits for user to input text or click button, and returns `String` containing text box content.

```vba
Dim userColor As String
userColor = InputBox("What is your favorite color?", "Favorite Color")
```

## Error Handling

By default expects return value. If user hits OK or cancel button without input, error.

Also, may be convenient to auto-cast input type:

```vba
Dim userAge As Integer
userAge = InputBox("How old are you?", "Age")
```

But if user enters anything that doesn't cast to `Integer`, error.

To handle error, need to specify error handler:

```vba
Public Sub UserAgeInput()
    Dim userAge As Integer

    On Error GoTo errorHandler

    userAge = InputBox("How old are you?", "Age")

    If userAge <= 200 Then
        MsgBox (userAge)
    Else
errorHandler:
        tryAgain = MsgBox("Invalid value. Try again?", vbYesNo)
        If tryAgain = 6 Then  'yes
            UserAgeInput
        End If
    End If
End Sub
```

If need error handler at end of function:

```vba
Done:
    Exit Sub
errorHandler:
    'error handling
```
