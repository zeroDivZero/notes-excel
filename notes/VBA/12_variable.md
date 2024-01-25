# VARIABLE

```vba
Public Sub FunWithVariables()
    Dim userName As String
    Dim userAge As Integer

    userName = "John"
    userAge = 100

    MsgBox ("Hello " & userName & "! You are " & userAge & " years old.")
    MsgBox (userName & ", you were born in " & Year(Now()) - userAge & ".")
    MsgBox (userName & ", in 10 years you will be " & userAge + 10 & ".")
End Sub
```

`Dim` stands for *dimension*.
