1️⃣ break

## break লুপকে তৎক্ষণাৎ বন্ধ করে দেয়।

Syntax
for i in range(5):
    if i == 3:
        break
    print(i)


ব্যাখ্যা:
যখন i == 3 হয়, লুপ থেমে যায়। তাই 3 থেকে পরের সংখ্যা print হয়নি।

2️⃣ continue

## continue লুপের বর্তমান iteration skip করে এবং পরবর্তী iteration এ চলে যায়।

Syntax
for i in range(5):
    if i == 2:
        continue
    print(i)


ব্যাখ্যা:
যখন i == 2, continue দিয়ে সেই চক্র skip করা হয়েছে। তাই 2 print হয়নি।

3️⃣ pass

## pass কিছুই করে না। এটি সাধারণত placeholder হিসেবে ব্যবহার করা হয়।

Syntax
for i in range(5):
    if i == 3:
        pass
    print(i)

ব্যাখ্যা:
pass কোনো কাজ করে না, শুধু কোড ব্লক খালি রাখতে দেয়।


সারসংক্ষেপ:
| Keyword    | ব্যবহার                                           |
| ---------- | ------------------------------------------------- |
| `break`    | লুপ **থামাতে** ব্যবহার হয়                        |
| `continue` | লুপের **বর্তমান iteration skip** করতে ব্যবহার     |
| `pass`     | লুপ বা function এর **placeholder** হিসেবে ব্যবহার |
