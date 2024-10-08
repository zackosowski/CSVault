#article 

The most common types of [[Conditional Statements]] are `if`, `else if`, and `else` statements. These statements evaluate [[Boolean Expression (Condition)|boolean expressions]], which are expressions that return either `true` or `false`.

---
#### Coin Sorter Analogy

Imagine you have a coin sorting machine that sorts coins based on their size. This machine has several pans stacked on top of each other, each with holes of different sizes. The coins are dropped into the top pan and move downwards, getting sorted based on their size as they pass through the holes.

Here’s how this coin sorting machine is analogous to `if` statements in programming:

1. **Top Pan (First If Statement)**:
    
    - The top pan has the largest holes, allowing only the biggest coins to pass through. This is similar to the first `if` statement, which checks if a [[Boolean Expression (Condition)|condition]] is true. If it is, the code inside this `if` block is executed, just like how the biggest coins pass through the first set of holes.

2. **Middle Pans (Else If Statements)**:
    
    - The middle pans have progressively smaller holes. Coins that are too small for the top pan but large enough for these pans pass through. These pans act like `else if` statements, which check additional conditions if the previous `if` condition was not met. Each `else if` statement represents another pan with a different hole size, catching the coins (conditions) that match.

3. **Bottom Pan (Else Statement)**:
    
    - The bottom pan has no holes and catches all the remaining coins (and pocket lint) that did not pass through any of the previous pans. This is like the `else` statement, which catches all conditions not met by any previous `if` or `else if` statements. If none of the prior conditions are true, the code inside the `else` block is executed. The else statement does not discriminate, it takes whatever is left.

An important takeaway from this analogy is that each coin only settings into a single pan. This is the same way if statements work; only one if/else if/else statement is ran.

---
#### Python

- **If Statement**: The [[If Statements|if statement]] checks a condition. If the condition is true, the block of code inside the if statement is executed. For example:
  ```python
  temperature = 81
  if (temperature > 80):
	  print("It's a hot day!")
  ```
  In this example, if the `temperature` [[Variables|variable]] is greater than 80, the program will print "It's a hot day!". If the `temperature` [[Variables|variable]] is NOT greater than 80, the program will not print anything.

- **Else Statement**: The else statement follows an if statement and executes if the [[Boolean Expression (Condition)|condition]] in the if statement is false. For instance:
  ```python
  temperature = 79
  if (temperature > 80):
      print("It's a hot day!")
  else:
      print("It's not a hot day.")
  ```
  Here, if the `temperature` variable is not greater than 80, instead of doing nothing, the program will print *"It's not a hot day."*

- **Else If Statement**: The else if (or *elif* in some [[Programming Language|languages]]) statement allows for multiple conditions to be checked in sequence. The first condition that is true will have its block of code executed. For example:
  ```python
  temperature = 79
  if (temperature > 80):
      print("It's a hot day!")
  elif (temperature > 70):
      print("It's a warm day.")
  else:
      print("It's a cool day.")
  ```
  This program checks multiple temperature ranges and prints a message based on which condition is true.
---

<span style="color: #7b6cd9; border: 2px solid #7b6cd9; padding: 3px">ACTIVITY</span>

Create a password checker.
1. Ask the user for a password
2. If the password is correct, print `ACCESS GRANTED`
3. If its wrong, print `ACCESS DENIED`
