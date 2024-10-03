#article 

In computer science, a statement is a single line of code that performs a specific action. Statements are the building blocks of a program, instructing the [[Computers and Computing|computer]] on what to do step by step. Each statement typically corresponds to a specific instruction in the computer's underlying [[Machine Code|machine language]].

---
#### Expression Statement

An expression statement is a type of instruction that performs an action and usually changes the state of the program. It is made up of expressions, which can include [[Variables]], [[Operators]], [[Functions (Python)|function]] calls, and [[Data|values]]. When the statement is executed, the expressions are evaluated, and the resulting values might be assigned to variables, used in calculations, or passed to functions. Here are three main types of expression statements with examples:

###### Assignments
These statements assign a value to a variable
* `x = 5`
* `color = "yellow"`
* `dog1 = Dog()`

###### Function Calls
These statements tell functions to run, which perform specific tasks
* `print(x)
* `input("What is the password?)`
* `cities.append("Minneapolis)`

###### Mathematical Expressions
These statements perform calculations
* `y = x + 2` 

---
#### Control Flow Statements

Control flow statements are instructions that determine the order in which other statements are executed in a program. These statements enable a program to make decisions, repeat actions, and choose between different paths of execution, making the program dynamic and responsive to different inputs and [[Boolean Expression (Condition)|conditions]]:

**[[Conditional Statements]]**: Such as `if`, `else if`, and `else`, which allow the program to make decisions based on certain conditions (e.g., `if (x > 10) { ... }`).

**[[Loop Statements]]**: Such as `for`, `while`, and `do-while`, which repeat a block of code multiple times (e.g., `for (int i = 0; i < 10; i++) { ... }`).

**[[Jump Statements]]**: These alter the flow of control unconditionally. Examples include [[Jump Statements#Break|break]] (exits a loop), [[Jump Statements#Continue|continue]] (skips the current iteration of a loop), and [[Functions (Python)#Return|return]] (exits a function).
