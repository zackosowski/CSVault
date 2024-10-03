#article

*[[Computer Science (CS)]] students may be looking for [[Lists (Python)]].*

In [[C-Sharp]], a List is a part of the `System.Collections.Generic` namespace and is implemented as the `List<T>` class. It is a dynamic collection that can store any form of data or class, determined by the programmer by defining `<T>`

C# Lists are a powerful and flexible data structure that provide dynamic sizing, type safety, and a rich set of methods for managing collections. They are commonly used in scenarios where the number of elements may change during runtime, making them more versatile than arrays.

----
#### Using Lists

Lists can grow and shrink in size automatically as elements are added or removed, unlike arrays that have a fixed size.

```c#
List<int> numbers = new List<int>(); // Creates an empty list of integers
```

Lists are strongly typed. You specify the type of elements they hold using generics (e.g., `List<string>`), ensuring type safety at compile time.

```c#
List<string> fruits = new List<string> { "apple", "banana", "cherry" };
```

Lists come with a variety of methods for manipulation, such as `Add()`, `Remove()`, `Insert()`, `Sort()`, and `Count`, making it easy to manage the collection.

```c#
fruits.Add("date"); // Adds "date" to the list 
fruits.Remove("banana"); // Removes "banana" from the list
```

You can access elements by index, similar to arrays, with zero-based indexing.

```c#
string firstFruit = fruits[0]; // "apple"
```

---
#### Related Articles
[[C-Sharp]]