- [ ] Data Types (String, Number, Boolean, Null, Undefined, Symbol, BigInt) 

# 🔢 JavaScript Data Types

JavaScript এ দুটি ধরণের Data Types আছে:

1. **Primitive Data Types**
2. **Non-Primitive (Reference) Data Types**

---

## 🅰️ Primitive Data Types  

 Primitive মানে একটা মাত্র value রাখে, পরিবর্তনযোগ্য নয় (immutable)।

1. String

টেক্সট বা অক্ষর সংরক্ষণের জন্য ব্যবহার হয়।  
```javascript
let name = "Parvej";
let city = 'Comilla';
let sentence = `Hello, ${name}`;
console.log(name, city, sentence);

2. Number

সংখ্যা (integer + decimal) সংরক্ষণ করে।
let age = 25;
let price = 99.99;
console.log(age + price); // 124.99

3. Boolean
True বা False মান রাখে।
let isStudent = true;
let isMarried = false;
console.log(isStudent); // true

4. Null

ইচ্ছাকৃতভাবে খালি মান (empty value)।
let car = null;
console.log(car); // null

5. Undefined
কোনো মান assign না করলে।
let country;
console.log(country); // undefined

6. Symbol
Unique value তৈরি করতে ব্যবহার হয়।
let id1 = Symbol("id");
let id2 = Symbol("id");
console.log(id1 === id2); // false

7. BigInt
খুব বড় সংখ্যা (2^53 এর বেশি) রাখার জন্য।

let bigNumber = 1234567890123456789012345678901234567890n;
console.log(bigNumber + 10n);


## 🅱️ Non-Primitive Data Types

👉 Non-Primitive মানে হচ্ছে এমন ডেটা যা reference আকারে সংরক্ষিত হয়।
Primitive data type value সরাসরি রাখে, কিন্তু Non-Primitive data type address (reference) রাখে।

1. Object

Key-Value Pair আকারে data সংরক্ষণ করতে ব্যবহৃত হয়।


let person = {
  name: "Parvej",
  age: 25,
  city: "Comilla"
};

console.log(person.name);   // Parvej
console.log(person["age"]); // 25 

2. Array 

List আকারে data সংরক্ষণ করতে ব্যবহৃত হয়।

let fruits = ["Mango", "Apple", "Banana"];
console.log(fruits[0]); // Mango
console.log(fruits.length); // 3

3. Function

Reusable block of code, যা বারবার ব্যবহার করা যায়।

function greet(name) {
  return "Hello " + name;
}

console.log(greet("Parvej")); // Hello Parvej

