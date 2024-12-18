#article

Dictionaries are an essential data structure in Python that allow you to store and manage data efficiently. Unlike [[Lists (Python)|lists]], which are ordered collections of items, dictionaries store data in key-value pairs. This means you can retrieve data quickly using a unique key instead of an index. Understanding how to use dictionaries will greatly enhance your programming skills and allow you to handle complex data in a more organized way.

---
#### What is a Dictionary?

A dictionary in Python is created using curly braces `{}` or the `dict()` function. Each key-value pair is separated by a colon `:`, and pairs are separated by commas. Keys in a dictionary must be unique and immutable (they can be strings, numbers, or tuples), while values can be of any data type and can be duplicated.

```python
# Example of a dictionary
my_dict = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}
```

In this example, the keys are `"name"`, `"age"`, and `"city"`, with their corresponding values being `"Alice"`, `25`, and `"New York"`.

---
#### Accessing Dictionary Values

You can access values in a dictionary by using their keys inside square brackets `[]` or with the `get()` method. Using square brackets will raise a `KeyError` if the key does not exist, while `get()` will return `None` or a specified default value.

```python
# Accessing values
print(my_dict["name"])  # Output: Alice
print(my_dict.get("age"))  # Output: 25
print(my_dict.get("country", "Not Found"))  # Output: Not Found
```

**Warning:** Always be cautious when accessing keys. If you try to access a key that does not exist using square brackets, your program will crash with a `KeyError`.

---
#### Adding and Modifying Entries

You can add new key-value pairs or modify existing ones by assigning a value to a key. If the key already exists, the value will be updated; if it does not, a new key-value pair will be created.

```python
# Adding a new entry
my_dict["country"] = "USA"

# Modifying an existing entry
my_dict["age"] = 26

print(my_dict)
```

---
#### Removing Entries

To remove a key-value pair from a dictionary, you can use the `del` statement or the `pop()` method. The `del` statement removes the item without returning it, while `pop()` returns the value of the removed key.

```python
# Removing an entry
del my_dict["city"]  # Removes the key "city"

age = my_dict.pop("age")  # Removes the key "age" and returns its value

print(my_dict)  # Output: {'name': 'Alice', 'country': 'USA'}
print(age)  # Output: 26
```

---
#### Looping Through a Dictionary

You can loop through dictionaries using loops. By default, iterating over a dictionary will give you the keys. You can use methods like `.items()` to get both keys and values.

```python
# Looping through keys
for key in my_dict:
    print(key)

# Looping through key-value pairs
for key, value in my_dict.items():
    print(f"{key}: {value}")
```

---
#### Common Dictionary Methods

Python dictionaries come with several built-in methods that make it easy to manipulate data. Here are a few commonly used methods:

- `my_dict.keys()` - Returns a view object displaying a list of all the keys.
- `my_dict.values()` - Returns a view object displaying a list of all the values.
- `my_dict.items()` - Returns a view object displaying a list of key-value tuple pairs.
- `my_dict.clear()` - Removes all items from the dictionary.

```python
# Example of using dictionary methods
keys = my_dict.keys()
values = my_dict.values()
items = my_dict.items()

print(keys)   # Output: dict_keys(['name', 'country'])
print(values) # Output: dict_values(['Alice', 'USA'])
print(items)  # Output: dict_items([('name', 'Alice'), ('country', 'USA')])
```

---
#### Practice Problems

1. **Create a Dictionary**  
   Write a program that creates a dictionary to store the names of five students and their corresponding grades. After creating the dictionary, print each student's name along with their grade.

   Example output:  
   ```
   Alice: A  
   Bob: B  
   Charlie: C  
   David: A  
   Eve: B  
   ```

2. **Accessing Values**  
   Given the following dictionary:  
   ```python
   student = {"name": "Alice", "age": 16, "grade": "A"}
   ```  
   Write a program that accesses and prints the student's name and age.

3. **Updating Values**  
   Extend the previous problem by writing a program that updates the student's grade to "A+" and then prints the updated dictionary.

4. **Adding New Key-Value Pairs**  
   Create a dictionary to store the names of three favorite movies and their release years. Write a program that allows the user to add a new movie and its release year to the dictionary, then print the updated dictionary.

5. **Removing Key-Value Pairs**  
   Write a program that creates a dictionary of five fruits and their prices. Allow the user to input the name of a fruit to remove it from the dictionary. After removal, print the updated dictionary.

6. **Looping Through a Dictionary**  
   Given the following dictionary:  
   ```python
   inventory = {"apples": 10, "bananas": 5, "oranges": 8}
   ```  
   Write a program that loops through the dictionary and prints each fruit along with its quantity in a formatted string.

7. **Counting Occurrences**  
   Write a program that takes a list of words and counts the occurrences of each word using a dictionary. Print the resulting dictionary with words as keys and their counts as values.

8. **Nested Dictionaries**  
   Create a dictionary that contains information about three different books, where each book has a title, author, and publication year. Write a program that prints the details of each book.

9. **Dictionary Comprehension**  
   Use dictionary comprehension to create a dictionary that maps integers from 1 to 10 to their squares. Print the resulting dictionary.

10. **Finding Maximum Value**  
    Write a program that takes a dictionary of employees with their salaries and finds the employee with the highest salary. Print the name of the employee along with their salary.

