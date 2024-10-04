
#### Import

Use the `import` [[keyword]] to import a [[Libraries|library]].

  ```python
  import math   # Import statement
  print(math.sqrt(16))  # Outputs: 4.0
  ```
In this example, we imported `math` on line 1 so that we could use it later on line 2.

---
#### From

The `from` keyword allows you to import specific attributes (like functions, classes, or variables) from a module instead of importing the entire module. This can make your code more concise and save memory.

```python
from module_name import attribute_name
```

If you only need the `sqrt` function from the `math` module:

```python
from math import sqrt
print(sqrt(16))  # Outputs: 4.0
```

This approach is useful when you only need a few functions or classes from a large module.

You can import multiple attributes by separating them with commas:

```python
from math import sqrt, pi
print(sqrt(16))  # Outputs: 4.0
print(pi)        # Outputs: 3.141592653589793
```

---
#### As

The `as` keyword allows you to give an imported module or attribute a different name, which can be helpful for avoiding name conflicts or for simplifying long module names.

```python
import module_name as alias
from module_name import attribute_name as alias
```

If a module name is long, you can alias it for convenience:

```python
import numpy as np
array = np.array([1, 2, 3])
print(array)  # Outputs: [1 2 3]
```

You can also alias specific attributes:

```python
from math import sqrt as square_root
print(square_root(16))  # Outputs: 4.0
```

You can use both keywords together to import specific attributes with aliases:

```python
from datetime import datetime as dt
current_time = dt.now()
print(current_time)  # Outputs: current date and time
```

---
#### Installing New Libraries

**Pip** is a package manager for Python that simplifies the process of installing and managing software packages written in Python. It stands for "Pip Installs Packages" or "Preferred Installer Program". Pip is an essential tool for Python developers as it enables them to easily access and integrate a wide range of third-party libraries and tools into their projects.

To browse Python packages, use [pypi.org](https://pypi.org/)

In most cases, Pip comes pre-installed with Python. However, if you need to install it manually, you can use the following commands in the [[terminal]]:

- On Windows:
  ```
  python -m ensurepip --upgrade
  ```

- On macOS and Linux:
  ```
  sudo apt-get install python3-pip
  ```

Pip provides a simple command-line interface for installing, upgrading, and removing Python packages. Here are some common commands:

- **Install a Package**:
  ```
  pip install package_name
  ```

- **Install a Specific Version**:
  ```
  pip install package_name==version_number
  ```

- **Upgrade a Package**:
  ```
  pip install --upgrade package_name
  ```

- **Remove a Package**:
  ```
  pip uninstall package_name
  ```

