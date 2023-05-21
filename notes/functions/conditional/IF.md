# `IF()`

If logical test passed, show one value, otherwise show other. To use, start typing `=IF(`, or under **Formulas**, open **Logical**:

![IF](/assets/IF.png)

Example:

```excel
=IF(F5>=$I$2,"YES","NO")
```

May rename absolute ref as named range for better context:

```excel
=IF(F5>=Goal,"YES","NO")
```
