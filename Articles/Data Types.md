#article

Not all [[data]] is made equal. In fact, data comes in many forms and types, and those types matter.

For example, if I asked you how old you are, I would expect to receive a number back. But if you responded to the question with something like "Fortnite", I would be terribly confused. This is because there is a mismatch between the type of data I expected to receive and the type of data you gave me. I wanted a number but you gave me a random word....

Here are some common data types (there are many more)
* [[Integer]] (whole numbers, can be positive or negative, or zero)
* [[Float]] (floating point number aka decimal number)
* [[Character]] (a single character)
* [[String]] (a group or "string" of characters)
* [[Boolean]] (a special type of data that can only be True or False)

---
#### Data Type Conversion

Converting data types is crucial for several reasons:

1. **Data Compatibility:** Different functions require specific data types. For example, mathematical operations need numbers, while concatenation requires strings.
2. **Data Processing:** When reading data from files or user input, the data is often in string format and needs to be converted to other types for processing.
3. **Storage Optimization:** Converting data to a more appropriate type can save memory and improve performance. For instance, using integers instead of floats when decimal precision is unnecessary.
4. **Avoiding Errors:** Ensuring that data is in the correct format prevents runtime errors that can occur from type mismatches.

---
#### Python Type Conversions

Python provides built-in functions to convert between different data types, which is known as type casting. Here are some common conversions:

**Integer to String**
 ```python
num = 123 num_str = str(num)
```

**String to Integer**
```python
num_str = "123" num = int(num_str)
```

**String to Float**
```python
float_str = "123.45" num = float(float_str)
```

**Integer to Float**
```python
num = 123 num_float = float(num)
```
    
**Float to Integer**
```python
num_float = 123.45 num = int(num_float)
```

