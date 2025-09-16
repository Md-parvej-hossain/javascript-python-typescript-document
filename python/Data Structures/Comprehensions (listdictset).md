🐍 Python Comprehensions — Detailed Explanation
## 🔹 1. Comprehension কী?

Comprehension হলো concise এবং readable way নতুন collection (list, dict, set) বানানোর।

Python-এ আমরা সাধারণত loop বা map/filter ব্যবহার করি।

Comprehension দিয়ে সেই কাজ এক লাইনে করতে পারি।

এটা code clean, short এবং fast করে।

## 🔹 2. List Comprehension
Syntax:
[expression for item in iterable if condition]


expression → কোন value add করা হবে

item → iterable থেকে প্রতিটি element

condition → optional, শুধু যেটা true তার element add হবে

* Example 1: Squares of numbers
numbers = [1, 2, 3, 4, 5]
squares = [x**2 for x in numbers]
print(squares)  # [1, 4, 9, 16, 25]

* Example 2: Only even numbers
evens = [x for x in numbers if x % 2 == 0]
print(evens)  # [2, 4]

* Example 3: Conditional expression
status = ["even" if x % 2 == 0 else "odd" for x in numbers]
print(status)  # ['odd', 'even', 'odd', 'even', 'odd']

## 🔹 3. Dictionary Comprehension
Syntax:
{key_expression: value_expression for item in iterable if condition}

* Example 1: Square of numbers as dictionary
numbers = [1, 2, 3, 4]
squares_dict = {x: x**2 for x in numbers}
print(squares_dict)  # {1: 1, 2: 4, 3: 9, 4: 16}

* Example 2: Only even numbers
even_dict = {x: x**2 for x in numbers if x % 2 == 0}
print(even_dict)  # {2: 4, 4: 16}

* Example 3: Key as string
names = ["parvej", "hiru", "ali"]
name_length = {name: len(name) for name in names}
print(name_length)  # {'parvej': 6, 'hiru': 4, 'ali': 3}

## 🔹 4. Set Comprehension
Syntax:
{expression for item in iterable if condition}

* Example 1: Unique squares
numbers = [1, 2, 2, 3, 4]
unique_squares = {x**2 for x in numbers}
print(unique_squares)  # {16, 1, 4, 9} → unordered, unique

* Example 2: Only odd numbers
odds = {x for x in numbers if x % 2 != 0}
print(odds)  # {1, 3}

* Example 3: Nested set comprehension
matrix = [[1, 2], [3, 4], [2, 5]]
unique_numbers = {num for row in matrix for num in row}
print(unique_numbers)  # {1, 2, 3, 4, 5}

## 🔹 5. Nested / Multi-level Comprehension
* Example 1: Flatten a matrix
matrix = [[1, 2], [3, 4], [5, 6]]
flat = [num for row in matrix for num in row]
print(flat)  # [1, 2, 3, 4, 5, 6]

* Example 2: Conditional nested
matrix = [[1, 2], [3, 4], [5, 6]]
even_numbers = [num for row in matrix for num in row if num % 2 == 0]
print(even_numbers)  # [2, 4, 6]

## 🔹 6. Advantages of Comprehensions
Advantage	Explanation
Compact code	এক লাইনে loop + condition
Readable	সহজে বোঝা যায়
Performance	অনেকক্ষেত্রে normal loop চেয়ে দ্রুত
Flexible	List, Set, Dict সবের জন্য ব্যবহার করা যায়
## 🔹 7. Quick Comparison: Loop vs Comprehension
# Using loop
squares = []
for x in range(5):
    squares.append(x**2)
print(squares)  # [0, 1, 4, 9, 16]

# Using list comprehension
squares = [x**2 for x in range(5)]
print(squares)  # [0, 1, 4, 9, 16]


✅ সংক্ষেপে:

List comprehension → [expr for item in iterable if condition]

Dict comprehension → {key: value for item in iterable if condition}

Set comprehension → {expr for item in iterable if condition}

Nested comprehension → multiple loops + condition