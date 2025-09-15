- [ ] Operators (+, -, *, /, %, **, ==, ===, !=, !==, &&, ||, ternary)  

# ⚡ JavaScript Operators

Operators হলো বিশেষ চিহ্ন বা keyword যা **মান (values) এর উপর কাজ করতে ব্যবহৃত হয়**।

🅰️ Arithmetic Operators (গাণিতিক)
🅱️ Assignment Operators (মান অ্যাসাইন করা)
🅲 Comparison Operators (তুলনা করা)
🅳 Logical Operators (যুক্তি)
🅴 Unary Operators (একটি মানের উপর কাজ করে)
🅵 Ternary Operator (Shortcut if else)
🅶 Type Operators


---

## 🅰️ Arithmetic Operators (গাণিতিক)
```javascript
let a = 10;
let b = 3;

console.log(a + b);  // 13 (Addition)
console.log(a - b);  // 7  (Subtraction)
console.log(a * b);  // 30 (Multiplication)
console.log(a / b);  // 3.33 (Division)
console.log(a % b);  // 1 (Modulus / Remainder)
console.log(a ** b); // 1000 (Exponent / Power)

🅱️ Assignment Operators (মান অ্যাসাইন করা)
let x = 5;

x += 2;  // 7   → x = x + 2
x -= 2;  // 5   → x = x - 2
x *= 2;  // 10  → x = x * 2
x /= 2;  // 5   → x = x / 2
x %= 2;  // 1   → x = x % 2
x **= 3; // 1   → x = x ** 3

🅲 Comparison Operators (তুলনা করা)
let a = 10;
let b = 5;

console.log(a == b);     // false  (value equal)
console.log(a != b);     // true   (not equal)
console.log(a === 10);   // true   (value + type equal)
console.log(a !== "10"); // true   (value or type not equal)
console.log(a > b);      // true
console.log(a < b);      // false
console.log(a >= 10);    // true
console.log(a <= 5);     // false

🅳 Logical Operators (যুক্তি)
let isStudent = true;
let isAdult = false;

console.log(isStudent && isAdult); // false (AND → দুটোই true হলে true)
console.log(isStudent || isAdult); // true  (OR → যেকোনো একটি true হলে true)
console.log(!isStudent);           // false (NOT → উল্টো করে দেয়)

🅴 Unary Operators (একটি মানের উপর কাজ করে)
let a = 5;

console.log(++a); // 6 (pre-increment → আগে বাড়ায়)
console.log(a++); // 6 (post-increment → পরে বাড়ায়)
console.log(a);   // 7

console.log(--a); // 6 (pre-decrement → আগে কমায়)
console.log(a--); // 6 (post-decrement → পরে কমায়)
console.log(a);   // 5

🅵 Ternary Operator (Shortcut if else)
let age = 18;
let result = (age >= 18) ? "Adult" : "Child";
console.log(result); // Adult

🅶 Type Operators
let name = "Parvej";
console.log(typeof name); // string

let number = 25;
console.log(typeof number); // number
