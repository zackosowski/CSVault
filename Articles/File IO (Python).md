#article

File input/output (I/O) is a fundamental concept in programming that allows a program to read from and write to files on a storage device. Understanding file I/O is essential for tasks such as data storage, logging, and configuration management. In Python, file I/O operations are straightforward, making it an excellent language for beginners to learn this concept.

---

#### Overview of File I/O

File I/O involves two main operations: reading data from a file and writing data to a file. When working with files in Python, you typically use built-in functions and methods to open, read, write, and close files. Files can be opened in different modes, which determine how you can interact with them, such as reading, writing, or appending data.

---

#### Opening Files

To work with a file, you first need to open it using the `open()` function. The syntax is as follows:

```python
file = open('filename.txt', 'mode')
```

Here, `filename.txt` is the name of the file you want to open, and `mode` specifies how you want to interact with the file. Common modes include:

- `'r'`: Read mode (default), opens a file for reading.
- `'w'`: Write mode, opens a file for writing (creates a new file or truncates an existing file).
- `'a'`: Append mode, opens a file for appending new data at the end.
- `'r+'`: Read and write mode, allows both reading and writing.

**Warning:** Opening a file in write mode will overwrite any existing data in the file. Be cautious when using this mode to avoid data loss.

---

#### Reading from Files

Once a file is opened in read mode, you can read its contents using several methods:

1. **`read()`**: Reads the entire file as a single string.
   ```python
   content = file.read()
   ```

2. **`readline()`**: Reads the next line from the file.
   ```python
   line = file.readline()
   ```

3. **`readlines()`**: Reads all lines and returns them as a list of strings.
   ```python
   lines = file.readlines()
   ```

After reading the data, it’s important to close the file to free up system resources.

```python
file.close()
```

---

#### Writing to Files

To write data to a file, open it in write or append mode. Use the following methods to write data:

- **`write()`**: Writes a string to the file.
  ```python
  file.write('Hello, World!')
  ```

- **`writelines()`**: Writes a list of strings to the file.
  ```python
  lines = ['First line\n', 'Second line\n']
  file.writelines(lines)
  ```

Remember to close the file after writing to ensure that all data is saved.

---

#### Using Context Managers

A common practice in Python is to use a context manager when working with files. This automatically handles opening and closing the file for you, which is safer and cleaner. You can use the `with` statement as follows:

```python
with open('filename.txt', 'r') as file:
    content = file.read()
```

When the block under the `with` statement is exited, the file is automatically closed, even if an error occurs.

---

#### Practice Activity

Create a program that performs the following tasks:

1. Write a list of five of your favorite movies to a file named `movies.txt`, with each movie on a new line.
2. Read the contents of `movies.txt` and print them to the console.
3. Append a new movie to `movies.txt` and read the contents again to verify the new entry.

This activity will help you understand how to handle file I/O operations effectively.