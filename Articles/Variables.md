#article

In computer science, a variable is a fundamental concept used to store and manage [[data]] within a program. Think of a variable as a container or a storage box that holds information which can be changed or updated as the program runs.

---
#### Declaration
To use a variable, you first need to declare it. This means telling the computer what kind of data the variable will hold, such as numbers, text, or more complex data types. For example, in Python, you can declare a variable by simply writing its name and assigning a value to it:

   ```python
   age = 16
   name = "Alice"
   ```
Here, `age` is a variable that stores the number 16, and `name` stores the text "Alice". 

---

#### Assignment

You can change the value of a variable by reassigning it at any point in your program.

   ```python
   name = "Bob"
   print("Hello " + name + "!")
   
   name = "Tom"
   print("Hello " + name + "!")
   ```
In this example, `name` was *declared* on line 1, and *reassigned* on line 4.
#### Importance

Variables are crucial because they allow programs to store, manipulate, and retrieve data dynamically. This makes it possible to create programs that can handle a wide range of tasks, from simple calculations to complex simulations.

---
#### Warehouse Analogy

Imagine a warehouse where items are stored in boxes. In this analogy, the warehouse is tour [[RAM (Random Access Memory)|RAM]] and each box is a variable.

**Boxes and Labels**
Each box in the warehouse has a label that identifies it, just like a variable has a name. For example, one box might be labeled `age` and another `name`. Anytime the program wants to use a variables, it checks the warehouse for a box of the name you requested and gives you the content inside of it.

**Contents**
Inside each box, there's something stored, which represents the value of the variable. The box labeled `age` might contain the number 16, while the box labeled `name` might hold the text "John".

**Changing Contents**
You can open any box and change what's inside. If John has a birthday, you take out the number 16 from the `age` box and replace it with the number 17. Similarly, if John wants to start going by his full name now that he's much older and sophisticated, you could change the contents of the `name` box to "Johnathan"

**Missing Box**
What happens if we request a box in the warehouse, only to realize that that box doesn't exist? In this case, we would get an [[Errors|error]] because the variable does not exist.

By thinking of variables as labeled boxes in a warehouse, it becomes easier to understand how data is stored, accessed, and managed in a computer program.

---
#### Scope and Lifetime

**Scope**
The scope of a variable determines where in the program the variable can be accessed. Variables declared inside a function are local to that function, while variables declared outside are global.

**Lifetime**
The lifetime of a variable is the period during which it exists in memory. Local variables exist only while the function runs, while global variables exist for the duration of the program.
