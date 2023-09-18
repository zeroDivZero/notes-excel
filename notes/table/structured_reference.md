# STRUCTURED REFERENCE

When creating table, Excel assigns names to table and columns. Formulas can use those names instead of cell refs. Example:

| Explicit cell refs | Table and column names          |
| ------------------ | ------------------------------- |
| `=SUM(C2:C7)`      | `=SUM(DeptSales[Sales Amount])` |

## Special Item Identifiers

`#All`: Entire table, including column headers, data, and totals (if any).

`#Data`: Only data rows.

`#Headers`: Only header row.

`#Totals`: Only total row. If none exists, returns null.
