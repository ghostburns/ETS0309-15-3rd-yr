# Python String Methods

## Overview

Python provides built-in string methods for manipulating text including case conversion, substring search, and prefix/suffix verification. Common methods for changing text case include:

- str.lower(): Converts all characters to lowercase.
- str.upper(): Converts all characters to uppercase.
- str.title(): Capitalizes the first letter of each word.
- str.capitalize(): Capitalizes only the first character.
- str.swapcase(): Swaps the case of all letters.
- str.find(): Returns the index of the first occurrence of a substring.
- str.index(): Returns the index of the first occurrence; raises an error if not found.
- str.startswith(): Checks if the string begins with a specified prefix.
- str.endswith(): Checks if the string ends with a specified suffix.
- str.count(): Returns the count of non-overlapping occurrences of a substring.
- str.replace(): Returns a copy of the string with occurrences of a substring replaced.
- str.strip(): Returns a copy of the string with leading and trailing whitespace removed.
- str.lstrip(): Returns a copy of the string with leading whitespace removed.
- str.rstrip(): Returns a copy of the string with trailing whitespace removed.
- str.split(): Splits the string into a list of substrings.
- str.join(): Joins an iterable of strings using the string as a separator.
- str.isalpha(): Returns True if all characters in the string are alphabetic.
- str.isdigit(): Returns True if all characters in the string are digits.
- f-strings: Concise syntax for embedding expressions inside string literals.
- len(): Returns the number of items in an object.
- str.encode(): Converts a string into bytes using the specified encoding.

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

### str.index()

Description:
The str.index() method works like find(), but raises a ValueError if the substring is not found.

Syntax:

```python
string.index(substring, start, end)
```

- substring: The text to search for.
- start (optional): The starting index.
- end (optional): The ending index.

Example:

```python
text = "Hello, World!"
index = text.index("World")
print(index)  # Output: 7
```

### str.startswith()

Description:
The str.startswith() method checks if a string starts with a specified prefix. It returns True if it does; otherwise, it returns False.

Syntax:

```python
string.startswith(prefix, start, end)
```

- prefix: The string to check.
- start (optional): The starting index.
- end (optional): The ending index.

Example:

```python
text = "Hello, World!"
result = text.startswith("Hello")
print(result)  # Output: True
```

### str.endswith()

Description:
The str.endswith() method checks if a string ends with a specified suffix. It returns True if it does; otherwise, it returns False.

Syntax:

```python
string.endswith(suffix, start, end)
```

- suffix: The string to check.
- start (optional): The starting index.
- end (optional): The ending index.

Example:

```python
text = "Hello, World!"
result = text.endswith("World!")
print(result)  # Output: True
```

### str.count()

Description:
The str.count() method returns the number of non-overlapping occurrences of a substring in a string.

Syntax:

```python
string.count(sub, start, end)
```

- sub: The substring to search for.
- start (optional): The starting index.
- end (optional): The ending index.

Example:

```python
text = "apple, banana, apple"
count = text.count("apple")
print(count)  # Output: 2
```

### str.replace()

Description:
The str.replace() method returns a copy of the string with all occurrences of a specified substring replaced with another substring.

Syntax:

```python
string.replace(old, new, count)
```

- old: The substring to be replaced.
- new: The substring to replace with.
- count (optional): Maximum number of replacements.

Example:

```python
text = "Hello, World!"
replaced_text = text.replace("World", "Python")
print(replaced_text)  # Output: "Hello, Python!"
```

### str.strip()

Description:
The str.strip() method returns a copy of the string with leading and trailing whitespace removed.

Syntax:

```python
string.strip([chars])
```

- chars (optional): A string specifying the set of characters to be removed. If omitted, whitespace is removed.

Example:

```python
text = "  Hello, World!  "
stripped_text = text.strip()
print(stripped_text)  # Output: "Hello, World!"
```

### str.lstrip()

Description:
The str.lstrip() method returns a copy of the string with leading whitespace (or specified characters) removed.

Syntax:

```python
string.lstrip([chars])
```

Example:

```python
text = "   Hello, World!"
lstripped_text = text.lstrip()
print(lstripped_text)  # Output: "Hello, World!"
```

### str.rstrip()

Description:
The str.rstrip() method returns a copy of the string with trailing whitespace (or specified characters) removed.

Syntax:

```python
string.rstrip([chars])
```

Example:

```python
text = "Hello, World!   "
rstripped_text = text.rstrip()
print(rstripped_text)  # Output: "Hello, World!"
```

### str.split()

Description:
The str.split() method splits a string into a list of substrings using a specified separator. By default, it splits on any whitespace.

Syntax:

```python
string.split(sep=None, maxsplit=-1)
```

Example:

```python
text = "Hello, World, Python"
split_text = text.split(",")
print(split_text)  # Output: ["Hello", " World", " Python"]
```

### str.join()

Description:
Joins the elements of an iterable into a single string, with the string acting as the separator.

Syntax:

```python
separator.join(iterable)
```

Example:

```python
words = ["Hello", "World"]
sentence = " ".join(words)
print(sentence)  # Output: "Hello World"
```

### str.isalpha()

Description:
Checks whether all characters in the string are alphabetical. Returns True if yes, False otherwise.

Syntax:

```python
string.isalpha()
```

Example:

```python
text = "HelloWorld"
print(text.isalpha())  # Output: True
```

### str.isdigit()

Description:
Checks whether all characters in the string are digits. Returns True if yes, False otherwise.

Syntax:

```python
string.isdigit()
```

Example:

```python
num = "12345"
print(num.isdigit())  # Output: True
```

// Additional Methods and Concepts

### f-strings

Description: f-strings provide a concise way to embed expressions inside string literals.

Syntax:

```python
name = "Guru"
greeting = f"Hello, {name}"
```

Example:

```python
name = "Guru"
print(f"Hello, {name}!")  # Output: "Hello, Guru!"
```

### len()

Description: The len() function returns the number of items in an object. For strings, it returns the number of characters.

Syntax:

```python
len(string)
```

Example:

```python
text = "Hello, World!"
print(len(text))  # Output: 13
```

### str.encode()

Description: The str.encode() method converts the string into bytes using the specified encoding.

Syntax:

```python
string.encode(encoding="utf-8", errors="strict")
```

Example:

```python
text = "Hello, World!"
encoded_text = text.encode("utf-8")
print(encoded_text)  # Output: b"Hello, World!"
```

## Summary

| **Method**     | **Description**                                               | **Example Output** |
| -------------- | ------------------------------------------------------------- | ------------------ |
| `lower()`      | Converts all letters to lowercase                             | "hello, world!"    |
| `upper()`      | Converts all letters to uppercase                             | "HELLO, WORLD!"    |
| `title()`      | Capitalizes the first letter of each word                     | "Hello, World!"    |
| `capitalize()` | Capitalizes only the first character, rest lowercase          | "Hello, world!"    |
| `swapcase()`   | Swaps the case of all letters                                 | "hELLO, wORLD!"    |
| `find()`       | Returns the index of the first occurrence of substring        | 7                  |
| `index()`      | Returns the index of the first occurrence; error if not found | 7                  |
| `startswith()` | Checks if the string starts with the specified prefix         | True               |
| `endswith()`   | Checks if the string ends with the specified suffix           | True               |
| `count()`      | Counts the occurrences of a substring                         | 2                  |
| `replace()`    | Replaces occurrences of a substring                           | "Hello, Python!"   |
| `strip()`      | Removes leading and trailing whitespace                       | "Hello, World!"    |
| `lstrip()`     | Removes leading whitespace or characters                      | "Hello, World!"    |
| `rstrip()`     | Removes trailing whitespace or characters                     | "Hello, World!"    |
| `split()`      | Splits the string into a list by a separator                  | ["Hello", "World"] |
| `join()`       | Joins an iterable of strings using the string as a separator  | "Hello World"      |
| `isalpha()`    | Returns True if all characters are alphabetic                 | True               |
| `isdigit()`    | Returns True if all characters are digits                     | True               |
| `f-strings`    | Embeds expressions within string literals                     | "Hello, Guru!"     |
| `len()`        | Returns the number of characters in a string                  | 13                 |
| `str.encode()` | Converts a string into bytes                                  | b"Hello, World!"   |

## Use Cases

- **`lower()`**: Useful when performing case-insensitive comparisons.
- **`upper()`**: Commonly used for formatting user input or emphasizing text.
- **`title()`**: Helpful for formatting titles and names in a readable manner.
- **`capitalize()`**: Standardizes strings by capitalizing the first letter.
- **`swapcase()`**: Handy for toggling letter cases.
- **`find()`**: Valuable for locating substrings efficiently.
- **`index()`**: Useful when an error should be raised if a substring is absent.
- **`startswith()`**: Ideal for verifying the beginning of strings.
- **`endswith()`**: Ideal for verifying the ending of strings.
- **`count()`**: Useful for counting occurrences of a substring.
- **`replace()`**: Handy for replacing parts of a string.
- **`strip()`**: Useful for cleaning up strings by removing unwanted whitespace.
- **`lstrip()`**: Useful for removing leading whitespace or characters.
- **`rstrip()`**: Useful for removing trailing whitespace or characters.
- **`split()`**: Useful for splitting a string into a list of substrings.
- **`join()`**: Useful for joining elements of an iterable into a single string.
- **`isalpha()`**: Useful for checking if all characters in a string are alphabetic.
- **`isdigit()`**: Useful for checking if all characters in a string are digits.
- **`f-strings`**: Useful for embedding expressions inside string literals efficiently.
- **`len()`**: Useful for determining the length of a string or iterable.
- **`str.encode()`**: Useful for converting strings into bytes, especially for encoding data.
