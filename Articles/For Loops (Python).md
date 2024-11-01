#article

In Python, a *for loop* allows code to be repeated over a sequence, such as a list, tuple, string, or range of numbers. Unlike while loops, which continue based on a condition, for loops iterate over each element in the specified sequence, making them ideal for when you know exactly how many times you want the loop to run.

---
#### Syntax of a For Loop

The syntax of a for loop in Python is as follows:

```python
for variable in sequence:
    # Code to execute for each item in the sequence
```

- **`variable`**: The name of the variable that will hold each item in the sequence one at a time.
- **`sequence`**: The collection of items to iterate over (e.g., a list, range, or string).
----
#### Example

###### Looping Over a List
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```
###### Looping Over a String
```python
for letter in "hello":
    print(letter)
```
###### Looping Over a Range
The `range()` function generates a sequence of numbers, which is often used in for loops when you want to repeat an action a certain number of times.

```python
for i in range(5):
    print(i)
```

- `range(5)` generates numbers from 0 up to, but not including, 5.
- `range(start, stop, step)` is also valid, where `start` is the starting point, `stop` is the endpoint, and `step` is the increment.

---
#### Common For Loop Patterns

###### Accumulating Values
For loops are commonly used to calculate a sum or product of a sequence of numbers.

```python
numbers = [2, 4, 6, 8]
total = 0
for num in numbers:
    total += num
print(total)
```
###### Filtering Items
You can use a for loop to filter specific items from a list based on a condition.

```python
numbers = [1, 2, 3, 4, 5]
even_numbers = []
for num in numbers:
    if num % 2 == 0:
        even_numbers.append(num)
print(even_numbers)
```

---
#### Nested For Loops

A *nested for loop* is a for loop inside another for loop. This is often used to work with two-dimensional data, like lists of lists.

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

for row in matrix:
    for item in row:
        print(item, end=" ")
    print()
```

---
### Using `break` and `continue` in For Loops

- **`break`**: Stops the loop entirely when a certain condition is met.
- **`continue`**: Skips the current iteration and continues with the next one.

```python
# Using break
for i in range(5):
    if i == 3:
        break
    print(i)
```

```python
# Using continue
for i in range(5):
    if i == 3:
        continue
    print(i)
```

---
#### Practice Problems

Write a Python program that performs the following tasks using for loops:

1. **Print a Countdown**: Create a countdown from 10 to 1 using a for loop. Print each number on a new line.
    
2. **Sum of a List**: Create a list of 10 integers, use a for loop to calculate the sum of the numbers in the list and print the result.
    
3. **Square Each Number**: Create a list of integers from 1 to 5. Use a for loop to create a new list that contains the squares of these numbers. Print the new list.
    
4. **Character Count**: Ask the user to enter a string. Use a for loop to count and print the number of vowels (a, e, i, o, u) in the string.
    
5. **Print Multiplication Table**: Use a for loop to print the multiplication table for a number provided by the user (e.g., 5). Print the results in a readable format (e.g., `5 x 1 = 5`).
    
6. **List of Names**: Create a list of names (e.g., `names = ["Alice", "Bob", "Charlie"]`). Use a for loop to print a greeting for each name in the list (e.g., `Hello, Alice!`).