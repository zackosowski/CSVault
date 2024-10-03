*[[Video Game Design (VGD)]] students may be looking for [[Lists (C-Sharp)]]*

A list is a versatile, ordered collection of items that can hold elements of different types. Lists are mutable, meaning you can modify them after creation by adding, removing, or changing elements.

Python lists are a powerful and flexible data structure, making them essential for managing collections of items in various programming scenarios. Their simplicity and functionality contribute to their widespread use in Python programming.

----
#### Using Lists

Lists maintain the order of elements, allowing you to access items by their position (index).

```python
my_list = [1, 2, 3, 'four', 5.0]
```

You can change the contents of a list without creating a new one. This includes adding or removing elements.

```python
fruits = ['apple', 'banana', 'cherry'] 
fruits.append('date') # Adds 'date' 
fruits.remove('banana') # Removes 'banana'
print(fruits) # Output: ['apple', 'cherry', 'date']
```

Lists can contain items of different data types, such as integers, strings, and other lists.

```python
mixed_list = [1, 'hello', 3.14, [1, 2, 3]]
```

You can access individual elements or slices of the list using indexing.

```python
first_item = my_list[0]  # Accesses the first element
sub_list = my_list[1:3]   # Gets elements from index 1 to 2
```