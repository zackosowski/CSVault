In computer science, an **error** is any issue in a program that prevents it from functioning as intended. Understanding and handling errors is crucial for writing reliable and efficient code. Errors can generally be categorized into two types: *compiler errors* and *runtime errors*.

---
#### Compiler Errors

Compiler [[Errors|errors]] are mistakes in a program's code that prevent it from being successfully [[Compiler|compiled]] into an executable program. If there are errors in the code, the compiler will generate error messages and stop the translation process.

###### **Syntax Errors**	
These occur when the code violates the [[Syntax]] rules of the [[programming language]]. For example, if you forget a colon at the end of an [[If Statements|if statement]] in [[Python]] or misspell a [[keyword]], you'll get a syntax error. Syntax errors are often the easiest to fix because they are underlined in red in the [[IDE (Integrated Development Environment)|IDE]] compiler usually provides specific details about what and where the problem is. Below are some examples of syntax errors.

```python
#The string is missing a closing quotation symbol
print("Hello World!)
```

```python
#The if statement is missing a color symbol
if x > 15
	print("x is greater than 15")
```

```python
#The p on print is capitalized
Print("Hello World!")
```

###### **Semantic Errors**
These happen when the code is syntactically correct but makes no sense logically. For instance, if you try to perform an operation on incompatible data types (like adding a number to a [[string]] in a language that doesn't allow it), you'll encounter a semantic error. These errors are harder to spot because the code looks correct but doesn't behave as expected.
 
 ###### **Linker Errors**
 These errors occur during the linking stage, which is after the compilation of the code. Linker errors happen when the compiler cannot find the correct references to functions or variables defined in other files or [[libraries]]. This might happen if you forget to include a necessary library or if there is a mismatch in [[Functions|function]] declarations.

---

#### Runtime Errors

In computer science, a **runtime error** occurs when a program encounters an issue during its execution. Unlike syntax errors, which are detected by the compiler or interpreter before the program runs, runtime errors occur while the program is running.

Runtime errors can result from various unexpected conditions or actions in the program, such as:

1. **Division by Zero**: Attempting to divide a number by zero.
2. **Invalid Input**: Providing input that the program cannot handle.
3. **Memory Issues**: Accessing memory locations that are not allocated or out of bounds.
4. **Type Errors**: Performing operations on incompatible data types.

When a runtime error occurs, the program may:

- Crash or terminate unexpectedly.
- Display error messages or warnings.
- Produce incorrect or unexpected output.


To handle runtime errors effectively:

1. **Debugging**: Use debugging tools to identify and fix the root cause of the error.
2. **Error Handling**: Implement mechanisms like exception handling to gracefully manage errors during program execution.
3. **Testing**: Conduct thorough testing to detect and address potential runtime errors before deploying the program.

### Example:

python

Copy code

`# Division by Zero Error numerator = 10 denominator = 0 result = numerator / denominator  # Causes a runtime error`

## How to Read an Error Message

Reading and understanding error messages is a vital skill for debugging. Here are common components of an error message:

1. **Error Type**: Indicates the kind of error (e.g., SyntaxError, TypeError, IndexError).
2. **Error Description**: Provides details about what caused the error.
3. **File and Line Number**: Shows where in the code the error occurred, which helps locate the problem quickly.
4. **Stack Trace**: For runtime errors, this shows the sequence of function calls that led to the error.

*Example of a Python error message*:
```plaintext
Traceback (most recent call last):
  File "example.py", line 3, in <module>
    num = int("abc")
ValueError: invalid literal for int() with base 10: 'abc'
```
In this message:
- **Error Type**: `ValueError`
- **Error Description**: `invalid literal for int() with base 10: 'abc'`
- **File and Line Number**: `File "example.py", line 3`

Understanding this structure helps in quickly identifying and fixing errors.
