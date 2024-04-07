# `TEXT`

Changes way number appears by applying formatting with format code. Useful to display number in more readable format, or to combine number with text or symbol.

## Format

```excel
=TEXT(value to format, "format code")
```

## Examples

### Currency

```excel
=TEXT(1234.567, "$#,##0.00")
```

Returns text `$1,234.57`. With thousands separator and 2 decimals. Rounds decimal places.

### Date and Time

```excel
=TEXT(TODAY(), "MM/DD/YY")
```

Today's date, such as `04/15/24`.

```excel
=TEXT(TODAY(), "DDDD")
```

Today's day of week, like `Monday`. `MMMM` for month.

```excel
=TEXT(NOW(), "H:MM AM/PM")
```

Current time, like `1:29 PM`.

### Others

Percentage, fraction, scientific notation, phone number, padding 0s, latitude and longitude, etc.
