#article 

In [[Python]], a dictionary is a collection of [[data]] organized in a special way. Unlike [[List|lists]] and [[Tuple|tuples]] that store items in a sequence, dictionaries store data in **key-value pairs**. Imagine a phone book - each name (key) has a corresponding phone number (value). That's exactly how dictionaries work!

---
### Keys and Values

- **Keys** act like unique identifiers (like names in a phone book) and must be immutable data types. This means they can't be changed after creation. Common choices for keys include [[String|strings]], [[Integer|integers]], or [[Tuple|tuples]] containing immutable data types.
- **Values** can be any type of data (numbers, strings, lists, even other dictionaries!) and store the actual information you want to associate with the key.

Here's an example of a dictionary that stores information about your favorite video games:

```python
games = {
    "Name": "Minecraft",
    "Genre": "Adventure",
    "Year": 2011,
    "Platform": ["PC", "Mobile", "PS5", "PS4", "XB1"]
}
```

In this example, "Name", "Genre", "Year", and "Platform" are all keys, and their corresponding values are "Minecraft", "Adventure", 2011, and a list containing platforms the game is available on.

---
#### Using Dictionaries

There are several ways to work with dictionaries in Python. Here's a quick overview:

- **Creating a Dictionary:** You can enclose key-value pairs within curly braces `{}`.
- **Accessing Values:** Use the key within square brackets `[]` to get the corresponding value.
- **Adding Key-Value Pairs:** Use the assignment operator `=` to add new key-value pairs.
- **Removing Key-Value Pairs:** Use the `del` keyword with the key to remove it.

Here's an example demonstrating how to access and modify a dictionary:

```python
# Accessing a value
genre = games["Genre"]
print(genre)  # Output: Adventure

# Adding a new key-value pair
games["Players"] = "Multiplayer"

# Removing a key-value pair
del games["Year"]

print(games)  # Output: {'Name': 'Minecraft', 'Genre': 'Adventure', 'Platform': ['PC', 'Mobile', 'Consoles'], 'Players': 'Multiplayer'}
```

By understanding dictionaries, you can effectively store and manage complex data in your Python programs, making them more organized and easier to work with.
