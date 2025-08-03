

## 📑 Table of Contents

- [🔤 Basic Syntax](#-basic-syntax)
- [📦 Data Types & Casting](#-data-types--casting)
- [🔁 Control Flow](#-control-flow)
- [🧮 Operators](#-operators)
- [🔧 Functions](#-functions)
- [🎒 Data Structures](#-data-structures)
- [🧱 Modules & Packages](#-modules--packages)
- [🗃️ File I/O](#-file-io)
- [🧵 Error Handling](#-error-handling)
- [🎭 Object-Oriented Programming (OOP)](#-object-oriented-programming-oop)
- [⏳ Comprehensions](#-comprehensions)
- [⚙️ Lambda, Map, Filter, Reduce](#-lambda-map-filter-reduce)
- [📦 Virtual Environments](#-virtual-environments)
- [🧪 Testing](#-testing)
- [🐞 Debugging](#-debugging)
- [📚 Standard Libraries](#-standard-libraries)
- [🔗 Recommended Third-Party Libraries](#-recommended-third-party-libraries)

---

## 🔤 Basic Syntax

```python
# Comments
# This is a comment
""" This is a
multi-line comment """

# Variables
name = "Alice"
age = 30
is_active = True

# Print
print(f"{name} is {age} years old")


---

📦 Data Types & Casting

# Primitives
str_var = "hello"
int_var = 42
float_var = 3.14
bool_var = False
none_var = None

# Type Casting
str(42), int("10"), float("3.5"), bool("")

# Check type
type(str_var)


---

🔁 Control Flow

# Conditional
if age > 18:
    print("Adult")
elif age == 18:
    print("Just 18")
else:
    print("Minor")

# Loops
for i in range(5):
    print(i)

while condition:
    break  # exit loop
    continue  # skip rest of this iteration


---

🧮 Operators

# Arithmetic
+, -, *, /, %, **, //

# Comparison
==, !=, <, >, <=, >=

# Logical
and, or, not

# Membership
in, not in

# Identity
is, is not


---

🔧 Functions

def greet(name: str = "Guest") -> str:
    return f"Hello, {name}"

# Lambda
square = lambda x: x ** 2


---

🎒 Data Structures

List

nums = [1, 2, 3]
nums.append(4)
nums[0]  # 1
nums[1:3]  # slice

Tuple

coords = (4, 5)
x, y = coords

Set

items = {1, 2, 2, 3}
items.add(4)

Dictionary

person = {"name": "Alice", "age": 30}
person["name"]
person.get("age", 0)


---

🧱 Modules & Packages

import math
from datetime import datetime as dt

print(math.sqrt(9))
print(dt.now())

# Create module
touch utils.py
# Import from file
from utils import some_function


---

🗃️ File I/O

# Write
with open("file.txt", "w") as f:
    f.write("Hello\n")

# Read
with open("file.txt", "r") as f:
    content = f.read()


---

🧵 Error Handling

try:
    result = 10 / 0
except ZeroDivisionError as e:
    print("Error:", e)
finally:
    print("Always runs")


---

🎭 Object-Oriented Programming (OOP)

class Person:
    def __init__(self, name: str):
        self.name = name

    def greet(self):
        return f"Hi, I'm {self.name}"

# Inheritance
class Student(Person):
    def greet(self):
        return super().greet() + " and I'm a student"

p = Person("Alice")
s = Student("Bob")


---

⏳ Comprehensions

# List
squares = [x ** 2 for x in range(10) if x % 2 == 0]

# Dictionary
d = {x: x ** 2 for x in range(5)}

# Set
unique = {x for x in [1, 2, 2, 3]}


---

⚙️ Lambda, Map, Filter, Reduce

# Lambda
multiply = lambda x, y: x * y

# Map
list(map(str.upper, ["a", "b", "c"]))

# Filter
list(filter(lambda x: x % 2 == 0, range(10)))

# Reduce
from functools import reduce
reduce(lambda x, y: x + y, [1, 2, 3])


---

📦 Virtual Environments

# Create
python -m venv venv

# Activate
source venv/bin/activate  # Linux/macOS
venv\\Scripts\\activate   # Windows

# Install packages
pip install -r requirements.txt


---

🧪 Testing

# test_sample.py
def add(a, b): return a + b

def test_add():
    assert add(2, 3) == 5

# Run tests
pytest test_sample.py


---

🐞 Debugging

# Print-based
print("DEBUG:", variable)

# Built-in
import pdb; pdb.set_trace()


---

📚 Standard Libraries

Library	Purpose

os	Files, paths, env
sys	CLI args, interpreter settings
math	Math operations
datetime	Time & date
json	JSON encoding/decoding
random	Randomness
logging	Logging
re	Regular expressions



---

🔗 Recommended Third-Party Libraries

Library	Purpose

requests	HTTP requests
pandas	Data manipulation
flask	Web apps
beautifulsoup4	HTML parsing
pytest	Testing
fastapi	Modern async web APIs
sqlalchemy	ORM for SQL
numpy	Scientific computing



---

👤 Author

Built by @
Licensed under MIT
Last Updated: August 2025

---

