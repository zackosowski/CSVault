#article 

Boolean expressions, also known as *conditions* or *condition statements*, are a fundamental concept in computer science and mathematics, used to represent logical statements that can be either true or false. Named after the mathematician George Boole, Boolean expressions are built using [[Variables]], constants, and [[Operators|logical operators]].

Simply put, a boolean expression is like a question that your computer can answer with a "yes" or "no". They are used for making decisions in programs, like [[If Statements]].

---
#### Parts of a Boolean Expression

* **[[Data|Values]]**: data in the form of numbers and [[String|strings]], often including [[Operators#Arithmetic Operators|arithmetic expressions]] 
* **[[Operators#Relational Operators|Relational Operators]]**: symbols that compare two values such as, >, <, ==
* **[[Operators#Logical Operators|Logical Operators]]**: symbols used to connect to or more conditions like `and` and `or`

Below are some examples of boolean expressions in [[Python]]. Click the Run button to evaluate the expressions.

```python
print(5 > 10)
# values: 5, 10
# realtional operator: >
```

```python
x = "blue"
print(x == "yellow")
# values: x, "yellow"
# realtional operator: ==
```

```python
answer = "cube"
count = 1
print(answer == "cube" and count < 10)
# values: answer, "cube", count, 10
# realtional operators: ==, <
# logical operators: and
```