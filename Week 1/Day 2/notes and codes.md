# Welcome ! to *Day 2* of Python for beginners series
-by **[Shubham](https://github.com/Shubham-S151)** from `Bit and Pi` YouTube Channel.

***Channel Link :*** [![YouTube](https://img.shields.io/badge/YouTube-Bit_and_Pi-red?logo=youtube&style=for-the-badge)](https://www.youtube.com/@BitandPi)

#### Connect to the author and teacher here :
[![Email](https://img.shields.io/badge/Email-%23D14836.svg?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shubhamsharma15104@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-%23000000.svg?style=for-the-badge&logo=firefox&logoColor=white)](https://sites.google.com/view/shubham-sharma-portfolio/home)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shubham-data-science)  

## Index
|S.No.|topic name|Navigate|
|--|--|--|
|01|What is a String in Python? |[Click Here](#what-is-a-string-in-python)|
|02|Creating Strings|[Click Here](#creating-strings)|
|03|Basic Operations|[Click Here](#basic-operations)|
|04|String Indexing and Slicing|[Click Here](#string-indexing-and-slicing)|
|05|String Methods|[Click Here](#string-methods)|
|06|String Formatting|[Click Here](#string-formatting)|
|07|Escape Characters and Raw Strings|[Click Here](#escape-characters-and-raw-strings)|
|08|Summary|[Click Here](#summary)|

## What is a String in Python?

A **string** in Python is a sequence of characters enclosed in either single (`'`) or double (`"`) quotes. Strings are used to store text-based data like names, messages, or any collection of characters.

**String Definition and Examples**

You can create strings using:
```python
'Hello'
"World"
'1234'
"Python Programming"
```
All of the above are valid strings.

### Type: `str`

In Python, every string is an instance of the built-in str class.

```python
text = "Hello, Python!"
print(type(text))  # Output: <class 'str'>
```
### Immutable Nature of Strings

Strings in Python are **immutable**, meaning once a string is created, it cannot be changed. Any operation that seems to change a string actually creates a new string.

```python
s = "hello"
s[0] = "H"  # Error: 'str' object does not support item assignment
```
To "modify" a string, you can create a new one:

```python
s = "hello"
s = "H" + s[1:]  # "Hello"
```
**[🔝Index](#index)**

## Creating Strings

In Python, strings can be created using single quotes (`'`), double quotes (`"`), or triple quotes (`'''` or `"""`). All of them serve the same basic purpose, but each has specific use cases.

---

### Single Quotes vs Double Quotes vs Triple Quotes

You can use either single or double quotes to create simple strings:

```python
message1 = 'Hello'
message2 = "World"
```
Both are functionally the same. Using one type lets you include the other without escaping:

```python
quote1 = "It's a beautiful day"
quote2 = '"Python" is powerful'
```
Triple quotes are typically used for multi-line strings or docstrings:

```python
description = '''This is a
multi-line string in Python.'''

doc = """Triple quotes are useful
for documentation and long text blocks."""
```

### Triple Quotes for Multiline Strings

Triple-quoted strings preserve line breaks, tabs, and other formatting:

```python
text = """Line 1
Line 2
    Indented Line 3"""
print(text)
```
Output:

```scss
Line 1
Line 2
    Indented Line 3
```
### Escaping Characters (Intro)

Sometimes you need to include characters in a string that would otherwise be interpreted differently, such as quotes, newlines, or backslashes. This is done using **escape characters**.

Example (covered in detail later):

```python
print("Line1\nLine2")
print("This is a tab:\tRight here")
```
\> A full explanation is provided in the [Escape Characters and Raw Strings section](#escape-characters-and-raw-strings).

**[🔝Index](#index)**

## Basic Operations

Python provides several basic operations that you can perform on strings. These are useful for combining, measuring, and checking string content.

---

### Concatenation

You can **combine strings** using the `+` operator:

```python
greeting = 'Hello' + ' ' + 'World'
print(greeting)  # Output: Hello World
```
This creates a new string by joining the parts together.

### Repetition

You can **repeat a string** multiple times using the `*` operator:

```python
laugh = 'ha' * 3
print(laugh)  # Output: hahaha
```
Useful for simple patterns and placeholders.

### Length

Use the built-in `len()` function to get the **number of characters** in a string:

```python
word = "Hello"
print(len(word))  # Output: 5
```
This counts all characters, including spaces and punctuation.

### Membership

You can check whether a `character or substring exists` within another string using `in` and `not` in:

```python
print('a' in 'banana')      # Output: True
print('z' not in 'apple')   # Output: True
```
This is useful in search operations and conditionals.

---
**[🔝Index](#index)**

## String Indexing and Slicing

Strings in Python are **ordered sequences**, which means each character has a specific position (index). You can access and extract parts of a string using **indexing** and **slicing**.

---

### Indexing

Each character in a string has an index starting from `0`. You can use **positive indexing** (from the start) or **negative indexing** (from the end).

```python
s = "Python"
print(s[0])   # Output: 'P' (first character)
print(s[-1])  # Output: 'n' (last character)
```
Indexing a position that doesn’t exist will raise an `IndexError`.
### Slicing
**Slicing** lets you extract a substring using the format `string[start:stop]`.

```python
s = "Python"
print(s[0:3])   # Output: 'Pyt' (characters at index 0, 1, 2)
print(s[:5])    # Output: 'Pytho' (start is optional, defaults to 0)
print(s[::-1])  # Output: 'nohtyP' (reverses the string)
```
The stop index is exclusive, meaning the character at that position is not included.

### Step in Slices
You can also define a **step value** to skip characters.

```python
s = "Python"
print(s[::2])   # Output: 'Pto' (every second character)
print(s[1::2])  # Output: 'yhn' (starts from index 1, every second char)
```
The general slicing format is: s[start:stop:step]

- Indexing: s[0], s[-1]
- Slicing: s[0:3], s[:5], s[::-1]
- Step in slices: s[::2]
---
**[🔝Index](#index)**

## String Methods

Python provides a wide range of **built-in string methods** that allow you to manipulate and analyze text easily. Most string methods return new strings and do **not** modify the original string (because strings are immutable).

---

### Case Methods

Used to change the **letter casing** of a string:

```python
s = "hello world"

print(s.upper())      # Output: 'HELLO WORLD'
print(s.lower())      # Output: 'hello world'
print(s.title())      # Output: 'Hello World'
print(s.capitalize()) # Output: 'Hello world'
```
### Searching Methods
Used to **find substrings** within a string:

```python
s = "banana"

print(s.find("na"))       # Output: 2 (first occurrence)
print(s.index("a"))       # Output: 1 (like find, but raises error if not found)
print(s.count("a"))       # Output: 3 (number of occurrences)
print(s.startswith("ba")) # Output: True
print(s.endswith("na"))   # Output: True
```
### Modifying Methods
Used to **alter the contents** of a string:

```python
s = "  hello  "

print(s.replace("l", "L"))   # Output: '  heLLo  '
print(s.strip())             # Output: 'hello' (removes outer whitespace)
print(s.lstrip())            # Output: 'hello  ' (left side)
print(s.rstrip())            # Output: '  hello' (right side)
```
### Splitting and Joining
Used to **break a string into parts** or **combine parts into a string:**

```python
s = "apple,banana,cherry"

fruits = s.split(",")
print(fruits)  # Output: ['apple', 'banana', 'cherry']

sentence = " ".join(["Join", "these", "words"])
print(sentence)  # Output: 'Join these words'
```
`.split()` turns a string into a list; `.join()` does the reverse.

---
**[🔝Index](#index)**

## String Formatting

String formatting in Python lets you **insert variables or expressions** into strings in a clean, readable way. Python offers three main formatting styles.

---

### 🔹 f-Strings (Formatted String Literals)

Introduced in Python 3.6, **f-strings** are the most modern and readable way to format strings.

```python
name = "Alice"
age = 25

print(f"Hello, {name}. You are {age} years old.")
# Output: Hello, Alice. You are 25 years old.
```
### .format() Method
Available in Python 2.7 and 3.x. You can insert values into placeholders using `{}`.

```python
name = "Bob"
print("Hello, {}".format(name))  # Output: Hello, Bob

# Multiple values
print("Name: {}, Age: {}".format("Carol", 30))
```
You can also use **positional** and **named** arguments:

```python
print("Coordinates: {x}, {y}".format(x=10, y=20))
```
### Old-Style Formatting (C-style)
This is the oldest way to format strings, similar to C's **printf**.

```python
name = "Dave"
print("Hello %s" % name)  # Output: Hello Dave

# Multiple values
print("Name: %s, Age: %d" % ("Eve", 28))
```
>Still supported, but f-strings or `.format()` are preferred for readability.
---
**[🔝Index](#index)**

## Escape Characters and Raw Strings

In Python, some characters have **special meanings** when used in strings. These are called **escape characters**, and they are introduced with a backslash (`\`).

---

### 🔹 Common Escape Characters

| Escape Sequence | Description                         | Example / Notes                           |
|-----------------|-------------------------------------|-------------------------------------------|
| `\\`            | Backslash                           | Represents a literal backslash (`\`)      |
| `\'`            | Single quote                        | Useful inside single-quoted strings       |
| `\"`            | Double quote                        | Useful inside double-quoted strings       |
| `\n`            | Newline                             | Moves to the next line                    |
| `\t`            | Horizontal tab                      | Inserts a tab space                       |
| `\r`            | Carriage return                     | Moves cursor to beginning of the line     |
| `\b`            | Backspace                           | Removes the character before it           |
| `\f`            | Form feed                           | Advances the printer to the next page     |
| `\v`            | Vertical tab                        | Rarely used, adds vertical spacing        |
| `\a`            | Bell (alert)                        | Triggers system alert (may not be visible)|
| `\ooo`          | Octal value                         | Character with octal value `ooo`          |
| `\xhh`          | Hexadecimal value                   | Character with hex value `hh`             |
| `\N{name}`      | Unicode character by name           | `\N{COPYRIGHT SIGN}` = © (requires `unicodedata`) |
| `\uXXXX`        | 16-bit Unicode character             | e.g. `\u00A9` = ©                         |
| `\UXXXXXXXX`    | 32-bit Unicode character             | e.g. `\U0001F600` = 😀                     |


```python
print("Line1\nLine2")       # Output:
# Line1
# Line2

print("Column1\tColumn2")   # Output: Column1    Column2

print("She said: \"Hi!\"")  # Output: She said: "Hi!"
```
### Raw Strings
Raw strings treat backslashes **literally**—they are not interpreted as escape characters. Use them when dealing with paths, regular expressions, etc.

```python
path = r"C:\Users\Admin\Documents"
print(path)  # Output: C:\Users\Admin\Documents
```
Without `r`, you'd have to escape every backslash:

```python
path = "C:\\Users\\Admin\\Documents"
```
>Always consider raw strings when working with file paths on Windows or regex patterns.
---
**[🔝Index](#index)**

## Summary
Strings are one of the most fundamental data types in Python and are used to handle and manipulate text data. Here's a quick recap of what you've learned:

---

### 🔹 Key Takeaways

- Strings are sequences of characters enclosed in quotes (`'...'`, `"..."`, or `'''...'''`).
- Strings are of type `str` and are **immutable**, meaning they cannot be changed after creation.
- Python supports:
  - **Concatenation** (`+`) and **repetition** (`*`)
  - **Indexing** and **slicing** to access parts of strings
  - A wide range of **built-in string methods** for case conversion, searching, modifying, splitting, and joining
- Strings can be formatted using:
  - `f-strings`
  - `.format()` method
  - Old-style `%` formatting
- **Escape characters** allow special characters like newlines (`\n`), tabs (`\t`), and quotes to be included in strings.
- **Raw strings** (`r"..."`) treat backslashes literally, useful for file paths and regular expressions.

---

Mastering string operations is essential for working with user input, file processing, web data, and much more in real-world Python applications.

---
**[🔝Index](#index)**