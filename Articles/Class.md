#article

In C#, a class is a fundamental building block of object-oriented programming (OOP) that serves as a blueprint for creating objects. A class encapsulates data (attributes) and behavior (methods) related to a specific concept or entity.

---
#### Instantiation

Instances of a class (objects) are created using the `new` keyword. Each object has its own copy of the class's attributes.

```c#
class Person {
    public string Name;
    public int Age;
    public void Greet() {
        Console.WriteLine($"Hello, my name is " + this.Name + "and I am" + this.Age + " years old.");
    }
}

Person alice = new Person();
alice.Name = "Alice";
alice.Age = 30;
alice.Greet();  // Output: Hello, my name is Alice and I am 30 years old.

Person josh = new Person();
josh.Name = "Josh";
josh.Age = 25;
josh.Greet();  // Output: Hello, my name is Josh and I am 25 years old.
```

In this example, we created the `Person` class, and used it to instantiate 2 new person objects, each with their own name and age attached to them.

---
#### Related Articles
