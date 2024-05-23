#article 

In computer science, exception handling is a fancy way of saying how programs deal with unexpected [[errors]]. Imagine you're writing a program to calculate area, but someone enters a letter instead of a number. This unexpected event, called an exception, could crash the program. Exception handling allows you to catch these errors, display a user-friendly message (like "Enter a number!"), and keep the program running smoothly. It's like having a safety net to prevent your program from falling apart when things go wrong.

---
#### Python Error Handling

Python uses `try...except` blocks to handle exceptions.

*  **`try` block:** This block contains the code you think might cause an error. If an error occurs during execution, Python jumps out of the `try` block and checks for matching `except` blocks.

*  **`except` block:** This block follows the `try` block and is designed to catch specific errors. You can have multiple `except` blocks to handle different types of errors. Inside the `except` block, you write code to handle the error, such as displaying a user-friendly message or taking corrective actions.

*Example*
```python
try:
  result = 10 / 0  # This will cause a ZeroDivisionError
except:
  print("Oops! You can't divide by zero.")
```
In this example, the `try` block attempts to divide 10 by 0. Because dividing by zero throws an error, the `except` block will catches it and the program continues without crashing. Nice!

Python also allows you to specify the type of error you want to catch using the exception name after `except`. For instance, you can catch a `ZeroDivisionError` if someone tries to divide by zero.

*Example*
```python
try:
  result = 10 / 0  # This will cause a ZeroDivisionError
except:
  print("Oops! You can't divide by zero.")
```


There's also a third optional block called `finally`. The `finally` block always executes after the `try` block finishes, regardless of whether an error occurred. This is useful for code that needs to run every time, such as closing a file or releasing resources.