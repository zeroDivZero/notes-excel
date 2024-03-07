# `vbCrLf`

Carriage return linefeed. Equivalent to pressing enter key (next line).

```vba
Dim sortOrder As Integer
Dim promptMsg As String

promptMsg = "How would you like to sort the list?" & vbCrLf & _
"1 - Sort by Division" & vbCrLf & _
"2 - Sort by Category" & vbCrLf & _
"3 - Sort by Total"

sortOrder = InputBox(promptMsg, "Sort Order")
```

Above code displays each line of text on new line in input box. `_` is to type long string on multiple lines.
