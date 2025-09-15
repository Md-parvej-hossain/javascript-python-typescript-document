🐍 Python String Operations
🔹 1. String Slicing

String কে index ব্যবহার করে ভাগ/কেটে নেওয়া যায়।

👉 Indexing শুরু হয় 0 থেকে। Negative index দিয়ে পেছন দিক থেকে ধরা হয়।

text = "Python"

print(text[0])     # 'P' (প্রথম character)
print(text[1:4])   # 'yth' (index 1 থেকে 3 পর্যন্ত)
print(text[:3])    # 'Pyt' (শুরুর দিক থেকে index 2 পর্যন্ত)
print(text[2:])    # 'thon' (index 2 থেকে শেষ পর্যন্ত)
print(text[-1])    # 'n' (শেষ character)
print(text[-3:])   # 'hon' (শেষ 3 টা character)


🔹 2. String Formatting (old style, format())
(a) Old Style Formatting (%)

name = "Parvej"
age = 23
print("My name is %s and I am %d years old." % (name, age))
# My name is Parvej and I am 23 years old.

(b) str.format() Method

name = "Parvej"
age = 23
print("My name is {} and I am {} years old.".format(name, age))
print("My name is {0} and I am {1} years old.".format(name, age))
print("My name is {n} and I am {a} years old.".format(n=name, a=age))

🔹 3. f-Strings (Python 3.6+)

👉 সবচেয়ে modern ও সহজ উপায় string format করার জন্য।

name = "Parvej"
age = 23

print(f"My name is {name} and I am {age} years old.")
print(f"In 5 years, I will be {age + 5} years old.")

✅ Summary:

Slicing → String থেকে নির্দিষ্ট অংশ নেওয়া।

Formatting (% এবং format) → ভ্যালু string এর মধ্যে বসানো।

f-Strings → সবচেয়ে সহজ, সরাসরি {} এর মধ্যে expression/variable বসানো যায়।