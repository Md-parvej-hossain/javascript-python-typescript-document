# ⚡ Python Operators (A to Z)

Python এ Operators ব্যবহার করা হয় **গণনা করা**, **তুলনা করা**, **logic apply করা**, এবং **ভেরিয়েবল আপডেট করার জন্য**।
🐍 Python Operators (List)
🔹 1. Arithmetic Operators

🔹 2. Comparison (Relational) Operators

🔹 3. Logical Operators

🔹 4. Assignment Operators


🔹 5. Bitwise Operators


🔹 6. Identity Operators

🔹 7. Membership Operators

---

## 🔹 1. Arithmetic Operators (গাণিতিক অপারেটর)
👉 গাণিতিক হিসাব করার জন্য ব্যবহার হয়।

| Operator | Name              | Example (`a = 10, b = 3`) | Result |
|----------|------------------|----------------------------|--------|
| `+`      | Addition          | `a + b`                   | `13`   |
| `-`      | Subtraction       | `a - b`                   | `7`    |
| `*`      | Multiplication    | `a * b`                   | `30`   |
| `/`      | Division          | `a / b`                   | `3.333...` |
| `//`     | Floor Division    | `a // b`                  | `3`    |
| `%`      | Modulus           | `a % b`                   | `1`    |
| `**`     | Exponent (power)  | `a ** b`                  | `1000` |

---

## 🔹 2. Comparison Operators (তুলনা করার জন্য)
👉 দুটি মান compare করলে `True` বা `False` রিটার্ন করে।

| Operator | Meaning            | Example (`a = 10, b = 3`) | Result |
|----------|-------------------|----------------------------|--------|
| `==`     | Equal              | `a == b`                  | `False` |
| `!=`     | Not Equal          | `a != b`                  | `True`  |
| `>`      | Greater than       | `a > b`                   | `True`  |
| `<`      | Less than          | `a < b`                   | `False` |
| `>=`     | Greater or Equal   | `a >= b`                  | `True`  |
| `<=`     | Less or Equal      | `a <= b`                  | `False` |

---

## 🔹 3. Logical Operators (লজিক্যাল অপারেটর)
👉 Multiple condition check করতে ব্যবহৃত হয়।

| Operator | Meaning                          | Example (`a = 10, b = 3`) | Result |
|----------|----------------------------------|----------------------------|--------|
| `and`    | True if **both** True            | `(a > 5 and b < 5)`        | `True` |
| `or`     | True if **any one** True         | `(a > 5 or b > 10)`        | `True` |
| `not`    | Reverse the result               | `not(a > 5)`               | `False` |

---

## 🔹 4. Assignment Operators (মান সেট করার জন্য)
👉 Variable এ মান সেট বা আপডেট করতে ব্যবহার হয়।

| Operator | Meaning                        | Example (`x = 5`) | Result |
|----------|--------------------------------|-------------------|--------|
| `=`      | Assign value                   | `x = 5`           | `5`    |
| `+=`     | Add and assign                 | `x += 3`          | `8`    |
| `-=`     | Subtract and assign            | `x -= 2`          | `6`    |
| `*=`     | Multiply and assign            | `x *= 4`          | `24`   |
| `/=`     | Divide and assign              | `x /= 3`          | `8.0`  |
| `//=`    | Floor divide and assign        | `x //= 2`         | `4`    |
| `%=`     | Modulus and assign             | `x %= 3`          | `2`    |
| `**=`    | Power and assign               | `x **= 2`         | `25`   |

---

## 🔹 5. Bitwise Operators (বিটওয়াইজ অপারেটর)
👉 Binary (0/1) level এ কাজ করে।

| Operator | Name        | Example (`a = 6 (110)`, `b = 2 (010)`) | Result (Binary) |
|----------|-------------|-----------------------------------------|-----------------|
| `&`      | AND         | `a & b` → `110 & 010`                  | `010 (2)`       |
| `|`      | OR          | `a | b` → `110 | 010`                  | `110 (6)`       |
| `^`      | XOR         | `a ^ b` → `110 ^ 010`                  | `100 (4)`       |
| `~`      | NOT         | `~a`                                   | `-(a+1)`        |
| `<<`     | Left Shift  | `a << 1`                               | `12`            |
| `>>`     | Right Shift | `a >> 1`                               | `3`             |

---

## 🔹 6. Identity Operators (পরিচয় যাচাই করার জন্য)
👉 Object memory location check করে।

| Operator | Meaning                  | Example (`x = [1,2], y = [1,2]`) | Result |
|----------|--------------------------|----------------------------------|--------|
| `is`     | Same object?             | `x is y`                        | `False` |
| `is not` | Not same object?         | `x is not y`                    | `True`  |

---

## 🔹 7. Membership Operators (সদস্যতা যাচাই)
👉 Collection (list, tuple, string) এ কোনো element আছে কিনা check করে।

| Operator | Meaning                  | Example (`x = [1,2,3]`) | Result |
|----------|--------------------------|--------------------------|--------|
| `in`     | Present in collection?   | `2 in x`                | `True` |
| `not in` | Not present in collection? | `5 not in x`          | `True` |

---

## 🔹 Example Code (All Operators)
```python
a = 10
b = 3
x = [1, 2, 3]
y = [1, 2, 3]

# Arithmetic
print(a + b, a - b, a * b, a / b, a // b, a % b, a ** b)

# Comparison
print(a > b, a == b, a != b)

# Logical
print(a > 5 and b < 5)
print(a > 5 or b > 10)
print(not(a > 5))

# Assignment
num = 5
num += 3
print(num)

# Bitwise
print(a & b, a | b, a ^ b, ~a, a << 1, a >> 1)

# Identity
print(x is y)      # False (different objects)
print(x is not y)  # True

# Membership
print(2 in x)      # True
print(5 not in x)  # True
