#article

In computer science, a variable is a fundamental concept used to store and manage [[data]] within a program. Think of a variable as a container or a storage box that holds information which can be changed or updated as the program runs.

---
#### Declaration

To use a variable, you first need to declare it. This means telling the computer what kind of data the variable will hold, such as numbers, text, or more complex data types. For example, in [[Python]], you can declare a variable by simply writing its name and assigning a value to it:

   ```python
   age = 16
   name = "Alice"
   ```
Here, `age` is a variable that stores the number 16, and `name` stores the text "Alice". 

---
#### Naming Variables

Variable [[Naming Conventions|naming conventions]] are guidelines that help programmers choose names for variables in their code. Good variable names are essential for writing clear and maintainable code. A good variable name should be:

1. **Descriptive**: Clearly indicate what the variable represents.
2. **Concise**: Be as short as possible while still being descriptive.
3. **Consistent**: Follow the same style throughout the code.
4. **Readable**: Easy to read and understand, avoiding ambiguity.

###### Python
In Python, variable names should follow the [[Naming Conventions#Snake Case|snake_case]] naming convention. Words are separated by underscores (`_`), and all letters are lowercase.

Examples:
- `student_name` instead of `sN` or `sn`
- `total_score` instead of `ts` or `totals`

```python
student_name = "Alice"
total_score = 95
```

###### JavaScript
In JavaScript, variable names should follow the [[Naming Conventions#Camel Case|camelCase]] naming convention. The first word is lowercase, and each subsequent word starts with an uppercase letter.

Examples:
- `studentName` instead of `sn` or `student_name`
- `totalScore` instead of `ts` or `total_score`

```javascript
let studentName = "Alice";
let totalScore = 95;
```

---
#### Assignment

You can change the value of a variable by reassigning it at any point in your program.

   ```python
   name = "Bob"
   print("Hello " + name + "!")
   
   name = "Tom"
   print("Hello " + name + "!")
   ```
In this example, `name` was *declared* on line 1, and *reassigned* on line 4.
#### Importance

Variables are crucial because they allow programs to store, manipulate, and retrieve data dynamically. This makes it possible to create programs that can handle a wide range of tasks, from simple calculations to complex simulations.

---
#### Warehouse Analogy

Imagine a warehouse where items are stored in boxes. In this analogy, the warehouse is tour [[RAM (Random Access Memory)|RAM]] and each box is a variable.

**Boxes and Labels**
Each box in the warehouse has a label that identifies it, just like a variable has a name. For example, one box might be labeled `age` and another `name`. Anytime the program wants to use a variables, it checks the warehouse for a box of the name you requested and gives you the content inside of it.

**Contents**
Inside each box, there's something stored, which represents the value of the variable. The box labeled `age` might contain the number 16, while the box labeled `name` might hold the text "John".

**Changing Contents**
You can open any box and change what's inside. If John has a birthday, you take out the number 16 from the `age` box and replace it with the number 17. Similarly, if John wants to start going by his full name now that he's much older and sophisticated, you could change the contents of the `name` box to "Johnathan"

**Missing Box**
What happens if we request a box in the warehouse, only to realize that that box doesn't exist? In this case, we would get an [[Errors|error]] because the variable does not exist.

By thinking of variables as labeled boxes in a warehouse, it becomes easier to understand how data is stored, accessed, and managed in a computer program.

---
#### Local vs Global Variables

###### Local Variables
Local variables are declared within a specific block of code, like inside of a [[Functions|function]] or a [[Loop Statements|loop]]. They can only be accessed and used within that block. Once the block of code has finished executing, the local variables are destroyed from memory, and their values are lost.

**Example:**

```python
def example_function():     
	local_var = 10 # This is a local variable
	print(local_var) 
	
example_function()
# Output: 10
# local_var cannot be accessed outside example_function
````

In this example, `local_var` is a local variable and only exists inside `example_function`.

###### Global Variables
Global variables are declared outside of all functions or blocks, usually at the top of the program. They can be accessed and modified from any part of the program, making them useful for data that needs to be shared across multiple functions.

**Example:**

```python
global_var = 20  # This is a global variable

def another_function():
	print(global_var)
	
another_function()
# Output: 20
# global_var can be accessed from anywhere in the program
```

In this example, `global_var` is a global variable and can be accessed inside `another_function` or any other function in the program.

The problem with global variables comes when you try to modify their value inside another block. If you try to modify a global variable inside of a function, python will instead create a new, local variable with the same name. to avoid this, use the `global` keyword inside the function to designate the variable as global.

```python
```python
count = 0  # This is a global variable

def increase_count():
	global count # Decalre the count variable as global
	count += 1   # Modify the global variable
	print(count)
	
increase_count()
# Output: 1
```

**Key Differences:**

1. **Scope:** Local variables are limited to the block where they are defined. Global variables are accessible throughout the entire program.
2. **Lifetime:** Local variables exist only during the execution of the block they are in. Global variables exist for the duration of the program's execution.
3. **Access:** Local variables cannot be accessed outside their defining block, whereas global variables can be accessed from any function.

Using global variables can simplify sharing data across multiple functions, but it can also make debugging harder because any function can change the value. Local variables, on the other hand, help keep functions independent and easier to manage.
