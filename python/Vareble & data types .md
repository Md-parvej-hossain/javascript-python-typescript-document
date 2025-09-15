# 🐍 Python Variables & Data Types

## 🔹 Variables
- Variable হলো একটি **container (box)** যেখানে data রাখা হয়।
- Python এ `=` ব্যবহার করে মান (value) assign করা হয়।

```python
x = 10        # integer
name = "Parvej"   # string

🔹 Data Types
1. int → Integer (পূর্ণ সংখ্যা)

দশমিক ছাড়া সংখ্যা।

Positive, negative বা zero হতে পারে।
age = 25
year = 2025
roll = -101

print(type(age))   # <class 'int'>

2. float → Floating Point Number (দশমিক সংখ্যা)

দশমিক সহ সংখ্যা।

pi = 3.1416
price = 99.99
temperature = -12.5

print(type(pi))   # <class 'float'>

3. str → String (টেক্সট ডেটা)

টেক্সট/অক্ষর।

" " বা ' ' কোটেশনের ভেতরে লিখতে হয়।

name = "Md Parvej"
city = 'Comilla'
message = "Hello, World!"

print(type(name))   # <class 'str'>

4. bool → Boolean (True/False)

কেবল দুইটি মান থাকে → True অথবা False

সাধারণত condition এ ব্যবহার হয়।
is_student = True
has_money = False

print(type(is_student))   # <class 'bool'>


🔹 Full Example (Mixing All Types)

age = 20           # int
height = 5.7       # float
name = "Parvej"    # str
is_programmer = True   # bool

print(age, type(age))
print(height, type(height))
print(name, type(name))
print(is_programmer, type(is_programmer))
