# Python List Methods

## Overview
This document covers common list methods:
- list.append(): Adds an element at the end.
- list.insert(): Inserts an element at a given position.
- list.remove(): Removes the first occurrence of a value.

## Method Explanations and Examples

### list.append()
Description:
Adds an element to the end of the list.

Syntax:
```python
lst.append(element)
```
Example:
```python
lst = [1, 2, 3]
lst.append(4)
print(lst)  # Output: [1, 2, 3, 4]
```

### list.insert()
Description:
Inserts an element at a specified index.

Syntax:
```python
lst.insert(index, element)
```
Example:
```python
lst = [1, 3, 4]
lst.insert(1, 2)
print(lst)  # Output: [1, 2, 3, 4]
```

### list.remove()
Description:
Removes the first occurrence of a value.

Syntax:
```python
lst.remove(element)
```
Example:
```python
lst = [1, 2, 3, 2]
lst.remove(2)
print(lst)  # Output: [1, 3, 2]
```

## Summary

| **Method**    | **Description**                             | **Example Output**   |
| ------------- | ------------------------------------------- | -------------------- |
| `append()`    | Adds an element at the end                  | [1, 2, 3, 4]         |
| `insert()`    | Inserts an element at a specific index      | [1, 2, 3, 4]         |
| `remove()`    | Deletes the first occurrence of a value     | [1, 3, 2]            |

## Use Cases
- `append()`: Dynamically add elements to the end when processing sequences.
- `insert()`: Insert an element at a specific index to maintain order.
- `remove()`: Remove the first occurrence of a value to eliminate unwanted items.