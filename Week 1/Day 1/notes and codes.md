# Welcome ! to *Day 1* of Python for beginners series
-by **[Shubham](https://github.com/Shubham-S151)** from `Bit and Pi` YouTube Channel.

***Channel Link :*** [![YouTube](https://img.shields.io/badge/YouTube-Bit_and_Pi-red?logo=youtube&style=for-the-badge)](https://www.youtube.com/@BitandPi)

#### Connect to the author and teacher here :
[![Email](https://img.shields.io/badge/Email-%23D14836.svg?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shubhamsharma15104@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-%23000000.svg?style=for-the-badge&logo=firefox&logoColor=white)](https://sites.google.com/view/shubham-sharma-portfolio/home)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shubham-data-science)  

## Index
|S.No.|topic name|Navigate|
|--|--|--|
|1|Intro to python|[Click Here](#intro-to-python)|
|2|Defining a variable|[Click Here](#defining-a-variable)|
|3|Rules for Defining Variables in Python|[Click Here](#rules-for-defining-variables-in-python)|
|4|Data Types in Python|[Click Here](#data-types-in-python)|
|4-1|String Data Type|[Click Here](#4-1-string-data-type)|
|4-2|Numeric Data Type|[Click Here](#4-2-numeric-data-type)|
|4-3|Boolean & None Data Type|[Click Here](#4-3-boolean-and-none-data-type)|
|4-4|Collection Data Type|[Click Here](#4-4-collection-data-type)|
|5|Summary|[Click Here](#summary)|


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

## Defining a Variable

In Python, a variable is a name that refers to a value stored in memory. You can think of it as a labeled container for data. Variables make your code more readable and allow you to reuse values efficiently.

To define (or declare) a variable, use the assignment operator =. The syntax is:

```python
variable_name = value
```
Here’s a simple example:

```python
x = 23            # 'x' is a variable holding the integer value 23
name = 'Shubham'  # 'name' is a variable holding the string 'Shubham'

print(x)          # Output: 23
print(name)       # Output: Shubham
```
**Things to Remember:**

- Variable names should be descriptive and follow Python naming conventions (e.g., snake_case).
- Python is dynamically typed, so you don’t need to declare the type of a variable; it’s inferred automatically.
- Variable names are case-sensitive (age and Age are different).
- You can reassign variables to different values or even different types:

```python
age = 21
age = "twenty-one"  # Now 'age' holds a string instead of a number
```
Try experimenting with different variable names and values to solidify your understanding.

**[🔝Index](#index)**

---

## Rules for Defining Variables in Python

When defining variables in Python, there are a few rules and guidelines to follow to ensure your code runs correctly and is easy to read. Let’s take a look at these essential rules:

**1. Variable names must begin with a letter or an underscore (_).**
   - Valid: `x`, `_my_variable`, `age`
   - Invalid: `1age`, `@variable`

 **2. Variable names can only contain letters (a-z, A-Z), numbers (0-9), and underscores (_).**
   - Valid: `my_var`, `age_123`, `my_variable`
   - Invalid: `my-variable`, `my variable`

 **3. Variable names are case-sensitive.**
   - `age`, `Age`, and `AGE` are considered different variables in Python.

 **4. Avoid using Python keywords as variable names.**
   - Keywords are reserved words in Python, and they have special meanings. You can’t use them as variable names. Examples of keywords include: `if`, `else`, `for`, `while`, `def`, `class`, etc.
   - Valid: `variable`, `my_var`
   - Invalid: `if`, `else`, `while`

 **5. Variable names should be descriptive and follow a consistent naming convention.**
   - Use **snake_case** for variable names (e.g., `user_age`, `total_price`).
   - Avoid one-letter variables unless in specific cases (e.g., `x`, `y` in mathematical operations).

 **6. You can reassign variables to different data types.**
   - Since Python is dynamically typed, you can change the type of a variable during the execution of a program.
   - Example:
     ```python
     x = 10        # x is an integer
     x = "Hello"   # x is now a string
     ```

 **7. Whitespace (spaces, tabs) is not allowed within variable names.**
   - Valid: `first_name`, `total_score`
   - Invalid: `first name`, `total score`

 **8. Variables cannot start with a number.**
   - Valid: `age1`, `score_100`
   - Invalid: `1age`, `100_score`

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

### 4-1 String Data Type

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

### 4-2 Numeric Data Type

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

### 4-3 Boolean and None Data Type

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

### 4-4 Collection Data Type

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

## Summary

Today, we began our journey with Python by exploring the fundamental concepts every beginner should know:

- **Introduction to Python**  
  Python is a beginner-friendly, high-level programming language known for its clean syntax and readability. It's widely used in fields like data science, automation, and web development.

- **Defining Variables**  
  Variables are used to store data. Python uses the `=` operator for assignment and infers data types automatically (dynamic typing).

- **Variable Naming Rules**  
  Variable names must start with a letter or underscore, cannot include spaces or special characters, and are case-sensitive. Keywords like `if` or `class` cannot be used as variable names.

- **Data Types Overview**  
  Python supports several built-in data types:
  - **String (`str`)**: Text data
  - **Numeric Types**: Integers, floats, and complex numbers
  - **Boolean (`bool`)**: True/False values
  - **NoneType (`None`)**: Represents no value
  - **Collections**: Lists, tuples, sets, and dictionaries (covered partially today)

This foundation will help you write clean, readable, and effective Python code in upcoming lessons.

**[🔝Index](#index)**