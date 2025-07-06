# Welcome ! to *Day 1* of Python for beginners series
-by [Shubham](https://github.com/Shubham-S151) from [Bit and Pi Youtube Channel](https://www.youtube.com/@BitandPi) 
*Channel Link :* [![YouTube](https://img.shields.io/badge/YouTube-Bit_and_Pi-red?logo=youtube&style=for-the-badge)](https://www.youtube.com/@BitandPi)

#### Connect to the author and teacher here :
[![Email](https://img.shields.io/badge/Email-%23D14836.svg?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shubhamsharma15104@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-%23000000.svg?style=for-the-badge&logo=firefox&logoColor=white)](https://sites.google.com/view/shubham-sharma-portfolio/home)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shubham-data-science)  

## Index
|S.No.|topic name|Navigate|
|--|--|--|
|1|Intro to python|[Click Here](#intro-to-python)|
|2|Data Types in Python|[Click Here](#data-types-in-python)|
|2-1|String Data Type|[Click Here](#2-1-string-data-type)|
|2-2|Numeric Data Type|[Click Here](#2-2-numeric-data-type)|
|2-3|Boolean & None Data Type|[Click Here](#2-3-boolean-and-none-data-type)|
|2-4|Collection Data Type|[Click Here](#2-4-collection-data-type)|


## Intro to Python


Python is a **high-level, interpreted programming language** known for its simplicity and readability. Created by Guido van Rossum and released in 1991, Python emphasizes code clarity using indentation instead of braces, making it an excellent first language for beginners.

Key features include:
- **Easy syntax:** Close to natural English.
- **Interpreted:** Runs line by line, great for quick feedback.
- **Cross-platform:** Works on Windows, macOS, Linux.
- **Extensive libraries:** Supports everything from web development to data science.
- **Dynamic typing:** Variable types are inferred, making coding faster.
- **Community support:** Huge ecosystem and active community.

Python is widely used in web development, automation, data analysis, machine learning, scripting, and more.

**[🔝Index](#index)**

---
## Data Types in Python

Python supports several built-in **data types** that represent different kinds of values. Understanding these types is foundational to programming in Python.

- **Numeric types:** int, float, complex
- **Text type:** str (string)
- **Boolean type:** bool (True or False)
- **NoneType:** None, represents the absence of a value
- **Collection types:** list, tuple, set, dict

Each type has unique properties and methods, and Python automatically manages memory and type conversions where possible.

**[🔝Index](#index)**

### 2-1 String Data Type

Strings (`str`) in Python represent sequences of Unicode characters. Strings are **immutable**, meaning once created, they cannot be changed directly.

Features:
- Created by enclosing text in single (`'...'`), double (`"..."`), or triple quotes (`'''...'''` or `"""..."""`).
- Support concatenation (`+`), repetition (`*`), slicing (`str[start:end]`), and many useful methods like `.lower()`, `.upper()`, `.strip()`, `.replace()`.
- Can contain escape sequences like `\n` (newline), `\t` (tab).
- Formatted strings (`f"Hello, {name}!"`) enable embedding expressions inside string literals.
- Used extensively for user input/output, file handling, and text processing.

Example:
```python
name = "Alice"
greeting = f"Hello, {name}!"
print(greeting)  # Output: Hello, Alice!
```

**[🔝Index](#index)**

### 2-2 Numeric Data Type

Python has three main numeric types:

- **int**: Integer numbers (e.g., `5`, `-42`, `1000`) with arbitrary precision.

- **float**: Floating-point numbers (e.g., `3.14`, `-0.001`), representing real numbers using double-precision.

- **complex**: Numbers with real and imaginary parts (e.g., `2+3j`), used in scientific computing.

`Note :`here **j** is the complex number inplace of **i (iota)** which is sqrt(-1)

Python supports standard arithmetic operations (`+`, `-`, `*`, `/`, `//`, `%`, `**`) and provides built-in functions like `abs()`, `round()`, and `pow()`.

**Example:**

```python
a = 10
b = 3
print(a // b)  # Integer division, output: 3
print(a / b)   # Float division, output: 3.3333333333333335
```

**[🔝Index](#index)**

### 2-3 Boolean and None Data Type

**Boolean (bool)**
- Represents truth values: True and False.
- Used extensively in control flow (conditions, loops).
- Results of comparison operators (==, >, <) and logical operators (and, or, not) are booleans.

Example:

```python
is_adult = True
if is_adult:
    print("Access granted.")
```

**NoneType (None)**

- Represents the absence of a value or a null value.
- Commonly used to indicate “no result” or “empty” variables.
- None is a singleton; you check it with is None not equality.

Example:

```python
result = None
if result is None:
    print("No result available.")
```

**[🔝Index](#index)**

### 2-4 Collection Data Type

### 2-4 Collection Data Type

Python provides several built-in collection data types that group multiple values into a single variable. These collections are versatile and widely used to store, organize, and manipulate data.

The main collection types are:

- **list**  
  An ordered, mutable (changeable) collection of items. Lists allow duplicate elements and can contain mixed data types.

  Example:

  ```python
  fruits = ["apple", "banana", "cherry"]
  fruits.append("orange")  # Adds "orange" to the list
  print(fruits[1])         # Output: banana
  ``` 

**[🔝Index](#index)**