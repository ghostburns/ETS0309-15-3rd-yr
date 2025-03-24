# Python String Methods: str.lower(), str.upper(), and str.title()

## Overview

Python provides built-in string methods that allow for easy manipulation of text. Three common methods for changing the case of a string are:

str.lower(): Converts all characters in a string to lowercase.

str.upper(): Converts all characters in a string to uppercase.

str.title(): Capitalizes the first letter of each word in a string.

## Method Explanations and Examples

### str.lower()

Description:

The str.lower() method converts all uppercase letters in a string to lowercase. It does not modify numbers, punctuation, or already lowercase characters.

Syntax:

```python
string.lower()
```

Example:

```python
text = "Hello, WORLD!"
lower_text = text.lower()
print(lower_text)  # Output: "hello, world!"
```

### str.upper()

Description:

The str.upper() method converts all lowercase letters in a string to uppercase. Like lower(), it does not affect numbers or punctuation.

Syntax:

```python
string.upper()
```

Example:

```python
text = "Hello, world!"
upper_text = text.upper()
print(upper_text)  # Output: "HELLO, WORLD!"
```

### str.title()

Description:

The str.title() method capitalizes the first letter of each word in a string while converting all other letters to lowercase.

Syntax:

```python
string.title()
```

Example:

```python
text = "hello, world!"
title_text = text.title()
print(title_text)  # Output: "Hello, World!"
```

### str.capitalize()

Description:
The str.capitalize() method capitalizes only the first character of the string and converts the rest to lowercase.

Syntax:
```python
string.capitalize()
```

Example:
```python
text = "hello, WORLD!"
capitalized_text = text.capitalize()
print(capitalized_text)  # Output: "Hello, world!"
```

### str.swapcase()

Description:
The str.swapcase() method swaps the case of all letters in the string, converting uppercase-to-lowercase and vice versa.

Syntax:
```python
string.swapcase()
```

Example:
```python
text = "Hello, World!"
swapped_text = text.swapcase()
print(swapped_text)  # Output: "hELLO, wORLD!"
```

### str.find()

Description:
The str.find() method searches for a specified substring and returns the index of its first occurrence. If the substring is not found, it returns -1.

Syntax:
```python
string.find(substring, start, end)
```
- substring: The text to search for.
- start (optional): The starting index.
- end (optional): The ending index.

Example:
```python
text = "Hello, World!"
index = text.find("World")
print(index)  # Output: 7
```

## Summary
 
| **Method**     | **Description**                                        | **Example Output**    |
|----------------|--------------------------------------------------------|-----------------------|
| `lower()`      | Converts all letters to lowercase                      | `"hello, world!"`     |
| `upper()`      | Converts all letters to uppercase                      | `"HELLO, WORLD!"`     |
| `title()`      | Capitalizes the first letter of each word              | `"Hello, World!"`     |
| `capitalize()` | Capitalizes only the first character, rest lowercase   | `"Hello, world!"`     |
| `swapcase()`   | Swaps the case of all letters                          | `"hELLO, wORLD!"`     |
| `find()`       | Returns the index of the first occurrence of substring | 7                     |

## Use Cases

- **`lower()`**: Useful when performing case-insensitive comparisons.
- **`upper()`**: Commonly used for formatting user input or making text stand out.
- **`title()`**: Helpful for formatting titles and names in a readable manner.
- **`capitalize()`**: Standardizes strings by capitalizing the first letter.
- **`swapcase()`**: Handy for toggling letter cases.
- **`find()`**: Valuable for locating substrings efficiently.
