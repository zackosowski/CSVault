#lesson 

#### Targets
I can use if and else statements to make decisions about what code should run in my python programs.

I can create a simple quiz that tallies a score.

---
#### Lesson

1. Work through [[If Statements#Python]] as a class
	1. Use supporting code below as a guide
2. Students complete the if statements password activity
3. Review activity
4. Work through
5. Students complete [[Simple Quiz]]

---
#### Supporting Code

```python
# If statements evaluate boolean expressions!

# Thye make decisions about which code to run next

  

# Take a temperature

# Print "<temperature> is hot" if its >= 80

# Otherwise, print "<temperature is not hot"

temp = input("Whats the temperature in F?\n>")

temp = int(temp)

  

# if <boolean expression>:

# This should remind of writing a function

# def <name>():

if temp >= 80:

    print(str(temp) + "° is hot!")

  

else:   # Otherwise....

    print(str(temp) + "° is not hot...")

  

# Not all if statements need an else, in fact NONE of them NEED and else

# Else statements are an option, they are optional

# All else statements must have a corresponding if statement

# Else statements cannot exist alone

# An if statement can only have one else

  

# Create a program that asks for a password

# IF the password is correct, print ACCESS GRANTED

# Otherwise, print ACCESS DENIED

# The password is skibidi68

  

real_pass = "skibidi68"

input_pass = input("Whats the password?\n>")

  

if input_pass == real_pass:

    print("ACCESS GRANTED")

else:

    print("ACCESS DENIED")

  
  

# Activity 2, electric boogaloo

# Create a five question quiz that prints your score at the end

# Choose any five questions

# EZ
```
