# 🌐 JavaScript Conditionals:

JavaScript এ **Conditionals** ব্যবহার করা হয় কোনো **শর্ত (condition)** এর ভিত্তিতে কোড চালাতে।  
মানে, শর্ত **সত্য (true)** হলে একটা কাজ হবে, আর **মিথ্যা (false)** হলে অন্য কাজ হবে।  

---

## 1️⃣ if  
👉 শর্ত সত্য (true) হলে কোড চালায়।  

```javascript
let age = 20;

if (age >= 18) {
  console.log("তুমি ভোট দিতে পারবে।");
}
2️⃣ else if

👉 একাধিক শর্ত চেক করার জন্য ব্যবহার করা হয়।
let marks = 65;

if (marks >= 80) {
  console.log("A+");
} else if (marks >= 70) {
  console.log("A");
} else if (marks >= 60) {
  console.log("A-");
}



3️⃣ else

👉 যখন সব শর্ত মিথ্যা হয়, তখন else চালানো হয়।
let time = 20;

if (time < 12) {
  console.log("সুপ্রভাত");
} else if (time < 18) {
  console.log("শুভ অপরাহ্ন");
} else {
  console.log("শুভ সন্ধ্যা");
}


4️⃣ switch

👉 একই ভেরিয়েবলের একাধিক মান চেক করার জন্য ব্যবহার করা হয়।

let day = 4;

switch (day) {
  case 1:
    console.log("রবিবার");
    break;
  case 2:
    console.log("সোমবার");
    break;
  case 3:
    console.log("মঙ্গলবার");
    break;
  case 4:
    console.log("বুধবার");
    break;
  case 5:
    console.log("বৃহস্পতিবার");
    break;
  case 6:
    console.log("শুক্রবার");
    break;
  case 7:
    console.log("শনিবার");
    break;
  default:
    console.log("অজানা দিন");
}


📝 সারাংশ (Summary)

if → শর্ত সত্য হলে কোড চালাবে

else if → একাধিক শর্ত পরীক্ষা করার জন্য

else → সব শর্ত মিথ্যা হলে চালাবে

switch → একই ভেরিয়েবল এর জন্য অনেক condition থাকলে
