A comprehensive quick reference guide for Python (3.x). Perfect for developers, learners, and bug hunters.

---

## 📌 Table of Contents

- [🧱 Basics](#-basics)
- [📦 Data Types](#-data-types)
- [🔁 Conditionals & Loops](#-conditionals--loops)
- [🔧 Functions](#-functions)
- [🎒 Collections](#-collections)
- [🛠️ Modules & Imports](#-modules--imports)
- [🗃️ File I/O](#-file-io)
- [🧵 Error Handling](#-error-handling)
- [🎭 Classes & OOP](#-classes--oop)
- [⏳ Comprehensions](#-comprehensions)
- [🔗 Lambda, Map, Filter, Reduce](#-lambda-map-filter-reduce)
- [🧪 Virtual Environments](#-virtual-environments)
- [🔍 Debugging Tips](#-debugging-tips)
- [📚 Useful Libraries](#-useful-libraries)

---

## 🧱 Basics

```python
# Comments
# Single-line comment
""" Multi-line
comment """

# Print
print("Hello, World!")

# Variables
x = 5
name = "Alice"
```

---

## 📦 Data Types

```python
# Numbers
int_num = 10
float_num = 3.14
complex_num = 2 + 3j

# Strings
s = "hello"
s.upper()       # "HELLO"
s[0]            # 'h'

# Boolean
is_true = True
```

---

## 🔁 Conditionals & Loops

```python
# If, Elif, Else
if x > 0:
    print("Positive")
elif x < 0:
    print("Negative")
else:
    print("Zero")

# For Loop
for i in range(5):
    print(i)

# While Loop
while x > 0:
    x -= 1
```

---

## 🔧 Functions

```python
def greet(name):
    return f"Hello, {name}"

# Default argument
def greet(name="Guest"):
    return f"Hello, {name}"
```

---

## 🎒 Collections

### List

```python
lst = [1, 2, 3]
lst.append(4)
lst[0]  # 1
```

### Tuple

```python
t = (1, 2)
t[0]  # 1
```

### Set

```python
s = {1, 2, 2}
s.add(3)
```

### Dictionary

```python
d = {"name": "Alice", "age": 25}
d["name"]       # "Alice"
d.get("age")    # 25
```

---

## 🛠️ Modules & Imports

```python
import math
from datetime import datetime

print(math.sqrt(16))
```

---

## 🗃️ File I/O

```python
# Writing
with open("file.txt", "w") as f:
    f.write("Hello")

# Reading
with open("file.txt", "r") as f:
    content = f.read()
```

---

## 🧵 Error Handling

```python
try:
    x = 1 / 0
except ZeroDivisionError as e:
    print("Cannot divide by zero")
finally:
    print("Done")
```

---

## 🎭 Classes & OOP

```python
class Person:
    def __init__(self, name):
        self.name = name

    def greet(self):
        return f"Hi, I'm {self.name}"

p = Person("Alice")
p.greet()
```

---

## ⏳ Comprehensions

```python
# List
squares = [x*x for x in range(5)]

# Dictionary
d = {x: x*x for x in range(5)}

# Set
s = {x for x in [1,2,2,3]}
```

---

## 🔗 Lambda, Map, Filter, Reduce

```python
# Lambda
add = lambda x, y: x + y

# Map
list(map(lambda x: x*2, [1, 2, 3]))

# Filter
list(filter(lambda x: x % 2 == 0, [1, 2, 3]))

# Reduce
from functools import reduce
reduce(lambda x, y: x + y, [1, 2, 3])
```

---

## 🧪 Virtual Environments

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\\Scripts\\activate   # Windows
pip install -r requirements.txt
```

---

## 🔍 Debugging Tips

```python
# Built-in
print(variable)

# Using pdb
import pdb; pdb.set_trace()
```

---

## 📚 Useful Libraries

- `requests` – HTTP requests
- `re` – Regex
- `os` / `shutil` – File & OS operations
- `json` – JSON parsing
- `datetime` – Date/time handling
- `logging` – Logging system
- `argparse` – CLI argument parsing

---

## ❤️ Author

Cheatsheet by [@femonla02](https://github.com/femonla02)  
Last updated: August 2025
"""

# Save to file
file_path = "/mnt/data/python-cheatsheet.md"
with open(file_path, "w", encoding="utf-8") as f:
    f.write(cheatsheet_content)

file_path
