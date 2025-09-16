🔹 Python Ternary Operator (Conditional Expression)

Syntax:

value_if_true if condition else value_if_false

🔸 Example 1: সাধারণ ব্যবহার
age = 18
result = "Adult" if age >= 18 else "Child"
print(result)  


👉 Output: Adult

🔸 Example 2: Even / Odd Check
num = 7
result = "Even" if num % 2 == 0 else "Odd"
print(result)  


👉 Output: Odd

🔸 Example 3: Positive / Negative / Zero
num = -5
result = "Positive" if num > 0 else "Zero" if num == 0 else "Negative"
print(result)


👉 Output: Negative

🔸 Example 4: Short Assignment
is_logged_in = True
message = "Welcome back!" if is_logged_in else "Please log in"
print(message)


👉 Output: Welcome back!

🔸 Example 5: Inline ব্যবহার (function এর মধ্যে)
def max_num(a, b):
    return a if a > b else b

print(max_num(10, 20))  


👉 Output: 20

✅ Ternary operator mainly code ছোট করার জন্য ব্যবহার হয়।
✅ তবে খুব বেশি nested ব্যবহার করলে code বুঝতে কষ্ট হয়।