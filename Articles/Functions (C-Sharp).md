#article

*[[Computer Science (CS)]] students may be looking for [[Functions (Python)]]*

In computer science, a function is a reusable block of code designed to perform a specific task. Functions help make programs more modular, readable, and easier to maintain. By using functions, programmers can avoid repeating code and manage complexity more effectively.

Functions in C# are essential for organizing code into manageable, reusable pieces. They support parameters, return types, and can be overloaded, making them a fundamental aspect of programming in C#.

----
#### Defining Functions

You can define a function in C-Sharp by declaring the `returnType`, followed by the `functionName`, and finally the `parameters` in parentheses following the name. 

A basic C# will look something like this:

```c#
void PrintGreeting()
{
	Console.WriteLine($"Hello, world.");
}
```

This function will write "Hello, world." to the console when called.

----
#### Parameters

Functions can take parameters (inputs) that allow passing data into them. Parameters can have default values and can be passed by value or by reference.

```c#
void Greet(string name = "Guest") 
{ 
	Console.WriteLine($"Hello, {name}!"); 
}
```

----
#### Return Types

Functions can return a value of a specified type (e.g., `int`, `string`, `void` for no return). The return type must be declared before the function name.

```c#
int Add(int a, int b) 
{ 
	return a + b; // Returns the sum of a and b 
}
```

----
#### Method Overloading

C# supports method overloading, allowing multiple functions with the same name but different parameters (type, number, or order).

```c#
void Display(int number) { /* ... */ }
void Display(string message) { /* ... */ }
```

----

#### Access Modifiers

Functions can have access modifiers (e.g., `public`, `private`, `protected`) that control visibility and accessibility when called from different classes.

```c#
public class MathMaster
{
	public int Add(int a, int b) { /*...*/ }
	private int Multiply(int a, int b) { /*...*/ }
}
```

In this example, `MathMaster`'s `Add` function is `public`, allowing it to be used by other classes outside of `MathMaster`. However, `Multiply` is set to `private`, meaning that the function can only be used within `MathMaster`.