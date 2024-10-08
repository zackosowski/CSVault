#lesson 

#### Targets
I can explain the contribution of George Boole to the world of computer science and algebra.

I can understand and apply comparison operators to compare values within Boolean expressions.

I can evaluate and predict the outcome of Boolean expressions and debug them if necessary.

---
#### Lesson
1. Introduction to the lesson
	* Making decisions in our code
	* Different "paths" through the program
	* Changes based on Boolean Expressions, also called "Conditions"<br><br>
2. Work through [[George Boole]] as a class<br><br>
3. Work through [[Boolean Expression (Condition)]] as a class
	* Show that `true` and `false` are keywords in python<br><br>
4. Work through [[Operators#Comparison Operators|Comparison Operators]]
	* Cover basic comparison operators using examples with print statements<br><br>
5. Complete the activity below<br><br>

<span style="color: #7b6cd9; border: 2px solid #7b6cd9; padding: 3px">ACTIVITY</span>

Boolean expression quiz! Guess the values of each of these Boolean expressions before revealing their answers.

<details>
	<summary>4 >= 2</summary>
		<p style="font-style: italic">True, fours is greater than or equal to two.</p>
</details>
<br>
<details>
	<summary>1993 == 1993</summary>
		<p style="font-style: italic">True, 1993 is equal to 1993</p>
</details>
<br>
<details>
	<summary>-90 &lt -99</summary>
		<p style="font-style: italic">False, negative ninety is NOT less than negative ninety-nine</p>
</details>
<br>
<details>
	<summary>10 != 10</summary>
		<p style="font-style: italic">False, ten is not NOT equal to ten.</p>
</details>
<br>
<details>
	<summary>4 > 3 and 3 > 2</summary>
		<p style="font-style: italic">True, four is greater than three and also three is greater than 2</p>
</details>

<hr>

6. Review the activity with the class<br><br>

7. Students complete [[Boolean Expressions Quiz]] assignment.

---
#### Supporting Code
```python
# Boolean Expressions

# Kinda like a mathematical formula

# 14 + 10 = 24      Algebra uses arithmetic operators

# + - / * ** % //

# Can only evaluate to True or False

# 5 > 10 = False    Boolean Algebra uses comparison operators

# > < >= <= == !=

  

print(14 + 10)      #Algebra

print(5 > 10)       #Boolean Algebra

  

x = 6               # SET x equal to 5, tell it what to be

print(x == 6)       # GET x equals 5, ask a question

  

# This is the PERFECT test question

# What is the difference between = and == ?

  

print(4 >= 2)           # True

print(1993 == 1993)     # True

print(-90 < -99)        # False

print(10 != 10)         # False, "not"

  

# Boolean expressions quiz!

answer_one = input("Give me an integer that is negative\n>")

answer_one = int(answer_one)

print(answer_one < 0)

  

answer_two = input("Write the number 5\n>")

print(answer_two == "5")

  

print("Walrus" + "Walrus")  #   WalrusWalrus

print("Walrus" == "Walrus") #   True
```
