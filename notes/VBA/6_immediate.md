# IMMEDIATE

In Visual Basic Editor, **View &rarr; Immediate Window** to make Immediate Window visible.

Can enter code to be executed immediately.

![Immediate Window](/assets/vba/immediate-window.png)

To display current value, add `?` in front of code.

`ActiveWorkbook` implied, don't need to specify it every time.

Assign value to cell:

```vba
ActiveSheet.Range("A2").Value = "Hello, world!"
```
