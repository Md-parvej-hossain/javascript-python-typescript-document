🐍 Python Tuples — Immutable Sequences
🔹 1. Tuple কী?

Tuple হলো Python-এর একটা ordered collection যেখানে একাধিক value রাখা যায়।
👉 কিন্তু tuple immutable, মানে একবার tuple বানানো হলে এর ভেতরের value পরিবর্তন, যোগ বা মুছা যায় না।

* tuple পরিবর্তন করা যায় না আনমিউট

# Example of a tuple
numbers = (10, 20, 30, 40)
fruits = ("apple", "banana", "mango")

🔹 2. Tuple বানানোর নিয়ম

ছোট বন্ধনী () ব্যবহার করে tuple তৈরি করা হয়।

একটা element থাকলে অবশ্যই comma , দিতে হবে।

t1 = (10, 20, 30)  
print(type(t1))  # <class 'tuple'>

t2 = (10,)  
print(type(t2))  # <class 'tuple'>

t3 = (10)  
print(type(t3))  # <class 'int'> (কারণ comma নাই)

🔹 3. Indexing (List-এর মতোই)

Tuple ordered, তাই index ব্যবহার করে value পাওয়া যায়।

numbers = (10, 20, 30, 40)

print(numbers[0])   # 10
print(numbers[2])   # 30
print(numbers[-1])  # 40

🔹 4. Slicing

Tuple immutable হলেও slice করা যায়, কিন্তু নতুন tuple তৈরি হবে।

numbers = (10, 20, 30, 40, 50)

print(numbers[1:4])   # (20, 30, 40)
print(numbers[:3])    # (10, 20, 30)
print(numbers[-2:])   # (40, 50)

🔹 5. Immutability

Tuple পরিবর্তন করা যায় না।

fruits = ("apple", "banana", "mango")

fruits[0] = "orange"   # ❌ TypeError: 'tuple' object does not support item assignment


👉 তবে, যদি tuple-এর ভেতরে mutable data type থাকে (যেমন list), সেটা modify করা যায়।

mixed = (10, [20, 30], 40)
mixed[1].append(50)
print(mixed)  # (10, [20, 30, 50], 40)

🔹 6. Tuple Methods

Tuple immutable, তাই list-এর সব method নাই। শুধু কিছু method আছে:

count(value) → কয়বার আছে সেটা বলে

index(value) → কোন index-এ আছে সেটা বলে

nums = (10, 20, 30, 20, 40)

print(nums.count(20))  # 2
print(nums.index(30))  # 2

🔹 7. Tuple ব্যবহার কেন?

ডেটা পরিবর্তন করতে না চাইলে (fixed data রাখার জন্য)

Dictionary-এর key হিসেবে ব্যবহার করা যায় (কারণ immutable)

একসাথে multiple values return করতে কাজে লাগে

# Example: function multiple return
def student():
    return ("Parvej", 22, "Comilla")

info = student()
print(info)  # ('Parvej', 22, 'Comilla')