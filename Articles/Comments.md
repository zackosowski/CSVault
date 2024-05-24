In computer programming, **comments** are notes added to code by developers to explain the purpose, functionality, or logic behind specific lines or sections of code. They are non-executable and serve as documentation for both the programmer and others who may read the code in the future.

Comments enhance code readability and maintainability. They help programmers understand their own code and enable collaboration among team members. Additionally, comments assist in [[debugging]] by providing insights into the programmer's intentions.

While comments are valuable, excessive or redundant commenting can clutter code and make it harder to read. It's crucial to strike a balance between providing sufficient explanation and avoiding unnecessary [verbosity](https://en.wikipedia.org/wiki/Verbosity).

---
#### Comments in Python

Python supports two types of comments: single-line comments and multi-line comments. Single-line comments start with a hash symbol (`#`). Multi-line comments are typically enclosed within triple quotes (`'''` or `"""`), although Python does not have a dedicated syntax for multi-line comments.

```python
# Calculate the area of a circle
radius = 5.0  # Radius of the circle

area = 3.14159 * radius ** 2 # Calculate area using pi * r^2 formula
print("Area of the circle:", area) # Output the result
```

In this Python example, the grey comments clarify the purpose of each line, aiding comprehension for both the programmer and others who may work with the code in the future.