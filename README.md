# Python Learning Roadmap

A comprehensive guide to learn Python from basics to advanced level.

## Table of Contents
1. [What is Python?](#what-is-python)
2. [Installing Python](#installing-python)
3. [Code Editors](#code-editors)
4. [Python Basics](#python-basics)
5. [Intermediate Python](#intermediate-python)
6. [Advanced Python](#advanced-python)
7. [Practice Resources](#practice-resources)

---

## What is Python?

Python is a high-level, interpreted programming language known for its readability and versatility. It supports multiple programming paradigms including procedural, object-oriented, and functional programming.

**Why Learn Python?**
- Easy to learn and read
- Versatile (Web, Data Science, AI, Automation, etc.)
- Large community and ecosystem
- High demand in job market

---

## Installing Python

### Windows
1. Download Python from [python.org](https://www.python.org/downloads/)
2. Run the installer
3. **Important:** Check "Add Python to PATH"
4. Open Command Prompt and verify:
   ```
   python --version
   ```

### macOS
1. Install Homebrew (if not installed):
   ```
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
2. Install Python:
   ```
   brew install python3
   ```
3. Verify:
   ```
   python3 --version
   ```

### Linux (Ubuntu/Debian)
```bash
sudo apt update
sudo apt install python3
python3 --version
```

### Using Anaconda (Data Science)
1. Download from [anaconda.com](https://www.anaconda.com/download)
2. Install and verify:
   ```
   conda --version
   ```

---

## Code Editors

### 1. VS Code (Recommended)
- **Download:** [code.visualstudio.com](https://code.visualstudio.com/)
- **Extensions to install:**
  - Python (Microsoft)
  - Python Indent
  - Pylance
  - Jupyter

### 2. PyCharm
- **Download:** [jetbrains.com/pycharm](https://www.jetbrains.com/pycharm/)
- Community Edition (Free) or Professional (Paid)

### 3. Jupyter Notebook
- Great for data science and experimentation
- Install via:
  ```
  pip install jupyter
  jupyter notebook
  ```

### 4. Sublime Text
- Lightweight editor
- Install Package Control and Python plugins

---

## Python Basics

### 1. Hello World
```python
print("Hello, World!")
```

### 2. Variables and Data Types
```python
# Numbers
age = 25          # int
price = 19.99     # float
complex_num = 3j  # complex

# Strings
name = "Python"
message = 'Hello'

# Boolean
is_active = True
is_done = False

# None
result = None
```

### 3. Basic Operators
```python
# Arithmetic
a, b = 10, 3
print(a + b)   # 13 (Addition)
print(a - b)   # 7  (Subtraction)
print(a * b)   # 30 (Multiplication)
print(a / b)   # 3.333... (Division)
print(a // b)  # 3  (Floor Division)
print(a % b)   # 1  (Modulus)
print(a ** b)  # 1000 (Exponent)

# Comparison
print(a == b)  # False
print(a != b)  # True
print(a > b)   # True
print(a < b)   # False

# Logical
x, y = True, False
print(x and y) # False
print(x or y)  # True
print(not x)   # False
```

### 4. Strings
```python
text = "Hello, Python!"

# Accessing characters
print(text[0])    # H
print(text[-1])   # !

# Slicing
print(text[0:5])   # Hello
print(text[7:])    # Python!

# String methods
print(text.upper())           # HELLO, PYTHON!
print(text.lower())           # hello, python!
print(text.replace("Python", "World"))  # Hello, World!
print(text.split(","))        # ['Hello', ' Python!']
print(len(text))             # 14
```

### 5. Lists
```python
fruits = ["apple", "banana", "cherry"]

# Access
print(fruits[0])    # apple
print(fruits[-1])   # cherry

# Modify
fruits.append("orange")
fruits.insert(1, "mango")
fruits.remove("banana")

# Slicing
print(fruits[1:3])

# List comprehension
squares = [x**2 for x in range(5)]  # [0, 1, 4, 9, 16]
```

### 6. Tuples
```python
coordinates = (10, 20, 30)
# Immutable - cannot change after creation
print(coordinates[0])  # 10
```

### 7. Dictionaries
```python
person = {
    "name": "John",
    "age": 30,
    "city": "New York"
}

# Access
print(person["name"])      # John
print(person.get("age"))   # 30

# Methods
print(person.keys())    # dict_keys(['name', 'age', 'city'])
print(person.values())  # dict_values(['John', 30, 'New York'])
print(person.items())   # dict_items([('name', 'John'), ('age', 30), ('city', 'New York')])
```

### 8. Sets
```python
numbers = {1, 2, 3, 4, 5}
# Unique values, unordered

# Operations
numbers.add(6)
numbers.update([7, 8])
numbers.remove(1)

# Set operations
set1 = {1, 2, 3}
set2 = {3, 4, 5}
print(set1 | set2)  # Union: {1, 2, 3, 4, 5}
print(set1 & set2)  # Intersection: {3}
print(set1 - set2)  # Difference: {1, 2}
```

### 9. Conditionals
```python
age = 18

if age < 13:
    print("Child")
elif age < 20:
    print("Teenager")
else:
    print("Adult")

# Ternary operator
status = "Adult" if age >= 18 else "Minor"
```

### 10. Loops
```python
# For loop
for i in range(5):
    print(i)  # 0, 1, 2, 3, 4

fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

# While loop
count = 0
while count < 5:
    print(count)
    count += 1

# Loop control
for i in range(10):
    if i == 3:
        continue  # Skip this iteration
    if i == 7:
        break     # Exit loop
    print(i)
```

### 11. Functions
```python
# Basic function
def greet(name):
    return f"Hello, {name}!"

# Default parameters
def greet(name, greeting="Hello"):
    return f"{greeting}, {name}!"

# Multiple parameters
def add(*args):
    return sum(args)

def person_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

# Lambda functions
square = lambda x: x ** 2
add = lambda a, b: a + b
```

### 12. File Handling
```python
# Read file
with open("file.txt", "r") as file:
    content = file.read()
    # or
    lines = file.readlines()

# Write file
with open("file.txt", "w") as file:
    file.write("Hello, World!")

# Append to file
with open("file.txt", "a") as file:
    file.write("\nNew line")
```

---

## Intermediate Python

### 1. Object-Oriented Programming (OOP)
```python
class Person:
    # Class attribute
    species = "Human"
    
    # Constructor
    def __init__(self, name, age):
        self.name = name    # Instance attribute
        self.age = age
    
    # Instance method
    def greet(self):
        return f"Hello, I'm {self.name}"
    
    # String representation
    def __str__(self):
        return f"Person({self.name}, {self.age})"
    
    # Private method
    def _private_method(self):
        print("Private method")

# Inheritance
class Student(Person):
    def __init__(self, name, age, grade):
        super().__init__(name, age)
        self.grade = grade
    
    def greet(self):
        return f"Hi, I'm {self.name} and I'm in grade {self.grade}"

# Create object
person = Person("John", 30)
student = Student("Alice", 20, 10)

# Access attributes
print(person.name)
print(Student.species)
```

### 2. Exception Handling
```python
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")
except Exception as e:
    print(f"Error: {e}")
else:
    print("No errors occurred")
finally:
    print("This always executes")

# Raising exceptions
def divide(a, b):
    if b == 0:
        raise ValueError("Divisor cannot be zero")
    return a / b

# Custom exception
class CustomError(Exception):
    pass
```

### 3. Modules and Packages
```python
# Import module
import math
print(math.sqrt(16))

# Import specific function
from math import sqrt, pi

# Import with alias
import numpy as np
from datetime import datetime as dt

# Create your own module
# mymodule.py
def my_function():
    return "Hello"

# Use it
import mymodule
```

### 4. List/Dict/Set Comprehensions
```python
# List comprehension
numbers = [1, 2, 3, 4, 5]
squares = [x**2 for x in numbers]
evens = [x for x in numbers if x % 2 == 0]

# Dictionary comprehension
dict1 = {x: x**2 for x in range(5)}

# Set comprehension
set1 = {x**2 for x in range(5)}
```

### 5. Generators
```python
def count_up_to(n):
    i = 1
    while i <= n:
        yield i
        i += 1

# Using generator
counter = count_up_to(5)
print(next(counter))  # 1
print(next(counter))  # 2

# Generator expression
gen = (x**2 for x in range(5))
```

### 6. Decorators
```python
def my_decorator(func):
    def wrapper():
        print("Before")
        func()
        print("After")
    return wrapper

@my_decorator
def say_hello():
    say_hello()  # Before\nHello\nAfter

# Decorator with arguments
def repeat(times):
    def decorator(func):
        def wrapper(*args, **kwargs):
            for _ in range(times):
                result = func(*args, **kwargs)
            return result
        return wrapper
    return decorator

@repeat(times=3)
def greet():
    print("Hello!")
```

### 7. Context Managers
```python
# Using with statement
with open("file.txt", "r") as f:
    content = f.read()
# File automatically closed

# Custom context manager
class MyContext:
    def __enter__(self):
        print("Enter")
        return self
    
    def __exit__(self, exc_type, exc_val, exc_tb):
        print("Exit")

with MyContext() as ctx:
    print("Inside context")
```

### 8. Working with JSON
```python
import json

# Convert to JSON
data = {"name": "John", "age": 30}
json_str = json.dumps(data)

# Convert from JSON
parsed = json.loads(json_str)

# Read from file
with open("data.json", "r") as f:
    data = json.load(f)

# Write to file
with open("data.json", "w") as f:
    json.dump(data, f, indent=4)
```

### 9. Working with CSV
```python
import csv

# Read CSV
with open("data.csv", "r") as f:
    reader = csv.reader(f)
    for row in reader:
        print(row)

# Write CSV
with open("data.csv", "w", newline="") as f:
    writer = csv.writer(f)
    writer.writerow(["Name", "Age"])
    writer.writerow(["John", "30"])
```

### 10. Virtual Environments
```bash
# Create virtual environment
python -m venv myenv

# Activate (Windows)
myenv\Scripts\activate

# Activate (Mac/Linux)
source myenv/bin/activate

# Install packages
pip install package_name

# Deactivate
deactivate

# Create requirements.txt
pip freeze > requirements.txt

# Install from requirements.txt
pip install -r requirements.txt
```

---

## Advanced Python

### 1. Advanced OOP Concepts
```python
# Multiple Inheritance
class A:
    def method(self):
        print("A")

class B:
    def method(self):
        print("B")

class C(A, B):
    pass

# MRO (Method Resolution Order)
print(C.__mro__)

# Abstract Base Classes
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def sound(self):
        pass
    
    def common(self):
        print("All animals breathe")

class Dog(Animal):
    def sound(self):
        return "Woof!"

# Metaclasses
class Meta(type):
    def __new__(cls, name, bases, dict):
        dict['added_attribute'] = 'Hello'
        return type.__new__(cls, name, bases, dict)

class MyClass(metaclass=Meta):
    pass
```

### 2. Advanced Decorators
```python
# Class as decorator
class Decorator:
    def __init__(self, func):
        self.func = func
    
    def __call__(self, *args, **kwargs):
        print("Before")
        result = self.func(*args, **kwargs)
        print("After")
        return result

@Decorator
def func():
    print("Function")

# Stacked decorators
@decorator1
@decorator2
def func():
    pass
```

### 3. Async Programming
```python
import asyncio

async def fetch_data():
    print("Fetching data...")
    await asyncio.sleep(2)
    return {"data": 123}

async def main():
    # Sequential
    result1 = await fetch_data()
    result2 = await fetch_data()
    
    # Concurrent
    results = await asyncio.gather(
        fetch_data(),
        fetch_data()
    )

asyncio.run(main())
```

### 4. Multithreading
```python
import threading

def worker(number):
    print(f"Thread {number} is working")

threads = []
for i in range(5):
    t = threading.Thread(target=worker, args=(i,))
    threads.append(t)
    t.start()

for t in threads:
    t.join()

# Using ThreadPoolExecutor
from concurrent.futures import ThreadPoolExecutor

with ThreadPoolExecutor(max_workers=5) as executor:
    executor.map(worker, range(5))
```

### 5. Multiprocessing
```python
import multiprocessing

def worker(number):
    print(f"Process {number} is working")

if __name__ == "__main__":
    processes = []
    for i in range(5):
        p = multiprocessing.Process(target=worker, args=(i,))
        processes.append(p)
        p.start()

    for p in processes:
        p.join()
```

### 6. Type Hints
```python
def greet(name: str) -> str:
    return f"Hello, {name}!"

def process_items(items: list[int]) -> dict[str, int]:
    return {"sum": sum(items)}

from typing import Union, Optional, Callable

def func(arg: Optional[str] = None) -> Union[str, int]:
    pass

def high_order_func(func: Callable[[int], int]) -> int:
    return func(10)
```

### 7. Dataclasses
```python
from dataclasses import dataclass, field

@dataclass
class Person:
    name: str
    age: int
    email: str = "unknown@example.com"
    
    def __post_init__(self):
        if self.age < 0:
            raise ValueError("Age cannot be negative")

person = Person("John", 30)
print(person)
```

### 8. Enums
```python
from enum import Enum

class Color(Enum):
    RED = 1
    GREEN = 2
    BLUE = 3

print(Color.RED.name)    # RED
print(Color.RED.value)   # 1
```

### 9. Working with Databases
```python
import sqlite3

# Create database
conn = sqlite3.connect("database.db")
cursor = conn.cursor()

# Create table
cursor.execute("""
    CREATE TABLE users (
        id INTEGER PRIMARY KEY,
        name TEXT,
        email TEXT
    )
""")

# Insert data
cursor.execute("INSERT INTO users (name, email) VALUES (?, ?)", ("John", "john@example.com"))
conn.commit()

# Select data
cursor.execute("SELECT * FROM users")
rows = cursor.fetchall()

# Update data
cursor.execute("UPDATE users SET name = ? WHERE id = ?", ("Jane", 1))
conn.commit()

# Delete data
cursor.execute("DELETE FROM users WHERE id = ?", (1,))
conn.commit()

conn.close()
```

### 10. Testing
```python
# Using unittest
import unittest

class TestMathOperations(unittest.TestCase):
    def test_add(self):
        self.assertEqual(1 + 1, 2)
    
    def test_divide(self):
        with self.assertRaises(ZeroDivisionError):
            1 / 0

if __name__ == "__main__":
    unittest.main()

# Using pytest
# Install: pip install pytest
def test_add():
    assert 1 + 1 == 2
```

---

## Practice Resources

### Online Platforms
- [LeetCode](https://leetcode.com/) - Coding challenges
- [HackerRank](https://www.hackerrank.com/) - Practice problems
- [Codewars](https://www.codewars.com/) - Kata challenges
- [Project Euler](https://projecteuler.net/) - Math/Programming problems
- [Real Python](https://realpython.com/) - Tutorials
- [W3Schools Python](https://www.w3schools.com/python/) - Basics
- [Python.org Docs](https://docs.python.org/3/) - Official documentation

### Practice Projects
1. **Beginner:** Calculator, To-Do List, Guess the Number
2. **Intermediate:** Weather App, REST API, Web Scraper
3. **Advanced:** Machine Learning Model, Full-stack Web App, Automation Script

### Recommended Learning Path
```
Week 1-2:   Basic syntax, variables, data types
Week 3-4:   Control flow, functions
Week 5-6:   Data structures
Week 7-8:   OOP concepts
Week 9-10:  File handling, modules
Week 11-12: Intermediate topics (decorators, generators)
Week 13-16: Advanced topics (async, databases, testing)
Week 17+:   Specialize in your chosen field
```

---

## Contributing

Feel free to contribute to this roadmap by submitting a pull request!

---

## License

MIT License
