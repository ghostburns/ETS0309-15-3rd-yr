# Python Dictionary Methods

## Overview

This document covers common dictionary methods:
- `keys()`: Returns a view object containing the dictionary's keys.
- `values()`: Returns a view object containing the dictionary's values.
- `get()`: Returns the value for a specified key, or a default value if the key is not found.
- `pop()`: Removes a key and returns its value.
- `items()`: Returns a view object of key-value pairs.

## Method Explanations and Examples

### keys()
The `keys()` method returns a view object that displays a list of all the keys in the dictionary.

Syntax:
```python
dictionary.keys()
```

Example:
```python
my_dict = {"a": 1, "b": 2, "c": 3}
keys = my_dict.keys()
print(keys)  # Output: dict_keys(['a', 'b', 'c'])
```

### values()

Description:
The `values()` method returns a view object that displays a list of all the values in the dictionary.

Syntax:
```python
dictionary.values()
```

Example:
```python
my_dict = {"a": 1, "b": 2, "c": 3}
values = my_dict.values()
print(values)  # Output: dict_values([1, 2, 3])
```

### get()

Description:
The `get()` method returns the value for a specified key. If the key does not exist, it returns a default value (or `None` if no default is provided).

Syntax:
```python
dictionary.get(key, default)
```

- `key`: The key to search for.
- `default` (optional): The value to return if the key is not found.

Example:
```python
my_dict = {"a": 1, "b": 2, "c": 3}
value = my_dict.get("b")
print(value)  # Output: 2

default_value = my_dict.get("d", "Not Found")
print(default_value)  # Output: "Not Found"
```

### pop()

Description:
The `pop()` method removes the specified key and returns the corresponding value. If the key is not found, it raises a `KeyError` unless a default value is provided.

Syntax:
```python
dictionary.pop(key, default)
```

- `key`: The key to remove.
- `default` (optional): The value to return if the key is not found.

Example:
```python
my_dict = {"a": 1, "b": 2, "c": 3}
value = my_dict.pop("b")
print(value)  # Output: 2
print(my_dict)  # Output: {"a": 1, "c": 3}

default_value = my_dict.pop("d", "Not Found")
print(default_value)  # Output: "Not Found"
```

### items()

Description:
The `items()` method returns a view object that displays a list of dictionary's key-value tuple pairs.

Syntax:
```python
dictionary.items()
```

Example:
```python
my_dict = {"a": 1, "b": 2, "c": 3}
items = my_dict.items()
print(items)  # Output: dict_items([('a', 1), ('b', 2), ('c', 3)])
```

## Summary

| **Method** | **Description**                                   | **Example Output**                     |
| ---------- | ------------------------------------------------- | -------------------------------------- |
| `keys()`   | Returns a view object of the dictionary's keys    | dict_keys(['a', 'b', 'c'])             |
| `values()` | Returns a view object of the dictionary's values  | dict_values([1, 2, 3])                 |
| `get()`    | Returns the value for a key or a default value    | 2                                      |
| `pop()`    | Removes a key and returns its value               | 2                                      |
| `items()`  | Returns a view object of key-value pairs          | dict_items([('a', 1), ('b', 2), ('c', 3)])

## Use Cases

- **`keys()`**: Useful for iterating over all keys in a dictionary.
- **`values()`**: Useful for accessing all values in a dictionary.
- **`get()`**: Useful for safely retrieving a value without raising a `KeyError`.
- **`pop()`**: Useful for removing a key-value pair and getting its value.
- **`items()`**: Useful for iterating over key-value pairs in a dictionary.