#article

In computer science, input functions are used to gather [[data]] from users or other sources. These [[Functions (Python)]] are essential because they allow programs to be interactive and responsive to user needs. Input functions can read data entered through a keyboard, a file, or other input devices.

---
#### Input Function in Python

[[Python]] provides simple and powerful ways to get input from users. The basic input function in Python is `input()`. This function reads a line of text entered by the user and [[Functions (Python)#Return|returns]] it as a [[string]].

The `input()` function prompts the user to enter data. The [[syntax]] is straightforward:


```python
user_input = input("Enter something: ")
print("You entered: " + user_input)
```


In this example, the program displays the message "Enter something:". The user types something and presses Enter. Whatever the user types is stored in the [[Variables|variable]] `user_input` as a string, and then the program [[Print Functions|prints]] it back to the user.

---
#### Converting Input Data Types

Since `input()` always returns a string, you might need to convert the input to other [[Data#Data Types|data types]]. For example, if you want to read an [[integer]], you can use the `int()` function:

```python
num = input("Enter the number you want to sqaure:")
num = int(num)
print(num * num)
```

Here, the user's input is first stored as a string, then converted to an integer so that it can be used in the arithmetic expression later.

---
#### Handling Invalid Input

Using an input function is just asking for [[errors]] to occur. Allowing a user to type anything into an input often leads to unexpected results. It is important to [[Exception Handling|handle]] these unexpected results when using input functions.

```python
try:    
	age = int(input("Enter your age: "))
	print("You are", age, "years old.")

except ValueError:     
	print("That's not a valid number!")
```

In this example, if the user enters something that cannot be converted to an integer, the program will print an error message instead of crashing.