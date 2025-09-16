* Python Nested Loops (নেস্টেড লুপ)

## Nested Loop মানে হলো একটি লুপের ভিতরে আরেকটি লুপ। এটি তখন ব্যবহার করা হয় যখন আমাদের মাল্টিপল লেয়ার বা Matrix-এর মতো ডেটা iterate করতে হয়।
1️⃣ Syntax
for outer_item in outer_sequence:
    for inner_item in inner_sequence:
        # কোড ব্লক

2️⃣ উদাহরণ (Example)
a) Simple Nested for loop
for i in range(1, 4):          # Outer loop
    for j in range(1, 4):      # Inner loop
        print(f"i={i}, j={j}")


Output:

i=1, j=1
i=1, j=2
i=1, j=3
i=2, j=1
i=2, j=2
i=2, j=3
i=3, j=1
i=3, j=2
i=3, j=3


ব্যাখ্যা:
Outer loop প্রতি iteration-এ, Inner loop পুরোপুরি execute হয়।

b) Nested while loop
i = 1
while i <= 3:
    j = 1
    while j <= 2:
        print(f"i={i}, j={j}")
        j += 1
    i += 1


Output:

i=1, j=1
i=1, j=2
i=2, j=1
i=2, j=2
i=3, j=1
i=3, j=2

c) Nested loop with list
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

for row in matrix:
    for num in row:
        print(num, end=" ")
    print()  # new line


Output:

1 2 3
4 5 6
7 8 9


ব্যাখ্যা:
Outer loop row ধরে iterate করছে, Inner loop row-এর প্রতিটি element print করছে।

3️⃣ Tips

Nested loop যত বেশি levels, execution time তত বেশি। তাই সতর্ক ব্যবহার করা উচিত।

Matrix, Table, বা Grid এর জন্য Nested loop খুব উপকারী।

Python list comprehension-এর মাধ্যমে অনেক simple nested loop এক লাইনে করা যায়।

💡 Python Nested Loop Summary Table

| Loop Type       | Example Use Case                         |
| --------------- | ---------------------------------------- |
| Nested for      | List, Tuple, String iterate              |
| Nested while    | Condition অনুযায়ী multi-level iteration |
| For + While mix | জটিল loop pattern তৈরি করার জন্য         |


