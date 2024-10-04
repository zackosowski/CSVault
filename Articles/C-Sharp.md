#article

C# (pronounced "C-sharp") is a modern, object-oriented [[programming language]] developed by Microsoft as part of the .NET framework. Introduced in the early 2000s, it combines the power of C and C++ with features that enhance productivity and safety, such as garbage collection, type safety, and rich libraries. C# is widely used for developing Windows applications, web services, and games, especially with the Unity engine. Its [[syntax]] is clean and easy to read, making it accessible for beginners while still powerful enough for experienced developers. With support for asynchronous programming and a strong community, C# continues to evolve and remains a popular choice for a variety of applications.

---
#### Key Features

- **Object-Oriented Programming:** C# is a fully object-oriented language, meaning it is built around the concepts of [[classes and objects]]. This allows developers to create modular, reusable code. By bundling data and methods into a single unit (class), the language promotes data hiding and reduces complexity.

- **Type Safety**: C# enforces strict type checking at compile-time, reducing the chances of runtime errors. Many common programming errors (like using a string as a number) are caught early in the development process, leading to more stable code. Clear data types make the code easier to understand and maintain, as developers know exactly what type of data is being used.

---
#### Data Types

C# supports many of the same [[data types]] as [[Python]], such as:
- **[[Integer|Integers]]**: Whole numbers, e.g., `5`, `419`.
- **[[Float|Floats]]**: Decimal numbers, e.g., `3.14`, `0.001`.
- **[[String|Strings]]**: Text, e.g., `"Hello World"`, `"C# is really cool!"`.
C# also supports some data types exclusive to the language, such as:
- Arrays: Fixed-size data structures, e.g., `"apple"`, `"banana"`, `"cherry"`.
- [[Lists (C-Sharp)|Lists]]: Dynamic, more flexible data structures
- [[Class|Classes]]: Custom data structures, with properties and methods, e.g., `class Person { public string Name; public int Age; }`.
----
#### Control Structures

Like Python, C# uses loops and conditional statements. However, the syntax is very different.

Here's an example of an if/else statement:

```c#
int x = 4;

if(x > 5)
{
	Console.WriteLine("x is greater than 5");
}
else
{
	Console.WriteLine("x is less than or equal to 5");
}
```

And, an example of a simple for loop:

```c#
for(int i = 0; i < 5; i++)
{
	Console.WriteLine("This loop has ran: "+ (i+1) + "time(s)!");
}
/* Output:

This loop has ran 1 time(s)!
This loop has ran 2 time(s)!
This loop has ran 3 time(s)!
This loop has ran 4 time(s)!
This loop has ran 5 time(s)!
*/
```

----
#### Functions
[[Functions (C-Sharp)|Functions]] are declared by stating the `returnType`, followed by the `functionName`, and finally the `parameters` in parentheses following the name. 

A basic C# will look something like this:

```c#
void PrintGreeting(){
	Console.WriteLine($"Hello, world.");
}
```

This function will write "Hello, world." to the console when called. It takes no parameters.

----
#### Usage

**Game Development**
- **[[Unity Game Engine]]**: C# is the primary language used in Unity, one of the most popular game development platforms (and the program used for [[Video Game Design (VGD)]] class!). Developers use C# to script game mechanics, control character behaviors, and manage game interactions.
- **[Godot](https://godotengine.org/)**: Godot supports C# as an option for a scripting language, alongside Godot's own GDScript language.

**Desktop Applications**
- **[Microsoft Visual Studio](https://visualstudio.microsoft.com/)**: A powerful integrated development environment (IDE) used for developing applications in various languages, including C#. It provides tools for code editing, debugging, and project management.
- **[Notepad++](https://notepad-plus-plus.org/)**: Although primarily written in C++, it has plugins and features that are often developed using C#. This source code editor is widely used for programming and text editing.
- **[Revit](https://www.autodesk.com/products/revit/architecture)**: A Building Information Modeling (BIM) software used in architecture, engineering, and construction. It allows for custom plugin development in C#, enabling users to extend functionality.

----
#### Related Articles
[[Functions (C-Sharp)]]