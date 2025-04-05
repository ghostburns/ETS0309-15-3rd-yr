# Python List Methods

## Overview
This document covers common list methods:
- list.append(): Adds an element at the end.
- list.insert(): Inserts an element at a given position.
- list.remove(): Removes the first occurrence of a value.
- list.pop(): Removes and returns the last element.
- len(): Returns the number of elements in the list.
- list.sort(): Sorts the list in ascending order.
- Slicing: Extracts a portion of the list.

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

### list.pop()
Description:
Removes and returns the last element of the list. If an index is specified, it removes and returns the element at that index.

Syntax:
```python
lst.pop([index])
```
Example:
```python
lst = [1, 2, 3]
last_element = lst.pop()
print(last_element)  # Output: 3
print(lst)  # Output: [1, 2]
```

### len()
Description:
Returns the number of elements in the list.

Syntax:
```python
len(lst)
```
Example:
```python
lst = [1, 2, 3]
print(len(lst))  # Output: 3
```

### list.sort()
Description:
Sorts the list in ascending order. By default, it modifies the list in place.

Syntax:
```python
lst.sort()
```
Example:
```python
lst = [3, 1, 2]
lst.sort()
print(lst)  # Output: [1, 2, 3]
```

### Slicing
Description:
Extracts a portion of the list using slicing syntax.

Syntax:
```python
lst[start:end:step]
```
Example:
```python
lst = [1, 2, 3, 4, 5]
print(lst[1:4])  # Output: [2, 3, 4]
print(lst[:3])   # Output: [1, 2, 3]
print(lst[::2])  # Output: [1, 3, 5]
```

## Summary

| **Method**    | **Description**                             | **Example Output**   |
| ------------- | ------------------------------------------- | -------------------- |
| `append()`    | Adds an element at the end                  | [1, 2, 3, 4]         |
| `insert()`    | Inserts an element at a specific index      | [1, 2, 3, 4]         |
| `remove()`    | Deletes the first occurrence of a value     | [1, 3, 2]            |
| `pop()`       | Removes and returns the last element        | [1, 2]               |
| `len()`       | Returns the number of elements in the list  | 3                    |
| `sort()`      | Sorts the list in ascending order           | [1, 2, 3]            |
| `slicing`     | Extracts a portion of the list              | [2, 3, 4]            |

## Use Cases
- `append()`: Dynamically add elements to the end when processing sequences.
- `insert()`: Insert an element at a specific index to maintain order.
- `remove()`: Remove the first occurrence of a value to eliminate unwanted items.
- `pop()`: Retrieve and remove elements dynamically.
- `len()`: Determine the size of a list for iteration or validation.
- `sort()`: Organize elements in ascending order for easier processing.
- `slicing`: Extract specific portions of a list for further operations.