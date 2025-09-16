Python লুপ (Loop) বাংলায়

Python-এ লুপ ব্যবহার করি কোনো কাজ বারবার করার জন্য। মূলত দুই ধরনের লুপ আছে:

for লুপ

while লুপ

এছাড়াও loop control statements আছে: break, continue, pass।

1️⃣ for লুপ

for লুপ দিয়ে আমরা কোনো sequence (list, string, tuple, range) এর উপর iteration করি।

Syntax
for item in sequence:
    # কোড ব্লক

উদাহরণ

a) List এর উপর লুপ

fruits = ["আপেল", "কলা", "চেরি"]
for fruit in fruits:
    print(fruit)


b) String এর উপর লুপ

word = "Python"
for letter in word:
    print(letter)


c) range() দিয়ে লুপ

for i in range(5):  # 0 থেকে 4
    print(i)

for i in range(1, 6):  # 1 থেকে 5
    print(i)

for i in range(0, 10, 2):  # 0,2,4,6,8
    print(i)


d) Nested for লুপ (লুপের ভিতরে লুপ)

for i in range(1, 4):
    for j in range(1, 4):
        print(i, j)

2️⃣ while লুপ

while লুপ তখন পর্যন্ত চলে যতক্ষণ condition True থাকে।

Syntax
while condition:
    # কোড ব্লক

উদাহরণ
i = 1
while i <= 5:
    print(i)
    i += 1


a) Infinite loop (সাবধানে ব্যবহার করুন)

while True:
    print("Hello")
    break  # লুপ থামানোর জন্য


b) while + else

i = 1
while i <= 3:
    print(i)
    i += 1
else:
    print("লুপ শেষ")

3️⃣ Loop Control Statements

লুপের ভিতরে আমাদের নিয়ন্ত্রণের জন্য তিনটি keyword আছে:

a) break → লুপ বন্ধ করে দেয়

for i in range(5):
    if i == 3:
        break
    print(i)


b) continue → বর্তমান iteration skip করে পরের iteration এ চলে যায়

for i in range(5):
    if i == 2:
        continue
    print(i)


c) pass → কোনো কাজ করে না, placeholder হিসাবে ব্যবহার হয়

for i in range(5):
    if i == 3:
        pass
    print(i)

4️⃣ Nested Loop (লুপের ভিতরে লুপ)
for i in range(1, 4):
    for j in range(1, 3):
        print(f"i={i}, j={j}")

5️⃣ List Comprehension (One-line loop)
squares = [x**2 for x in range(5)]
print(squares)  # [0, 1, 4, 9, 16]

সারাংশ (Summary)
Loop / Keyword	ব্যবহার
for	list, string, tuple, range এর উপর iteration
while	condition True থাকা পর্যন্ত loop চালানো
break	লুপ বন্ধ করার জন্য
continue	বর্তমান iteration skip করার জন্য
pass	placeholder, কিছু না করার জন্য

💡 Tip: Python লুপ শিখতে হলে range() এবং list/string iteration ভালোভাবে প্র্যাকটিস করতে হবে।