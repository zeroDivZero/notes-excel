# `SUBTOTAL()`

Subtotal of list, taking filtering into account.

Syntax:

```excel
SUBTOTAL(function_num,ref1,...)
```

**function_num** specifies summary function for subtotal. Each function has unique number, see doc. **ref1,ref2,...** are cells participating in subtotal.

Ex:

```excel
=SUBTOTAL(9,F4:F61)
```

Above example specifies `SUM()` as function, so it calculates subtotal like `DSUM()`. Unlike `DSUM()`, doesn't need criteria.
