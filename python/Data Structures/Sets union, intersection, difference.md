🐍 Python Sets — Union, Intersection, Difference
🔹 1. Set কী?

Set হলো Python-এর একটা unordered collection যেখানে unique elements থাকে।
👉 অর্থাৎ, একই value দুইবার রাখা যায় না।

numbers = {10, 20, 30, 20, 40}
print(numbers)   # {40, 10, 20, 30} → duplicate মুছে গেছে

🔹 2. Set বানানোর নিয়ম
# set literal
s1 = {1, 2, 3}

# set() constructor
s2 = set([4, 5, 6])

print(s1)  # {1, 2, 3}
print(s2)  # {4, 5, 6}


⚠️ নোট: Empty set বানাতে হলে {} ব্যবহার করা যাবে না (ওটা dictionary হবে)।

empty = set()
print(type(empty))  # <class 'set'>

🔹 3. Union (মিলিত করা)

👉 দুটি set-এর সব element একত্রিত করে, কিন্তু duplicate বাদ দিয়ে।

a = {1, 2, 3}
b = {3, 4, 5}

print(a.union(b))   # {1, 2, 3, 4, 5}
print(a | b)        # {1, 2, 3, 4, 5} (shortcut)

🔹 4. Intersection (সাধারণ অংশ)

👉 দুটি set-এর মধ্যে যে elements common আছে, শুধু সেগুলো রাখে।

a = {1, 2, 3}
b = {2, 3, 4}

print(a.intersection(b))   # {2, 3}
print(a & b)               # {2, 3} (shortcut)

🔹 5. Difference (ভিন্ন অংশ)

👉 এক set-এর মধ্যে যা আছে কিন্তু অন্যটাতে নাই।

a = {1, 2, 3, 4}
b = {3, 4, 5}

print(a.difference(b))   # {1, 2} → a - b
print(b.difference(a))   # {5}   → b - a

# shortcut
print(a - b)   # {1, 2}
print(b - a)   # {5}

🔹 6. Extra: Symmetric Difference

👉 দুই সেটের মধ্যে যে element গুলো একটাতে আছে কিন্তু দুটোতেই নাই।

a = {1, 2, 3}
b = {3, 4, 5}

print(a.symmetric_difference(b))  # {1, 2, 4, 5}
print(a ^ b)                      # {1, 2, 4, 5} (shortcut)


✅ সংক্ষেপে:

Union → সব element (duplicate ছাড়া)

Intersection → common element

Difference → ভিন্ন element (a - b)

Symmetric Difference → শুধু আলাদা element, common বাদ দিয়ে

ভাই, তুমি কি চাও আমি Lists, Tuples আর Sets — এই তিনটার ব্যাখ্যা একসাথে একটা সুন্দর README.md ফরম্যাটে বানিয়ে দিই তোমার জন্য?

You said:
more explain
ChatGPT said:

ঠিক আছে ভাই 🙂 এখন আমি Python Sets নিয়ে আরও ডিটেইলসে বুঝিয়ে দিচ্ছি — যেন তুমি একেবারে ভালোভাবে বুঝতে পারো।

🐍 Python Sets — Deep Explanation
🔹 1. Set কী?

Set হলো unordered collection → মানে কোনো fixed order থাকে না।

সব element unique হয় (duplicate element automatically বাদ হয়ে যায়)।

Mutable → set-এ নতুন element যোগ করা যায়, element মুছে ফেলা যায়।

কিন্তু set-এর ভিতরের element immutable হতে হবে (যেমন string, int, tuple), mutable (যেমন list, dictionary) রাখা যাবে না।

# Example: set with numbers
s = {10, 20, 30, 20, 10}
print(s)  # {10, 20, 30} (duplicate বাদ গেছে)

# Example: set with mixed data
s2 = {1, "apple", (2, 3)}
print(s2)  # {1, 'apple', (2, 3)}

🔹 2. Set তৈরি করার নিয়ম
# Normal set
s1 = {1, 2, 3}

# Using set() function
s2 = set([4, 5, 6])

# Empty set
empty = set()   # ✅ Correct
wrong = {}      # ❌ এটা আসলে dict, set না

🔹 3. Set Indexing / Slicing

👉 List বা Tuple-এর মতো set-এ indexing বা slicing করা যায় না কারণ set unordered।

s = {1, 2, 3}
print(s[0])   # ❌ Error


👉 তবে loop দিয়ে element access করা যায়।

for item in {10, 20, 30}:
    print(item)

🔹 4. Set Operations
✅ (a) Union → সব element যোগ করা (duplicate বাদ দিয়ে)

👉 দুটি বা একাধিক set মিলে নতুন set তৈরি হয়।

a = {1, 2, 3}
b = {3, 4, 5}

print(a.union(b))   # {1, 2, 3, 4, 5}
print(a | b)        # shortcut

✅ (b) Intersection → common elements (যা দুইটাতে আছে)
a = {1, 2, 3}
b = {2, 3, 4}

print(a.intersection(b))  # {2, 3}
print(a & b)              # shortcut

✅ (c) Difference → একটাতে আছে, অন্যটাতে নাই
a = {1, 2, 3, 4}
b = {3, 4, 5}

print(a.difference(b))  # {1, 2} → a - b
print(b.difference(a))  # {5}   → b - a

# shortcut
print(a - b)   # {1, 2}
print(b - a)   # {5}

✅ (d) Symmetric Difference → শুধু ভিন্ন element (common বাদ দিয়ে)
a = {1, 2, 3}
b = {3, 4, 5}

print(a.symmetric_difference(b))  # {1, 2, 4, 5}
print(a ^ b)                      # shortcut

🔹 5. Set Methods
Method	কাজ
add(x)	set-এ নতুন element যোগ করে
update(iterable)	multiple elements যোগ করে
remove(x)	element মুছে ফেলে (না থাকলে error দেয়)
discard(x)	element মুছে ফেলে (না থাকলে error দেয় না)
pop()	random element মুছে ফেলে
clear()	সব element মুছে ফেলে
copy()	set-এর shallow copy তৈরি করে
s = {1, 2, 3}
s.add(4)  
print(s)  # {1, 2, 3, 4}

s.update([5, 6])  
print(s)  # {1, 2, 3, 4, 5, 6}

s.remove(2)  
print(s)  # {1, 3, 4, 5, 6}

s.discard(10)  # error দিবে না

s.pop()  # random একটা element মুছে ফেলবে

🔹 6. Practical Uses of Sets

Duplicate remove করার জন্য

nums = [1, 2, 2, 3, 4, 4, 5]
unique_nums = set(nums)
print(unique_nums)  # {1, 2, 3, 4, 5}


Membership test (খুব ফাস্ট)

fruits = {"apple", "banana", "mango"}
print("apple" in fruits)   # True
print("orange" in fruits)  # False


Mathematical set operations (union, intersection, difference)

✅ সংক্ষেপে:

Set → unique, unordered collection

Union → সব element

Intersection → common element

Difference → ভিন্ন element

Symmetric Difference → শুধু unique element