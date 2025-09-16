🐍 Python List — A to Z (Indexing, Slicing, Methods)
🔹 1. List কী?

List হলো Python-এর একটা collection data type, যেখানে একাধিক value রাখা যায় একই ভেরিয়েবলে।
👉 List-এর বৈশিষ্ট্য:

* লিস্টে ডাটা পরিবর্তন করা যায় list মিউটেবল 

Ordered (index থাকে)

Mutable (পরিবর্তন করা যায়)

Duplicate values রাখতে পারে

একসাথে different data types রাখতে পারে

# Example: Different types in one list
my_list = [10, "apple", True, 5.5]
print(my_list)  # [10, 'apple', True, 5.5]

🔹 2. Indexing

Index হলো element-এর position number।
👉 Python list index 0 থেকে শুরু হয়।
👉 Negative index ব্যবহার করলে, শেষ থেকে গুনে নেয়া হয়।

numbers = [10, 20, 30, 40, 50]

print(numbers[0])   # 10 → প্রথম element
print(numbers[2])   # 30 → তৃতীয় element
print(numbers[-1])  # 50 → শেষ element
print(numbers[-2])  # 40 → শেষের আগের element


📌 IndexError: যদি ভুল index দিই, error আসবে।

print(numbers[10])  # ❌ IndexError

🔹 3. Slicing

Slicing ব্যবহার করে list থেকে একটি sub-list বের করা হয়।

👉 Format:

list[start:end:step]


start → কোথা থেকে শুরু (default = 0)

end → কোথায় থামবে (exclusive, মানে ওই index-এর আগে পর্যন্ত)

step → কয় ধাপে যাবে (default = 1)

numbers = [10, 20, 30, 40, 50, 60]

print(numbers[1:4])   # [20, 30, 40] (index 1 → 3)
print(numbers[:3])    # [10, 20, 30] (শুরু থেকে 2 পর্যন্ত)
print(numbers[2:])    # [30, 40, 50, 60] (index 2 থেকে শেষ পর্যন্ত)
print(numbers[-3:])   # [40, 50, 60] (শেষের 3 element)
print(numbers[::2])   # [10, 30, 50] (step = 2)
print(numbers[::-1])  # [60, 50, 40, 30, 20, 10] (উল্টোদিক)

🔹 4. List Methods
✅ (a) append() → শেষে নতুন item যোগ করে
fruits = ["apple", "banana"]
fruits.append("mango")
print(fruits)  # ['apple', 'banana', 'mango']

✅ (b) pop() → index দিয়ে item মুছে ফেলে

index না দিলে, ডিফল্টভাবে শেষের element মুছে দেয়

fruits = ["apple", "banana", "mango"]

fruits.pop()    # শেষ element মুছে যাবে
print(fruits)   # ['apple', 'banana']

fruits.pop(0)   # index 0 এর element মুছে যাবে
print(fruits)   # ['banana']

✅ (c) sort() → list কে সাজিয়ে দেয় (ascending / descending)
numbers = [40, 10, 30, 20]

numbers.sort()  
print(numbers)  # [10, 20, 30, 40]  (ascending)

numbers.sort(reverse=True)
print(numbers)  # [40, 30, 20, 10]  (descending)


⚠️ নোট: যদি list-এ string আর number একসাথে থাকে, তাহলে sort() কাজ করবে না → TypeError আসবে।

🟢 Bonus: কিছু Extra Method

insert(index, value) → নির্দিষ্ট index-এ item যোগ করে

remove(value) → value দিয়ে item মুছে দেয়

clear() → সব element মুছে দেয়

copy() → list এর কপি তৈরি করে

fruits = ["apple", "banana", "mango"]

fruits.insert(1, "orange")  
print(fruits)  # ['apple', 'orange', 'banana', 'mango']

fruits.remove("banana")
print(fruits)  # ['apple', 'orange', 'mango']

fruits.clear()
print(fruits)  # []
