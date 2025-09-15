## JavaScript-এ variable (ভেরিয়েবল) হলো ডেটা সংরক্ষণের জন্য একটি নামকৃত কন্টেইনার।

এখানে আমরা যেকোনো মান (number, string, boolean, object ইত্যাদি) রাখতে পারি এবং
পরে সেই মান ব্যবহার বা পরিবর্তন করতে পারি।

1. Variable Declare করার উপায়

var → পুরোনো, function scoped।

let → আধুনিক, block scoped।

const → মান পরিবর্তন করা যায় না।

2. Naming Rules (ভেরিয়েবল নামকরণ)

✔ শুরু হবে letter / _ / $ দিয়ে।
✔ Space থাকবে না।
✔ Case-sensitive → Name ≠ name।
✔ Keyword ব্যবহার করা যাবে না (যেমন: let, if ইত্যাদি)।

3. Data Types in Variable

Variable-এ নানা ধরণের ডেটা রাখা যায়:

let name = "Parvej";     // String
let age = 25;            // Number
let isStudent = true;    // Boolean
let fruits = ["Mango","Apple"]; // Array
let person = {name:"Hiru", age:25}; // Object
let x = null;            // Null
let y;                   // Undefined

4. Scope (কোথায় Variable কাজ করে)

Global Scope → সব জায়গা থেকে access করা যায়।

Function Scope → function-এর ভিতরে সীমাবদ্ধ।

Block Scope → শুধু { } ব্লকের ভিতরে (let, const)।


5. Hoisting

JavaScript variable-কে উপরে টেনে নেয় (declare করে, কিন্তু মান assign করে না)।

console.log(a); // undefined
var a = 5;

কিন্তু let, const hoist হলেও আগে ব্যবহার করা যায় না (temporal dead zone)।

6. Re-declare & Re-assign

var a = 10;
var a = 20; // ✅ সম্ভব

let b = 10;
// let b = 20; ❌ Error (re-declare করা যাবে না)
b = 30;     // ✅ Re-assign করা যাবে

const c = 50;
// c = 60; ❌ Error (Re-assign সম্ভব নয়)


7. Constant vs Mutable Object

const person = {name:"Parvej", age:25};
person.age = 26; // ✅ object property পরিবর্তন করা যাবে
// person = {name:"Hiru"} ❌ পুরো object পরিবর্তন করা যাবে না


8. Best Practices

সবসময় let বা const ব্যবহার করো।

const বেশি ব্যবহার করো, শুধু প্রয়োজন হলে let।

Variable নাম meaningful দাও।
