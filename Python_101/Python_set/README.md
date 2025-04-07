# Python Set Methods

## Overview

This document covers common set methods:
- `add()`: Adds an element to the set.
- `remove()`: Removes a specified element from the set.
- `union()`: Combines all unique elements from two or more sets.

## Method Explanations and Examples

### add()

Description:
The `add()` method adds a single element to the set. If the element already exists, the set remains unchanged.

Syntax:
```python
set.add(element)
```

Example:
```python
s = {1, 2, 3}
s.add(4)
print(s)  # Output: {1, 2, 3, 4}
```

### remove()

Description:
The `remove()` method removes a specified element from the set. If the element does not exist, it raises a `KeyError`.

Syntax:
```python
set.remove(element)
```

Example:
```python
s = {1, 2, 3}
s.remove(2)
print(s)  # Output: {1, 3}
```

### union()

Description:
The `union()` method returns a new set containing all unique elements from two or more sets.

Syntax:
```python
set.union(*others)
```

Example:
```python
s1 = {1, 2, 3}
s2 = {3, 4, 5}
result = s1.union(s2)
print(result)  # Output: {1, 2, 3, 4, 5}
```

## Summary

| **Method** | **Description**                             | **Example Output**   |
| ---------- | ------------------------------------------- | -------------------- |
| `add()`    | Adds an element to the set                  | {1, 2, 3, 4}         |
| `remove()` | Removes a specified element from the set    | {1, 3}               |
| `union()`  | Combines all unique elements from two sets  | {1, 2, 3, 4, 5}      |

## Use Cases

- **`add()`**: Dynamically add elements to a set.
- **`remove()`**: Remove unwanted elements from a set.
- **`union()`**: Combine multiple sets into one.