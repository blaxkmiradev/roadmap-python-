# 🐍 Python Learning Roadmap

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python Version">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License">
  <img src="https://img.shields.io/badge/Contributions-Welcome-blue.svg" alt="Contributions">
</p>

> A comprehensive, structured roadmap for learning Python from zero to hero 🎯

---

## 📋 Table of Contents

1. [Roadmap Overview Diagram](#-roadmap-overview-diagram)
2. [What is Python?](#what-is-python)
3. [Setting Up Your Environment](#setting-up-your-environment)
4. [Python Fundamentals](#python-fundamentals)
5. [Intermediate Python](#intermediate-python)
6. [Advanced Python](#advanced-python)
7. [Python for Data Science](#python-for-data-science)
8. [Python for Web Development](#python-for-web-development)
9. [Python for Automation & Scripting](#python-for-automation--scripting)
10. [Career Paths](#career-paths)
11. [Practice Resources](#practice-resources)
12. [Project Ideas](#project-ideas)

---

## 🗺️ Roadmap Overview Diagram

```
┌─────────────────────────────────────────────────────────────────────────────────────────────┐
│                                    PYTHON LEARNING ROADMAP                                  │
└─────────────────────────────────────────────────────────────────────────────────────────────┘

    ┌─────────────┐     ┌─────────────┐     ┌─────────────┐     ┌─────────────┐
    │   BASICS    │────▶│ INTERMEDIATE│────▶│   ADVANCED  │────▶│  SPECIALIZE │
    └─────────────┘     └─────────────┘     └─────────────┘     └─────────────┘
          │                   │                   │                   │
    ┌─────┴─────┐       ┌─────┴─────┐       ┌─────┴─────┐       ┌─────┴─────┐
    │           │       │           │       │           │       │           │
┌───┴───┐   ┌───┴───┐ ┌───┴───┐   ┌───┴───┐ ┌───┴───┐   ┌───┴───┐ ┌───┴───┐
│Syntax │   │  OOP  ││  Web  │   │ Async ││  ML   │   │  DevOps││ Career│
│ Vars  │   │  DB   ││  API  │   │Thread ││  AI   │   │  Cloud││       │
│ Types │   │  API  ││  ORM  │   │Testing││  DS   │   │       ││       │
└───────┘   └───────┘└───────┘   └───────┘└───────┘   └───────┘└───────┘


    ╔═══════════════════════════════════════════════════════════════════════════════════════╗
    ║                           LEARNING PHASES (Detailed)                                   ║
    ╠═══════════════════════════════════════════════════════════════════════════════════════╣
    ║                                                                                        ║
    ║  PHASE 1: FUNDAMENTALS (Weeks 1-4)                                                     ║
    ║  ├── Hello World & Print Statements                                                    ║
    ║  ├── Variables & Data Types (int, float, str, bool, None)                            ║
    ║  ├── Operators (arithmetic, comparison, logical)                                      ║
    ║  ├── Strings & String Formatting                                                      ║
    ║  ├── Lists, Tuples, Sets, Dictionaries                                               ║
    ║  ├── Conditionals (if/elif/else)                                                      ║
    ║  ├── Loops (for, while)                                                               ║
    ║  ├── Functions & Lambda Expressions                                                  ║
    ║  └── File I/O Operations                                                              ║
    ║                                                                                        ║
    ║  PHASE 2: INTERMEDIATE (Weeks 5-8)                                                    ║
    ║  ├── Object-Oriented Programming (Classes, Objects, Inheritance)                    ║
    ║  ├── Exception Handling                                                              ║
    ║  ├── Modules & Packages                                                               ║
    ║  ├── Virtual Environments                                                            ║
    ║  ├── Decorators                                                                       ║
    ║  ├── Generators                                                                      ║
    ║  ├── List/Dict/Set Comprehensions                                                    ║
    ║  ├── Working with JSON & CSV                                                          ║
    ║  └── Context Managers                                                                 ║
    ║                                                                                        ║
    ║  PHASE 3: ADVANCED (Weeks 9-12)                                                      ║
    ║  ├── Advanced OOP (Metaclasses, ABC, Multiple Inheritance)                          ║
    ║  ├── Async Programming (asyncio)                                                      ║
    ║  ├── Multithreading & Multiprocessing                                                ║
    ║  ├── Type Hints & Static Analysis                                                     ║
    ║  ├── Database Programming (SQL, NoSQL)                                               ║
    ║  ├── Testing (unittest, pytest)                                                       ║
    ║  ├── Design Patterns                                                                  ║
    ║  └── Performance Optimization                                                         ║
    ║                                                                                        ║
    ║  PHASE 4: SPECIALIZATION (Weeks 13+)                                                 ║
    ║  ├── Data Science & Machine Learning                                                  ║
    ║  ├── Web Development                                                                  ║
    ║  ├── Automation & Scripting                                                           ║
    ║  ├── API Development                                                                  ║
    ║  └── DevOps & Cloud                                                                    ║
    ║                                                                                        ║
    ╚═══════════════════════════════════════════════════════════════════════════════════════╝


    ╔═══════════════════════════════════════════════════════════════════════════════════════╗
    ║                        PYTHON ECOSYSTEM OVERVIEW                                       ║
    ╠═══════════════════════════════════════════════════════════════════════════════════════╣
    ║                                                                                        ║
    ║                              ┌─────────────────┐                                      ║
    ║                              │   PYTHON CORE   │                                      ║
    ║                              └────────┬────────┘                                      ║
    ║                                       │                                               ║
    ║         ┌──────────────────────────────┼──────────────────────────────┐               ║
    ║         │                              │                              │               ║
    ║    ┌────┴────┐                   ┌────┴────┐                   ┌────┴────┐           ║
    ║    │  WEB    │                   │   DATA  │                   │   DEV   │           ║
    ║    │ FRAMEWORKS                  │   SCIENCE│                  │   OPS   │           ║
    ║    ├─────────┤                   ├─────────┤                   ├─────────┤           ║
    ║    │ Django  │                   │ NumPy    │                   │ Docker  │           ║
    ║    │ Flask   │                   │ Pandas   │                   │ Kube    │           ║
    ║    │ FastAPI │                   │ Matplotlib│                  │ Terraform│          ║
    ║    │ Pyramid │                   │ Scikit   │                   │Ansible  │           ║
    ║    └─────────┘                   └─────────┘                   └─────────┘           ║
    ║                                                                                        ║
    ║    ┌─────────────────┐         ┌─────────────────┐         ┌─────────────────┐         ║
    ║    │ AUTOMATION      │         │   AI/ML         │         │   TESTING      │         ║
    ║    ├─────────────────┤         ├─────────────────┤         ├─────────────────┤         ║
    ║    │ Selenium        │         │ TensorFlow      │         │   pytest       │         ║
    ║    │ BeautifulSoup   │         │ PyTorch         │         │   unittest     │         ║
    ║    │ Scrapy          │         │ Keras           │         │   coverage     │         ║
    ║    │ Pillow         │         │ OpenCV          │         │   tox          │         ║
    ║    └─────────────────┘         └─────────────────┘         └─────────────────┘         ║
    ║                                                                                        ║
    ╚═══════════════════════════════════════════════════════════════════════════════════════╝
```

---

## 🔰 What is Python?

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg" width="150" alt="Python Logo">
</p>

Python is a **high-level, interpreted** programming language known for its:

| Feature | Description |
|---------|-------------|
| **Easy to Learn** | Clean syntax that reads like English |
| **Versatile** | Used in Web, Data Science, AI, Automation, and more |
| **Interpreted** | No compilation needed - runs line by line |
| **Multi-paradigm** | Supports OOP, Functional, and Procedural programming |
| **Cross-platform** | Works on Windows, macOS, Linux |
| **Huge Ecosystem** | 400,000+ packages available |

### Why Learn Python in 2025/2026?

```
┌─────────────────────────────────────────────────────────────────┐
│                    PYTHON POPULARITY                             │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│  📊 TIOBE Index: #1 (Most Popular Programming Language)        │
│                                                                  │
│  📈 Stack Overflow: Most Loved Language (6 years running)      │
│                                                                  │
│  💼 Job Market: High Demand with Competitive Salaries          │
│                                                                  │
│  🌐 Usage: Google, NASA, Netflix, Instagram, Spotify, NASA    │
│                                                                  │
│  🔬 Research: #1 Language in Data Science & Machine Learning   │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

---

## ⚙️ Setting Up Your Environment

### Installing Python

#### Windows
```powershell
# Method 1: Download from python.org
# Go to https://www.python.org/downloads/
# Download the latest version
# IMPORTANT: Check "Add Python to PATH"

# Method 2: Using Microsoft Store
python --version

# Verify Installation
python --version
pip --version
```

#### macOS
```bash
# Method 1: Using Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install python3

# Method 2: Download from python.org
# Go to https://www.python.org/downloads/mac-osx/

# Verify
python3 --version
pip3 --version
```

#### Linux (Ubuntu/Debian)
```bash
sudo apt update
sudo apt install python3 python3-pip python3-venv

# Verify
python3 --version
pip3 --version
```

#### Using Anaconda (Data Science)
```bash
# Download from https://www.anaconda.com/download
# Or use Miniconda (lightweight)
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh

# Verify
conda --version
```

---

### Code Editors & IDEs

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                              CODE EDITOR COMPARISON                                      │
├───────────────┬──────────────┬──────────────┬──────────────┬────────────────────────────┤
│    Editor     │    Type      │   License    │   Best For   │        Pros/Cons           │
├───────────────┼──────────────┼──────────────┼──────────────┼────────────────────────────┤
│  VS Code      │    IDE       │   Free       │ General      │ + Lightweight, Extensions   │
│               │              │              │  Development │ + Great Python Support      │
│               │              │              │              │ - Electron-based            │
├───────────────┼──────────────┼──────────────┼──────────────┼────────────────────────────┤
│   PyCharm     │    IDE       │ Comm (Free)  │ Large        │ + Full-Featured            │
│               │              │ Prof (Paid)  │  Projects    │ + Best Autocomplete        │
│               │              │              │              │ - Heavy on Resources        │
├───────────────┼──────────────┼──────────────┼──────────────┼────────────────────────────┤
│  Jupyter      │  Notebook    │   Free       │ Data Science │ + Great for Experiments    │
│   Notebook    │              │              │ & ML         │ + Interactive              │
│               │              │              │              │ - Not for Large Projects    │
├───────────────┼──────────────┼──────────────┼──────────────┼────────────────────────────┤
│   Sublime     │   Editor     │   Paid       │ Quick        │ + Extremely Fast           │
│   Text        │              │              │  Editing     │ + Minimalist               │
│               │              │              │              │ - Limited Python Support   │
├───────────────┼──────────────┼──────────────┼──────────────┼────────────────────────────┤
│    Vim        │   Editor     │   Free       │ Terminal     │ + Power User's Choice      │
│               │              │              │  Users       │ + Everywhere               │
│               │              │              │              │ - Steep Learning Curve     │
└───────────────┴──────────────┴──────────────┴──────────────┴────────────────────────────┘
```

### VS Code Setup (Recommended)

```bash
# 1. Download VS Code
# https://code.visualstudio.com/

# 2. Install Python Extension
# Open VS Code > Extensions (Ctrl+Shift+X) > Search "Python"

# 3. Essential Extensions
code --install-extension ms-python.python
code --install-extension ms-python.vscode-pylance
code --install-extension ms-toolsai.jupyter
code --install-extension ms-python.black-formatter

# 4. Configure Python Interpreter
# Ctrl+Shift+P > Python: Select Interpreter
```

### Virtual Environments

```bash
# Create virtual environment
python -m venv myenv

# Activate (Windows)
myenv\Scripts\activate

# Activate (Mac/Linux)
source myenv/bin/activate

# Install packages
pip install package_name
pip install -r requirements.txt

# Create requirements.txt
pip freeze > requirements.txt

# Deactivate
deactivate
```

---

## 📚 Python Fundamentals

### 1. Hello World

```python
# The classic first program
print("Hello, World!")

# Multiple prints
print("Hello")
print("World")

# Print with variables
name = "Python"
print(f"Hello, {name}!")

# Print with formatting
print("Hello, {}!".format(name))
print("Hello, %s!" % name)
```

### 2. Variables & Data Types

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                             PYTHON DATA TYPES                                            │
├─────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                          │
│  ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐                  │
│  │    NUMERIC      │     │     STRING       │     │    BOOLEAN      │                  │
│  ├─────────────────┤     ├─────────────────┤     ├─────────────────┤                  │
│  │  int    → 42    │     │  str  → "Hello"  │     │  bool → True    │                  │
│  │  float  → 3.14  │     │  str  → 'Python' │     │  bool → False   │                  │
│  │  complex→ 3+4j │     │  str  → """Multi │     │                 │                  │
│  └─────────────────┘     │       line str  │     └─────────────────┘                  │
│                          │       """       │                                         │
│                          └─────────────────┘                                         │
│                                                                                          │
│  ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐                  │
│  │    SEQUENCE     │     │     MAPPING     │     │     SET         │                  │
│  ├─────────────────┤     ├─────────────────┤     ├─────────────────┤                  │
│  │  list  → [1,2]  │     │ dict → {a:1}    │     │ set → {1,2,3}    │                  │
│  │  tuple → (1,2)  │     │                 │     │ frozenset      │                  │
│  │  range → range │     │                 │     │                 │                  │
│  └─────────────────┘     └─────────────────┘     └─────────────────┘                  │
│                                                                                          │
│  ┌─────────────────┐                                                                     │
│  │     NONE        │                                                                     │
│  ├─────────────────┤                                                                     │
│  │  NoneType→None  │                                                                     │
│  └─────────────────┘                                                                     │
│                                                                                          │
└─────────────────────────────────────────────────────────────────────────────────────────┘
```

```python
# Numbers
age = 25              # int
price = 19.99         # float
complex_num = 3j      # complex

# Strings
name = "Python"
message = 'Hello'
multi_line = """This is
a multi-line
string"""

# Boolean
is_active = True
is_done = False

# None
result = None

# Checking types
print(type(age))      # <class 'int'>
print(type(name))     # <class 'str'>
print(type(is_active))# <class 'bool'>

# Type conversion
int_to_float = float(10)
float_to_int = int(10.5)
str_to_int = int("42")
num_to_str = str(123)
```

### 3. Operators

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                              OPERATORS OVERVIEW                                         │
├─────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                          │
│  ARITHMETIC OPERATORS                    COMPARISON OPERATORS                            │
│  ═════════════════════                    ════════════════                              │
│  +   Addition           a + b = 13        ==  Equal             a == b                 │
│  -   Subtraction        a - b = 7         !=  Not Equal         a != b                 │
│  *   Multiplication    a * b = 30        >   Greater Than      a > b                  │
│  /   Division           a / b = 3.33     <   Less Than          a < b                  │
│  //  Floor Division     a // b = 3       >=  Greater/Equal      a >= b                 │
│  %   Modulus            a % b = 1        <=  Less/Equal         a <= b                 │
│  **  Exponent           a ** b = 1000                                                 │
│                                                                                          │
│  LOGICAL OPERATORS                      ASSIGNMENT OPERATORS                           │
│  ════════════════                       ══════════════                                 │
│  and  True if both True    x and y      =    Assign            a = 10                 │
│  or   True if either True  x or y       +=   Add & Assign      a += 5 (a = a + 5)    │
│  not  Inverts boolean      not x         -=   Subtract & Assign a -= 5                │
│                                           *=   Multiply & Assign  a *= 5                │
│  IDENTITY OPERATORS                     /=   Divide & Assign    a /= 5                │
│  ════════════════                                                                     │
│  is   True if same object  x is y       //=  Floor Div & Assign a //= 5               │
│  is not True if not same    x is not y   %=   Modulus & Assign   a %= 5                │
│                                           **=  Exponent & Assign  a **= 5               │
│  MEMBERSHIP OPERATORS                                                                       │
│  ════════════════                                                                     │
│  in    True if in        x in list                                                 │
│  not in True if not in   x not in list                                              │
└─────────────────────────────────────────────────────────────────────────────────────────┘
```

```python
# Arithmetic
a, b = 10, 3
print(a + b)    # 13
print(a - b)    # 7
print(a * b)    # 30
print(a / b)    # 3.333...
print(a // b)   # 3
print(a % b)    # 1
print(a ** b)   # 1000

# Comparison
print(a == b)   # False
print(a != b)   # True
print(a > b)    # True

# Logical
x, y = True, False
print(x and y)  # False
print(x or y)   # True
print(not x)    # False

# Identity
list1 = [1, 2]
list2 = [1, 2]
list3 = list1
print(list1 is list2)    # False
print(list1 is list3)     # True
```

### 4. Strings

```python
text = "Hello, Python!"

# Accessing
print(text[0])           # H
print(text[-1])          # !

# Slicing
print(text[0:5])          # Hello
print(text[7:])          # Python!
print(text[::2])         # Hlo Ptno (every 2nd char)

# Methods
print(text.upper())                    # HELLO, PYTHON!
print(text.lower())                    # hello, python!
print(text.replace("Python", "World")) # Hello, World!
print(text.split(","))                 # ['Hello', ' Python!']
print(text.strip())                    # Remove whitespace
print(text.find("Python"))             # 7
print("Python" in text)                # True

# F-strings (recommended)
name = "Alice"
age = 30
print(f"My name is {name} and I'm {age} years old")
print(f"Price: ${price:.2f}")           # Formatted: Price: $19.99
print(f"Hex: {255:#x}")                 # Hex: 0xff
```

### 5. Collections

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                           COLLECTIONS COMPARISON                                        │
├──────────────┬─────────────┬──────────────┬─────────────┬─────────────────────────────┤
│   Feature    │    List     │    Tuple     │     Set     │        Dictionary           │
├──────────────┼─────────────┼──────────────┼─────────────┼─────────────────────────────┤
│  Ordered     │    ✅       │      ✅      │     ❌      │           ✅ (3.7+)         │
│  Mutable     │    ✅       │      ❌      │     ✅      │           ✅                 │
│  Indexed     │    ✅       │      ✅      │     ❌      │          By Key              │
│  Duplicates  │    ✅       │      ✅      │     ❌      │           ❌ (keys)         │
│  Syntax      │   [1,2,3]   │   (1,2,3)    │   {1,2,3}   │        {a:1, b:2}           │
│  Use Case    │  Sequence  │  Fixed data  │  Unique     │        Key-Value Pairs        │
└──────────────┴─────────────┴──────────────┴─────────────┴─────────────────────────────┘
```

```python
# LIST - Mutable, ordered sequence
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
fruits.insert(1, "mango")
fruits.remove("banana")
fruits.pop()
print(fruits[0])
print(fruits[-1])

# TUPLE - Immutable, ordered sequence
coordinates = (10, 20, 30)
print(coordinates[0])  # 10

# SET - Unordered, unique elements
numbers = {1, 2, 3, 4, 5}
numbers.add(6)
numbers.update([7, 8])
numbers.remove(1)
print({1, 2, 3} | {3, 4, 5})  # Union: {1, 2, 3, 4, 5}
print({1, 2, 3} & {3, 4, 5})  # Intersection: {3}

# DICTIONARY - Key-value pairs
person = {"name": "John", "age": 30, "city": "NYC"}
print(person["name"])
print(person.get("age"))
person["email"] = "john@example.com"
print(person.keys())
print(person.values())
print(person.items())
```

### 6. Control Flow

```python
# CONDITIONAL STATEMENTS
age = 18

if age < 13:
    print("Child")
elif age < 20:
    print("Teenager")
else:
    print("Adult")

# Ternary operator
status = "Adult" if age >= 18 else "Minor"

# MATCH STATEMENT (Python 3.10+)
status = "active"
match status:
    case "active":
        print("Running")
    case "paused":
        print("Paused")
    case _:
        print("Unknown")
```

```python
# FOR LOOP
for i in range(5):              # 0, 1, 2, 3, 4
    print(i)

fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

# With enumerate
for index, fruit in enumerate(fruits):
    print(f"{index}: {fruit}")

# WHILE LOOP
count = 0
while count < 5:
    print(count)
    count += 1

# LOOP CONTROL
for i in range(10):
    if i == 3:
        continue    # Skip this iteration
    if i == 7:
        break       # Exit loop
    print(i)
```

### 7. Functions

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

# Higher-order functions
numbers = [1, 2, 3, 4, 5]
squares = list(map(lambda x: x**2, numbers))
evens = list(filter(lambda x: x % 2 == 0, numbers))

# Decorators
def my_decorator(func):
    def wrapper(*args, **kwargs):
        print("Before function")
        result = func(*args, **kwargs)
        print("After function")
        return result
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")
```

### 8. File Operations

```python
# Read file
with open("file.txt", "r") as f:
    content = f.read()
    lines = f.readlines()

# Write file
with open("file.txt", "w") as f:
    f.write("Hello, World!")

# Append to file
with open("file.txt", "a") as f:
    f.write("\nNew line")

# Read CSV
import csv
with open("data.csv", "r") as f:
    reader = csv.reader(f)
    for row in reader:
        print(row)

# Work with JSON
import json
data = {"name": "John", "age": 30}
json_str = json.dumps(data)
parsed = json.loads(json_str)
```

---

## 🚀 Intermediate Python

### 1. Object-Oriented Programming

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                              OOP CONCEPTS                                               │
├─────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                          │
│     ┌──────────────────────┐                                                           │
│     │       CLASS          │  Blueprint for creating objects                            │
│     │  (Blueprint)         │  - Defines attributes (data)                               │
│     └──────────┬───────────┘  - Defines methods (behavior)                             │
│                │                                                                   │
│                │ creates                                                               │
│                ▼                                                                   │
│     ┌──────────────────────┐                                                           │
│     │       OBJECT         │  Instance of a class                                      │
│     │    (Instance)        │  - Has its own state (attributes)                         │
│     └──────────────────────┘  - Can perform actions (methods)                          │
│                                                                                          │
│  ┌─────────────────────────────────────────────────────────────────────────────────┐   │
│  │                           OOP PRINCIPLES                                          │   │
│  ├─────────────────────────────────────────────────────────────────────────────────┤   │
│  │                                                                                  │   │
│  │  1. ENCAPSULATION     →  Bundling data + methods together                       │   │
│  │  2. INHERITANCE       →  Reusing code from parent class                          │   │
│  │  3. POLYMORPHISM      →  Same interface, different implementations              │   │
│  │  4. ABSTRACTION       →  Hiding complex implementation                          │   │
│  │                                                                                  │   │
│  └─────────────────────────────────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────────────────────────────────┘
```

```python
# Class Definition
class Person:
    # Class attribute
    species = "Human"
    
    # Constructor
    def __init__(self, name, age):
        self.name = name        # Instance attribute
        self.age = age
    
    # Instance method
    def greet(self):
        return f"Hello, I'm {self.name}"
    
    # String representation
    def __str__(self):
        return f"Person({self.name}, {self.age})"
    
    def __repr__(self):
        return f"Person(name='{self.name}', age={self.age})"
    
    # Private method
    def _private_method(self):
        return "Private"

# Inheritance
class Student(Person):
    def __init__(self, name, age, grade):
        super().__init__(name, age)
        self.grade = grade
    
    def greet(self):
        return f"Hi, I'm {self.name} in grade {self.grade}"

# Create objects
person = Person("John", 30)
student = Student("Alice", 20, 10)

# Access
print(person.name)
print(person.greet())
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

### 3. Modules & Packages

```python
# Standard library modules
import math
import datetime
import random
import os
import sys

# Third-party modules
# pip install package_name
import numpy as np
import pandas as pd

# Create your own module
# mymodule.py
def my_function():
    return "Hello"

# Use it
import mymodule
mymodule.my_function()

# Import with alias
from datetime import datetime as dt
from math import sqrt, pi
```

### 4. Advanced Features

```python
# List comprehension
squares = [x**2 for x in range(5)]
evens = [x for x in range(10) if x % 2 == 0]

# Dictionary comprehension
dict1 = {x: x**2 for x in range(5)}

# Generator
def count_up_to(n):
    i = 1
    while i <= n:
        yield i
        i += 1

counter = count_up_to(5)
print(next(counter))  # 1

# Generator expression
gen = (x**2 for x in range(5))

# Context manager
with open("file.txt", "r") as f:
    content = f.read()
# File automatically closed
```

---

## 🦾 Advanced Python

### 1. Advanced OOP

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

# Method Resolution Order
print(C.__mro__)

# Abstract Base Classes
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def sound(self):
        pass

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

### 2. Async Programming

```python
import asyncio

async def fetch_data():
    print("Fetching data...")
    await asyncio.sleep(2)
    return {"data": 123}

async def main():
    # Sequential
    result1 = await fetch_data()
    
    # Concurrent
    results = await asyncio.gather(
        fetch_data(),
        fetch_data()
    )

asyncio.run(main())
```

### 3. Multithreading & Multiprocessing

```python
# Threading
import threading

def worker(number):
    print(f"Thread {number}")

threads = []
for i in range(5):
    t = threading.Thread(target=worker, args=(i,))
    threads.append(t)
    t.start()

for t in threads:
    t.join()

# Multiprocessing
import multiprocessing

def worker(number):
    print(f"Process {number}")

if __name__ == "__main__":
    with multiprocessing.Pool(5) as p:
        p.map(worker, range(5))
```

### 4. Type Hints

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

### 5. Database Programming

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

# CRUD Operations
cursor.execute("INSERT INTO users (name, email) VALUES (?, ?)", ("John", "john@example.com"))
cursor.execute("SELECT * FROM users")
rows = cursor.fetchall()
cursor.execute("UPDATE users SET name = ? WHERE id = ?", ("Jane", 1))
cursor.execute("DELETE FROM users WHERE id = ?", (1,))

conn.commit()
conn.close()

# Using SQLAlchemy (ORM)
from sqlalchemy import create_engine
from sqlalchemy.orm import sessionmaker
```

### 6. Testing

```python
# unittest
import unittest

class TestMathOperations(unittest.TestCase):
    def test_add(self):
        self.assertEqual(1 + 1, 2)
    
    def test_divide(self):
        with self.assertRaises(ZeroDivisionError):
            1 / 0

if __name__ == "__main__":
    unittest.main()

# pytest (install: pip install pytest)
def test_add():
    assert 1 + 1 == 2
```

---

## 📊 Python for Data Science

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                         DATA SCIENCE TOOLKIT                                             │
├─────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                          │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐                   │
│  │   NumPy     │  │   Pandas    │  │  Matplotlib │  │   Seaborn   │                   │
│  │  Numerical  │  │  Data       │  │  Plotting   │  │  Statistical│                   │
│  │  Computing  │  │  Analysis   │  │             │  │  Plotting   │                   │
│  └─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘                   │
│                                                                                          │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐                   │
│  │ Scikit-learn│  │  TensorFlow │  │   PyTorch   │  │   Keras    │                   │
│  │   ML       │  │    Deep     │  │    Deep    │  │   High     │                   │
│  │  Library   │  │   Learning  │  │   Learning  │  │   Level API│                   │
│  └─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘                   │
│                                                                                          │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐                   │
│  │  OpenCV    │  │   NLTK     │  │  Spacy     │  │  Plotly    │                   │
│  │  Computer │  │  NLP       │  │  NLP       │  │  Interactive│                   │
│  │  Vision    │  │            │  │            │  │  Charts    │                   │
│  └─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘                   │
│                                                                                          │
└─────────────────────────────────────────────────────────────────────────────────────────┘
```

### Installation
```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow keras torch
```

### NumPy Example
```python
import numpy as np

# Create arrays
arr = np.array([1, 2, 3, 4, 5])
matrix = np.array([[1, 2], [3, 4]])

# Operations
print(arr * 2)          # [2, 4, 6, 8, 10]
print(np.mean(arr))      # 3.0
print(np.sum(arr))       # 15
```

### Pandas Example
```python
import pandas as pd

# Create DataFrame
data = {"Name": ["John", "Alice", "Bob"], "Age": [30, 25, 35]}
df = pd.DataFrame(data)

# Read from file
df = pd.read_csv("file.csv")
df = pd.read_excel("file.xlsx")

# Operations
print(df.head())
print(df.describe())
df.groupby("column").mean()
df.fillna(0)
```

---

## 🌐 Python for Web Development

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                          WEB DEVELOPMENT STACK                                          │
├─────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                          │
│                        ┌─────────────────────┐                                          │
│                        │   FRONTEND          │                                          │
│                        │   (JavaScript/HTML) │                                          │
│                        └──────────┬──────────┘                                          │
│                                   │                                                      │
│  ┌───────────────────────────────┼─────────────────────────────────────────────────┐   │
│  │                               ▼                                                  │   │
│  │  ┌─────────────────────────────────────────────────────────────────────────────┐  │   │
│  │  │                         BACKEND APIS                                        │  │   │
│  │  ├─────────────────────────────────────────────────────────────────────────────┤  │   │
│  │  │                                                                              │  │   │
│  │  │   ┌─────────────┐    ┌─────────────┐    ┌─────────────┐                     │  │   │
│  │  │   │   Django    │    │   Flask     │    │  FastAPI    │                     │  │   │
│  │  │   │  Full-Stack │    │  Micro      │    │  Async API  │                     │  │   │
│  │  │   │  Framework  │    │  Framework  │    │  Framework  │                     │  │   │
│  │  │   └─────────────┘    └─────────────┘    └─────────────┘                     │  │   │
│  │  │                                                                              │  │   │
│  │  │   ┌─────────────┐    ┌─────────────┐    ┌─────────────┐                     │  │   │
│  │  │   │  SQLAlchemy │    │  Pydantic   │    │   Celery    │                     │  │   │
│  │  │   │   ORM       │    │  Validation │    │  Task Queue │                     │  │   │
│  │  │   └─────────────┘    └─────────────┘    └─────────────┘                     │  │   │
│  │  │                                                                              │  │   │
│  │  └─────────────────────────────────────────────────────────────────────────────┘  │   │
│  │                                       │                                           │   │
│  └───────────────────────────────────────┼───────────────────────────────────────────┘   │
│                                          ▼                                              │
│                        ┌─────────────────────┐                                          │
│                        │    DATABASE         │                                          │
│                        │  PostgreSQL/MySQL   │                                          │
│                        │    SQLite/MongoDB   │                                          │
│                        └─────────────────────┘                                          │
└─────────────────────────────────────────────────────────────────────────────────────────┘
```

### Django Example
```python
# Install
pip install django

# Create project
django-admin startproject myproject
cd myproject
python manage.py startapp myapp

# models.py
from django.db import models

class Post(models.Model):
    title = models.CharField(max_length=200)
    content = models.TextField()
    created_at = models.DateTimeField(auto_now_add=True)
    
    def __str__(self):
        return self.title

# views.py
from django.shortcuts import render
from .models import Post

def post_list(request):
    posts = Post.objects.all()
    return render(request, 'post_list.html', {'posts': posts})
```

### Flask Example
```python
from flask import Flask, jsonify, request

app = Flask(__name__)

@app.route('/api/hello')
def hello():
    return jsonify({"message": "Hello, World!"})

@app.route('/api/posts', methods=['GET', 'POST'])
def posts():
    if request.method == 'POST':
        data = request.json
        return jsonify({"created": data})
    return jsonify({"posts": []})

if __name__ == '__main__':
    app.run(debug=True)
```

### FastAPI Example
```python
from fastapi import FastAPI
from pydantic import BaseModel

app = FastAPI()

class Item(BaseModel):
    name: str
    price: float
    is_offer: bool = None

@app.get("/")
def read_root():
    return {"Hello": "World"}

@app.post("/items/")
def create_item(item: Item):
    return item

# Run with: uvicorn main:app --reload
```

---

## 🤖 Python for Automation & Scripting

```python
# Web Scraping with BeautifulSoup
from bs4 import BeautifulSoup
import requests

response = requests.get("https://example.com")
soup = BeautifulSoup(response.content, "html.parser")
print(soup.title.text)

# Selenium Automation
from selenium import webdriver

driver = webdriver.Chrome()
driver.get("https://example.com")
element = driver.find_element_by_name("q")
element.send_keys("Python")
element.submit()

# File Automation
import os
import shutil

# Copy, move, delete files
shutil.copy("source.txt", "dest.txt")
shutil.move("old.txt", "new.txt")
os.remove("file.txt")

# Schedule Tasks
import schedule
import time

def job():
    print("Task running")

schedule.every().day.at("10:00").do(job)

while True:
    schedule.run_pending()
    time.sleep(60)
```

---

## 💼 Career Paths

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                            PYTHON CAREER PATHS                                           │
├─────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                          │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐              │
│  │  WEB        │    │  DATA       │    │  ML/AI      │    │  DEV OPS    │              │
│  │  DEVELOPER │    │  SCIENTIST  │    │  ENGINEER   │    │  ENGINEER   │              │
│  ├─────────────┤    ├─────────────┤    ├─────────────┤    ├─────────────┤              │
│  │ Salary:     │    │ Salary:     │    │ Salary:     │    │ Salary:     │              │
│  │ $80-150K    │    │ $90-160K    │    │ $100-200K   │    │ $90-170K    │              │
│  ├─────────────┤    ├─────────────┤    ├─────────────┤    ├─────────────┤              │
│  │ Skills:     │    │ Skills:     │    │ Skills:     │    │ Skills:     │              │
│  │ Django/Flask│    │ Pandas/NumPy│    │ TensorFlow │    │ Docker/K8s  │              │
│  │ REST APIs   │    │ SQL/NoSQL   │    │ PyTorch    │    │ AWS/GCP     │              │
│  │ PostgreSQL  │    │ ML Algos    │    │ ML Ops     │    │ CI/CD       │              │
│  │ JavaScript  │    │ Visualization│   │ NLP        │    │ Terraform   │              │
│  └─────────────┘    └─────────────┘    └─────────────┘    └─────────────┘              │
│                                                                                          │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────────┐                                 │
│  │  AUTOMATION │    │  SECURITY   │    │  GAME       │                                 │
│  │  ENGINEER   │    │  ENGINEER   │    │  DEVELOPER  │                                 │
│  ├─────────────┤    ├─────────────┤    ├─────────────┤                                 │
│  │ Salary:     │    │ Salary:     │    │ Salary:     │                                 │
│  │ $70-130K    │    │ $90-180K    │    │ $60-120K    │                                 │
│  ├─────────────┤    ├─────────────┤    ├─────────────┤                                 │
│  │ Skills:     │    │ Skills:     │    │ Skills:     │                                 │
│  │ Selenium    │    │ Penetration │    │ Pygame      │                                 │
│  │ Scripting   │    │ Testing     │    │ Unity (C#)  │                                 │
│  │ APIs        │    │ Security    │    │ 3D Graphics │                                 │
│  │ Linux       │    │ Cryptography│    │ Physics     │                                 │
│  └─────────────┘    └─────────────┘    └─────────────┘                                 │
│                                                                                          │
└─────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 📖 Practice Resources

### Interactive Platforms
| Platform | Focus | Link |
|----------|-------|------|
| LeetCode | Algorithms | leetcode.com |
| HackerRank | Practice | hackerrank.com |
| Codewars | Katas | codewars.com |
| Exercism | Mentored | exercism.org |
| Project Euler | Math/Code | projecteuler.net |

### Tutorials & Documentation
| Resource | Description |
|----------|-------------|
| Python.org Docs | Official Documentation |
| Real Python | In-depth Tutorials |
| W3Schools Python | Beginner Friendly |
| Programiz | Examples & Tutorials |
| GeeksforGeeks | Computer Science |

---

## 💡 Project Ideas

### Beginner (Week 1-4)
- [ ] Number guessing game
- [ ] Calculator
- [ ] To-Do List CLI
- [ ] Temperature converter
- [ ] Simple password generator

### Intermediate (Week 5-8)
- [ ] Weather app using API
- [ ] Web scraper
- [ ] REST API
- [ ] Blog with Flask/Django
- [ ] Data visualization dashboard

### Advanced (Week 9+)
- [ ] Machine learning model
- [ ] Chat application
- [ ] E-commerce platform
- [ ] Automation scripts
- [ ] Full-stack web app

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

## 📄 License

MIT License - Feel free to use this roadmap for learning!

---

<p align="center">
  <strong>Made with ❤️ for Python Learners</strong>
  <br>
  <a href="#-python-learning-roadmap">Back to Top ↑</a>
</p>
