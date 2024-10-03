#article

**Scope** in programming refers to the region within a program where a particular [[Variables|variable]] or [[Functions (Python)|function]] is accessible. Understanding scope is essential for managing and organizing code effectively, particularly when working with variables and functions in different contexts.

---
#### Types of Scope

1. **Global Scope**
	* Global scope refers to variables and functions that are defined **OUTSIDE** of any function or class, making them accessible throughout the entire program.
	* Variables defined in the global scope can be accessed and modified from anywhere in the code, including within functions.
	* Global variables are typically declared at the top of the script or module.
	* Example:
```python
global_var = 10 # Global variable

def print_global():
	print(global_var) # Accessing global variable
	
print_global() # Outputs: 10
```

2. **Local Scope**
	* Local scope refers to variables that are defined within a function or block of code, making them accessible only within that function or block.
	* Local variables are created when the function is called and are destroyed when the function exits.
	* They cannot be accessed outside of the function or block where they are defined.
	* Example:
```python
def my_function():
	local_var = 5 # Local variable
	print(local_var) # Accessing the local variable

my_function() # outputs 5
print(local_var) # Causes an error because the local variable does not exist at                     the global scope
```


<hr>

 #### Variable Shadowing

Variable shadowing occurs when a local variable in a function has the same name as a global variable. In such cases, the local variable shadows or overrides the global variable within that function's scope.

Example:
```python
global_var = 20  # Global variable

def my_function():
    global_var = 30  # Local variable shadows the global variable
    print(global_var)  # Outputs: 30

my_function()
print(global_var)  # Outputs: 20 (global variable remains unchanged)
```

<hr>

 #### Scope and Functions

* **Function Scope**: When a function is called, a new local scope is created. Variables defined within the function are local to that function and cannot be accessed outside of it.</br></br>
* **Accessing Global Variables in Functions**: To modify a global variable inside a function, you must use the `global` keyword to declare that you are referring to the global variable, not creating a new local one.

Example:
```python
global_var = 50

def modify_global():
    global global_var
    global_var = 100

modify_global()
print(global_var)  # Outputs: 100

```



---
#### Related Articles
[[Functions (Python)]]
