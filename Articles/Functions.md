#article

In computer science, a function is a reusable block of code designed to perform a specific task. Functions help make programs more modular, readable, and easier to maintain. By using functions, programmers can avoid repeating code and manage complexity more effectively.

---
#### Defining Functions

To define a function in [[Python]], you use the `def` [[keyword]], followed by the function's name and parentheses. Inside the parentheses, you can include parameters, which are inputs to the function. After the parentheses, you write a colon and then indent the following lines, which contain the function's code.

Defining a function does not actually run it, it is just stored in into [[RAM (Random Access Memory)|memory]], sort of like a [[Variables|variable]]. The function can the be ran, or "called" at any time after its definition.

Here’s a basic example of a function in Python:

```python
def greet():
    print("Hello, world!")
```

In this example, `greet` is a function that prints "Hello, world!" when called.

---
### Parameters and Arguments

Lets say you had a function called `add` that's purpose is to add two numbers together. In order for the function to work properly, we first need to provide the details of *which two numbers.* Those details are called parameters, and their values are called arguments.

Parameters allow functions to accept inputs, making them more flexible. You define parameters inside the parentheses in the function definition. When you call the function, you pass the corresponding arguments.

Example with parameters:

```python
def greet(name):
    print(f"Hello, {name}!")
```

Here, the `greet` function takes one parameter, `name`. When you call `greet("Alice")`, it prints "Hello, Alice!". "Alice" being the argument.

You can also define functions with multiple parameters by separating them with a comma:

```python
def add(a, b):
    print(a + b)
```

In this example, the `add` function takes two parameters, `a` and `b`, and prints their sum. When you call `add(3, 4)`, it prints `7`.


<span style="color: #7b6cd9; border: 2px solid #7b6cd9; padding: 3px">ACTIVITY</span>

Create a function called `calculate_tax` that prints the amount of tax to be collected on an item. The function should take three parameters called `item`, `price`, and `rate`.
* `item` is the name of the item as a [[String]]
* `price` is the cost of the item in dollars, represented as a [[Float]]
* `rate` is the tax rate of the item. *Minnesota's sales tax rate is 6.875%*

---
### Return Statement

The `return` [[Keyword|keyword]] is used to send back a result from a function to its caller. This allows the function to produce output that can be used elsewhere in the program.

Example with a return value:

```python
def square(number):
    return number * number
```

When you call `square(5)`, the function returns `25`. You can store this returned value in a variable:

```python
def square(number):
    return number * number
    
result = square(5)
print(result)  # Outputs: 25
```


---
### Python Examples
```python
# Function with no parameters and no return value
def greet():
    print("Hello, world!")

# Function with one parameter
def greet(name):
    print("Hello, " + name + "!")

# Function with multiple parameters and a return value
def add(a, b):
    return a + b

# Function that calculates and returns an area
def calculate_area(width, height):
    return width * height
```
