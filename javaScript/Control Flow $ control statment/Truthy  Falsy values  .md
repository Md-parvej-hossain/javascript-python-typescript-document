# 🔑 JavaScript Truthy & Falsy Values

JavaScript এ কোনো value কে **boolean context** (যেমন `if` statement, condition) এ ব্যবহার করলে সেটা হয় **Truthy** অথবা **Falsy** হিসেবে বিবেচিত হয়।  

---

## ❌ Falsy Values
JavaScript এ মোট **৭টি falsy value** আছে:

- `false`
- `0`
- `-0`
- `0n` (BigInt zero)
- `""` (খালি string)
- `null`
- `undefined`
- `NaN`

📌 Example:
```javascript
if (0) {
  console.log("Truthy");
} else {
  console.log("Falsy");
}
// Output: Falsy


✅ Truthy Values

Falsy বাদে সবকিছু Truthy ধরা হয়। যেমনঃ

true

"hello" (string)

" " (স্পেস সহ string)

42 (number)

-5 (negative number)

3.14 (decimal)

[] (empty array)

{} (empty object)

function(){} (function)

📌 Example:

if ("hello") {
  console.log("Truthy");
} else {
  console.log("Falsy");
}
// Output: Truthy


⚡ Shortcut ব্যবহার
1. OR (||) Operator → প্রথম truthy value নেবে
let name = "" || "Guest";
console.log(name);  // Output: Guest

2. AND (&&) Operator → প্রথম falsy value নেবে
let age = 18 && "Adult";
console.log(age);  // Output: Adult

3. Double NOT (!!) → Boolean এ রূপান্তর
console.log(!!"hello");  // true
console.log(!!0);        // false


📝 সারাংশ

Falsy Values: false, 0, -0, 0n, "", null, undefined, NaN

Truthy Values: বাকি সবকিছু truthy

|| (OR): প্রথম truthy value রিটার্ন করে

&& (AND): প্রথম falsy value রিটার্ন করে

!!: Boolean এ রূপান্তর করে