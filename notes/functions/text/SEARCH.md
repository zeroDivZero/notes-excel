# `SEARCH()`

Char num at which specified str 1st found, reading left to right. **Case-insensitive**.

## Syntax

```excel
SEARCH(find_text,within_text,start_num)
```

*	`find_text`: Text to find. Can use wildcards `?` and `*`; use `~?` and `~*` to find `?` and `*`.
* `within_text`: Text in which to search for `find_text`.
*	`start_num`: Char num in `within_text`, counting from left, at which to start searching. 1 if omitted.

## Example

Extracting first name from str where first and last names separated by space:

```excel
=LEFT(A2,SEARCH(" ",A2)-1)
```
