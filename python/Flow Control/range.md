# Python `range()` Function

এই ফাইলটি Python এর `range()` ফাংশন সম্পর্কে বিস্তারিত তথ্য দেয়।  

Python range() ফাংশন

range() ফাংশন মূলত নম্বরের একটি সিরিজ তৈরি করে। সাধারণত লুপের সাথে ব্যবহার করা হয়।
---

## **1️⃣ Syntax**
```python
range(stop)
range(start, stop)
range(start, stop, step)

Parameters:-

| Parameter | Description                                |
| --------- | ------------------------------------------ |
| start     | সিরিজের শুরু নম্বর (ডিফল্ট = 0)            |
| stop      | সিরিজের শেষ নম্বর (stop excluded)          |
| step      | প্রতি ধাপে কত করে বৃদ্ধি পাবে (ডিফল্ট = 1) |

2️⃣ Examples
a) range(stop)
for i in range(5):
    print(i)

    ব্যাখ্যা: 0 থেকে 4 পর্যন্ত সংখ্যাগুলো print হবে (stop excluded)।

b) range(start, stop)
for i in range(1, 6):
    print(i)

ব্যাখ্যা: start থেকে stop-1 পর্যন্ত সংখ্যা iterate হয়।

c) range(start, stop, step)
for i in range(0, 10, 2):
    print(i)

    ব্যাখ্যা: step=2 মানে প্রতি ধাপে 2 করে বৃদ্ধি।

d) Negative step (উল্টো ক্রমে)
for i in range(5, 0, -1):
    print(i)

    ব্যাখ্যা: step=-1 মানে সংখ্যা কমতে থাকবে।

e) range() কে list এ কনভার্ট করা
numbers = list(range(5))
print(numbers)


3️⃣ Summary

range(stop) → 0 থেকে stop-1 পর্যন্ত

range(start, stop) → start থেকে stop-1 পর্যন্ত

range(start, stop, step) → step অনুযায়ী iterate

💡 Tip:
range() লুপে, list, string বা tuple iteration এর জন্য খুবই গুরুত্বপূর্ণ। এটি Python প্রোগ্রামিং এ সবচেয়ে বেশি ব্যবহৃত হয়।