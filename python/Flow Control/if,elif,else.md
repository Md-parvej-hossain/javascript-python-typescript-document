🐍 Python Condition (if, elif, else) — A to Z
## 🔹 1. Condition কী?

Condition মানে হলো কোনো শর্ত যাচাই করা।'
Python এ আমরা if, elif, else ব্যবহার করি।

## 🔹 2. if স্টেটমেন্ট

👉 শুধু একটি শর্ত যাচাই করতে হলে।

age = 20
if age >= 18:
    print("You are an adult")

## 🔹 3. if + else

👉 যদি শর্ত মিলে না যায়, তখন অন্য কাজ
age = 15
if age >= 18:
    print("Adult")
else:
    print("Not Adult")


## 🔹 4. if + elif + else

👉 একাধিক শর্ত যাচাই করতে হলে।

marks = 75

if marks >= 80:
    print("A+")
elif marks >= 70:
    print("A")
elif marks >= 60:
    print("A-")
else:
    print("Fail")


## 🔹 5. Nested if (ভেতরে আরেকটা if)

👉 শর্তের ভেতরে আবার শর্ত
x = 25
if x > 10:
    print("Greater than 10")
    if x > 20:
        print("Also greater than 20")


## 🔹 6. Short Hand if

👉 এক লাইনে লিখতে পারো।

x = 5
if x > 2: print("x is greater than 2")



## 🔹 7. Short Hand if else
👉 এক লাইনে if else।



x = 10
print("Positive") if x > 0 else print("Negative")

## 🔹 8. Multiple Conditions (and/or)

👉 একাধিক শর্ত একসাথে ব্যবহার।

x = 15
if x > 10 and x < 20:
    print("x is between 10 and 20")

y = 5
if y < 10 or y == 5:
    print("y is valid")


## 🔹 9. Pass Statement

👉 যখন কিছু লিখতে চাই না তখন pass ব্যবহার।

x = 10
if x > 5:
    pass   # future code আসবে


## 🔹 10. Practical Example

temperature = 32

if temperature > 35:
    print("Hot Day")
elif temperature > 25:
    print("Normal Day")
elif temperature > 15:
    print("Cold Day")
else:
    print("Freezing Day")


✅ Summary (সারাংশ):

if → শর্ত চেক করার জন্য।

elif → একাধিক শর্ত চেক করার জন্য।

else → যখন কোনো শর্ত মিলবে না।

and / or / not → একাধিক শর্ত মেশানোর জন্য।

pass → ফাঁকা রেখে যাওয়ার জন্য।