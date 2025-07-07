# Solutions — Day 1 Assignment: Python for Beginners

---

## 🔹 Section A: Theory-Based Questions

1. **What is Python, and why is it considered a beginner-friendly language?**  
   Python is a high-level, interpreted programming language with a syntax that closely resembles English, making it easy to read and write. Its simplicity, dynamic typing, and massive standard libraries make it beginner-friendly.

2. **What does "Python is dynamically typed" mean?**  
   It means you don’t need to declare the data type of a variable when assigning it a value. The type is determined automatically at runtime.  
   **Example:**  
   ```python
   x = 10        # x is an integer
   x = "hello"   # Now x is a string
   ```
3. **Three rules to follow when naming a variable in Python:**
   - Variable names must start with a letter (a–z, A–Z) or an underscore (_).
   - Variable names can contain letters, digits (0–9), and underscores.
   - Python keywords (e.g., `if`, `class`, `for`) cannot be used as variable names.

4. **Difference between `Age` and `age` in Python:**
   Python is case-sensitive.  
   So `Age` and `age` are treated as **two distinct variables**.  
   Example:
   ```python
   Age = 25
   age = 30
   print(Age)  # Output: 25
   print(age)  # Output: 30
   ```
5. **Define the following data types with real-life examples:**

   - `str` (String): Used to represent text data.
     - Example: `"Hello, world!"` could be a greeting message on a website.

   - `int` (Integer): Used to represent whole numbers.
     - Example: `28` could be someone's age.

   - `bool` (Boolean): Represents either `True` or `False`.
     - Example: `is_logged_in = True` means a user is currently logged in.

   - `None` (NoneType): Used to signify the absence of a value.
     - Example: `score = None` when a quiz hasn’t been submitted yet, so no score is available.

## 🔹 Section B: Predict the Output — Solutions

### 1.
```python
x = 5
x = "Python"
print(x)
```
**Output :**
```
Python
```
**Explanation:**
The variable `x` is first assigned an integer 5, then reassigned the string `"Python"`.
Since Python is dynamically typed, the type can change. `print(x)` displays the latest value.

### 2. 
```python
name = "Alice"
print(f"Hello, {name}")
```
**Output :**
```
Hello, Alice
```
**Explanation:**
This is an example of an **f-string**, which allows embedding expressions inside strings using {}.
