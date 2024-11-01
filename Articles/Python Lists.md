#article

A Python *list* is a type of data that allows the storage of multiple items in a single variable. Lists in Python are ordered, mutable (can be changed after creation), and allow duplicate elements. Lists are one of the most commonly used data types in Python due to their versatility in handling collections of items.

---
### Key Characteristics of Python Lists

- **Ordered**: Items in a list maintain the order in which they were added. This order can be modified but is consistent unless changed.
- **Mutable**: Lists can be modified after they are created. This includes adding, removing, or changing elements.
- **Heterogeneous**: Lists can contain elements of different data types. For example, a list can contain integers, strings, or even other lists.
- **Indexed**: Each element in a list has an index, starting from 0 for the first element. This makes it easy to access individual elements by their position.

---
### Creating a List

A list is created by placing items inside square brackets `[]`, separated by commas. Lists can be created with any number of items, including zero.

```python
# Creating a simple list
fruits = ["apple", "banana", "cherry"]

# An empty list
empty_list = []
```

---
### Accessing List Items

To access an item from a list, use its index within square brackets. The first item has an index of 0, the second an index of 1, and so on. Negative indexing is also allowed, where `-1` refers to the last item, `-2` to the second last, etc.

```python
# Accessing the first item
print(fruits[0])  # Output: "apple"

# Accessing the last item using negative indexing
print(fruits[-1])  # Output: "cherry"
```

---
#### Modifying Lists

Since lists are mutable, you can modify their elements after creation. This includes changing an existing item, adding new items, or removing items.

###### Adding Items

- **`append()`**: Adds an item to the end of the list.
- **`insert()`**: Adds an item at a specified index.
- **`extend()`**: Adds multiple items (from another list or iterable) to the end of the list.

```python
# Adding items to the list
fruits.append("orange")      # ["apple", "banana", "cherry", "orange"]
fruits.insert(1, "grape")    # ["apple", "grape", "banana", "cherry", "orange"]
```

###### Removing Items

- **`remove()`**: Removes the first occurrence of a specified item.
- **`pop()`**: Removes an item by its index and returns it. If no index is specified, it removes the last item.
- **`clear()`**: Removes all items from the list, making it empty.

```python
# Removing items from the list
fruits.remove("banana")  # Removes "banana" from the list
fruits.pop(2)            # Removes the item at index 2 ("cherry" in this case)
```

---
#### Iterating Over Lists

Lists can be looped through using `for` or `while` loops. This allows you to process each item in a list individually.

```python
# Using a for loop to print each item
for fruit in fruits:
    print(fruit)
```

---
#### Common List Functions

| Method           | Description                                                           |
|------------------|-----------------------------------------------------------------------|
| `append(x)`      | Adds an item `x` to the end of the list.                              |
| `insert(i, x)`   | Inserts an item `x` at index `i`.                                     |
| `remove(x)`      | Removes the first occurrence of the item `x`.                         |
| `pop([i])`       | Removes and returns the item at index `i`; removes the last item if `i` is not specified. |
| `clear()`        | Removes all items from the list.                                      |
| `index(x)`       | Returns the index of the first occurrence of item `x`.                |
| `count(x)`       | Returns the count of item `x` in the list.                            |
| `sort()`         | Sorts the list in ascending order.                                    |
| `reverse()`      | Reverses the items in the list.                                       |
| `extend(iterable)` | Adds items from another iterable to the end of the list.             |

---
### List Comprehensions

List comprehensions provide a concise way to create lists by generating and processing items in a single line of code. They often replace traditional `for` loops to create new lists based on some criteria or transformation.

```python
# List comprehension to create a list of squares of numbers
squares = [x**2 for x in range(10)]  # Output: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```
