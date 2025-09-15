🔹 JavaScript break এবং continue

JavaScript এ লুপ (for, while, do...while) এর মধ্যে break এবং continue ব্যবহার করা হয় লুপের flow নিয়ন্ত্রণ করতে।

## 1️⃣ break

👉 লুপের execution মধ‍্যেই থামিয়ে দিতে ব্যবহার হয়।

লুপের মধ্যে শর্ত পূরণ হলে বাকি iteration আর চালানো হয় না।

for (let i = 1; i <= 10; i++) {
  if (i === 5) {
    break; // লুপ থেমে যাবে
  }
  console.log(i);
}


## 2️⃣ continue

👉 লুপের current iteration বাদ দিয়ে পরের iteration এ চলে যায়।

for (let i = 1; i <= 5; i++) {
  if (i === 3) {
    continue; // 3 এ প্রিন্ট হবে না
  }
  console.log(i);
}

🔑 সারাংশ

| স্টেটমেন্ট | কাজ                                               |
| ---------- | ------------------------------------------------- |
| `break`    | লুপ থামাতে                                        |
| `continue` | Current iteration বাদ দিয়ে পরের iteration চালাতে |
