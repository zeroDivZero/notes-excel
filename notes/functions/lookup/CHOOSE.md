# `CHOOSE()`

Selects one of up to 254 values based on `index_num`.

## Syntax

```excel
CHOOSE(index_num, value1, [value2], ...)
```

## Examples

If `B2` is 4, evaluates to **"Green"**:

```excel
=CHOOSE(B2,"Red","White","Blue","Green","Black")
```

Value arguments can be range refs. Following sums `B1:B10`:

```excel
=SUM(CHOOSE(2,A1:A10,B1:B10,C1:C10))
```
