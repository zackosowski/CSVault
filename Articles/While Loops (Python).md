#article 

In programming, loops are essential tools that help repeat sections of code without manually writing the same instructions multiple times. One of the most common types of loops in Python is the **while loop**. Understanding how while loops work is fundamental for tasks that involve repeated actions based on conditions.

---
#### Basic Structure of a While Loop

The general syntax of a while loop in Python is as follows:

```python
while condition:
    # code to repeat
```

- **`condition`**: This is a [[Boolean Expression (Condition)|Boolean Expression]] that the loop checks. If it evaluates to `True`, the loop executes. If it is `False`, the loop stops.
- **Code Block**: Any code inside the loop (indented under `while`) will repeat as long as the condition remains `True`.
---
#### Example of a While Loop

Here’s a simple example of a while loop that prints numbers from 1 to 5:

```python
counter = 1
while counter <= 5:
    print(counter)
    counter += 1  # Increment the counter
```

- **Explanation**: 
  - The `counter` variable is initialized to 1.
  - The loop checks if `counter <= 5`. If it’s true, the code inside the loop executes.
  - `counter` is incremented by 1 each time the loop runs.
  - When `counter` reaches 6, the condition becomes false, stopping the loop.

---
#### Infinite Loops

A common problem with while loops is accidentally creating an **infinite loop**—a loop that never stops running. This happens when the loop's condition always evaluates to `True`, meaning the code inside never has a chance to break out.

Example of an infinite loop:
```python
while True:
    print("This loop will run forever!")
```

In the example above, since `True` is always true, the loop will never stop unless manually interrupted (like by pressing `Ctrl + C`).

**Avoiding Infinite Loops**
To prevent infinite loops, ensure that your loop has a condition that will eventually become `False` or use a statement to break out of the loop when needed.

---
#### Using Break Statements in While Loops

A `break` statement can be used to exit a while loop prematurely. This is helpful when you want the loop to stop based on a condition inside the loop, regardless of the initial condition in the while statement.

Example:
```python
counter = 1
while counter <= 10:
    print(counter)
    if counter == 5:
        break  # Exit the loop when counter reaches 5
    counter += 1
```

In this example, the loop will stop when `counter` reaches 5, even though the while condition would allow it to go up to 10.

---
#### Using Continue Statements in While Loops

The `continue` statement allows you to skip the rest of the code in the current loop iteration and proceed to the next iteration.

Example:
```python
counter = 0
while counter < 5:
    counter += 1
    if counter == 3:
        continue  # Skip the rest of the loop when counter is 3
    print(counter)
```

Here, the number 3 will be skipped in the output because the `continue` statement causes the loop to jump directly to the next iteration without executing `print(counter)`.

---
#### Real-World Example: Input Validation with While Loops

While loops are often used in programs to validate user input, ensuring the user provides data in the correct format.

Example:
```python
user_input = ""
while user_input.lower() != "exit":
    user_input = input("Enter something (type 'exit' to quit): ")
    print("You entered:", user_input)
```

In this example:
- The loop continues to prompt for input until the user types `"exit"`.
- It’s useful for scenarios where you want the program to keep running until a specific input is given.

---
#### While Loops vs. For Loops

While loops and python for loops are both used for repeating code, but they differ in purpose and structure:
- **For loops**: Best for when you know in advance how many times you need to iterate (e.g., iterating over a list).
- **While loops**: Best for when the number of repetitions depends on a condition that might change within the loop.

---
#### Nesting While Loops

You can place one while loop inside another, creating a **nested while loop**. This can be useful in scenarios where multiple conditions need to be met in each iteration of the outer loop.

Example:
```python
i = 1
while i <= 3:
    j = 1
    while j <= 2:
        print(f"i = {i}, j = {j}")
        j += 1
    i += 1
```

This example demonstrates a nested loop where the inner loop runs fully every time the outer loop iterates once.

---
#### Practice Activity

**Guess the Number**: Generate a random number between 1 and 100 then use a while loop to allow the user to guess the number. Provide feedback on whether the guess is too high, too low, or correct. The loop should continue until the user guesses the correct number.
