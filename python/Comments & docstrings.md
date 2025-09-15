🐍 Python Comments & Docstrings (A to Z)
🔹 1. Comments (কমেন্টস)

👉 Python এ Comments হলো কোডে এমন লেখা যা interpreter ignore করে।
👉 এগুলো শুধু প্রোগ্রামার বুঝার জন্য লেখা হয়।

✨ Types of Comments
✅ Single-line Comment

# দিয়ে শুরু হয়।

# This is a single-line comment
x = 10  # Variable x stores an integer

✅ Multi-line Comment (Trick)

Python এ আলাদা multi-line comment নেই।

একাধিক লাইনে # ব্যবহার করতে হয়।
# This is line 1
# This is line 2
# This is line 3

✅ Comment for code explanation

# Add two numbers
a = 5
b = 3
sum = a + b  # 5 + 3 = 8
print(sum)


🔹 2. Docstrings (Documentation Strings)

👉 Docstrings হলো কোড (function, class, module) এর জন্য documentation বা বর্ণনা।
👉 এগুলো """ """ বা ''' ''' triple quotes এর মধ্যে লেখা হয়।
👉 এগুলোকে __doc__ attribute দিয়ে access করা যায়।

✨ Function Docstring
def add(a, b):
    """
    This function takes two numbers and returns their sum.
    
    Parameters:
    a (int): First number
    b (int): Second number
    
    Returns:
    int: Sum of a and b
    """
    return a + b

print(add.__doc__)   # Docstring দেখতে পারবেন


✨ Class Docstring

class Student:
    """
    A simple Student class.
    
    Attributes:
    name (str): The name of the student
    age (int): The age of the student
    """
    def __init__(self, name, age):
        self.name = name
        self.age = age


✨ Module Docstring

"""
This module contains simple math operations.
Author: Md Parvej
Date: 2025
"""

def multiply(a, b):
    """Return the product of two numbers."""
    return a * b

🔹 3. Difference: Comment vs Docstring

| Feature     | Comments                      | Docstrings                                           |
| ----------- | ----------------------------- | ---------------------------------------------------- |
| Syntax      | `#`                           | `""" """` / `''' '''`                                |
| Use         | কোড ব্যাখ্যা করার জন্য        | Documentation (functions, classes, modules)          |
| Interpreter | সম্পূর্ণ ignore করে           | `__doc__` দিয়ে access করা যায়                        |
| Scope       | যেকোনো জায়গায় ব্যবহার করা যায় | শুধু function, class, বা module এর শুরুতে ব্যবহার হয় |

🔹 4. Example (Mixing Both)

# This program demonstrates comments & docstrings

def greet(name):
    """
    This function greets the user by name.
    
    Parameters:
    name (str): The name of the user
    
    Returns:
    str: Greeting message
    """
    return f"Hello, {name}!"

# Call the function
print(greet("Parvej"))   # Output: Hello, Parvej!

# Docstring দেখা
print(greet.__doc__)

✅ Summary:

Comments → কোড ব্যাখ্যার জন্য (#)

Docstrings → Documentation এর জন্য (""" """)