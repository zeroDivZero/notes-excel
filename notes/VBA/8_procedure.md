# PROCEDURE

To create, ensure to click in module edit area, then **Insert &rarr; Procedure**.

![Add Procedure](/assets/vba/procedure-add.png)

Same naming rules as macro.

## Types

3 types.

### Sub

Code executed line by line, top to bottom. Once last line executed, sub-procedure is complete.

### Function

When code execution completes, returns value. Excel has many built-in functions.

### Property

To create custom objects and properties.

## Scope

Where procedure's available. **Public** means anywhere in this Excel project. **Private** means only available in this object (such as `Module1`).

## Example

```vba
Public Sub FunWithProcedures()
    ActiveSheet.Range("A1").Value = "Hello, world!"
End Sub
```

## Execute

Unlike code in **Immediate Window**, doesn't run immediately. Can run like macro (button, etc.), or use **Run** button in editor's toolbar.
