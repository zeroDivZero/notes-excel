# `SUBTOTAL()`

Subtotal of list, taking filtering into account.

Syntax:

```excel
SUBTOTAL(function_num,ref1,...)
```

**function_num** specifies summary function for subtotal. **ref1,ref2,...** are references in subtotal.

Ex:

```excel
=SUBTOTAL(9,F4:F61)
```

Above example specifies `SUM()` as function, so it calculates subtotal like `DSUM()`. Unlike `DSUM()`, doesn't need criteria.
