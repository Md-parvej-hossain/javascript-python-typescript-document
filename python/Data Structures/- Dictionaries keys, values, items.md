🐍 Python Dictionaries — Keys, Values, Items, get(), update()
🔹 1. Dictionary কী?

Dictionary হলো key-value pair এর collection।
👉 প্রতিটি data একটা key এর সাথে map হয়।
👉 Key অবশ্যই unique আর immutable হতে হবে (যেমন: string, number, tuple)।

# Example dictionary
student = {
    "name": "Parvej",
    "age": 22,
    "city": "Comilla"
}

print(student)
# {'name': 'Parvej', 'age': 22, 'city': 'Comilla'}

🔹 2. Keys

Dictionary-র keys() মেথড সবগুলো key রিটার্ন করে।

student = {"name": "Parvej", "age": 22, "city": "Comilla"}

print(student.keys())  
# dict_keys(['name', 'age', 'city'])

# loop দিয়ে access
for key in student.keys():
    print(key)

🔹 3. Values

Dictionary-র values() মেথড সব value রিটার্ন করে।

print(student.values())  
# dict_values(['Parvej', 22, 'Comilla'])

for value in student.values():
    print(value)

🔹 4. Items

Dictionary-র items() মেথড key-value pair একসাথে tuple আকারে দেয়।

print(student.items())  
# dict_items([('name', 'Parvej'), ('age', 22), ('city', 'Comilla')])

for key, value in student.items():
    print(key, ":", value)

🔹 5. get() মেথড

👉 সরাসরি dict[key] ব্যবহার করলে যদি key না থাকে তাহলে KeyError আসবে।
👉 কিন্তু get() ব্যবহার করলে error না দিয়ে default value রিটার্ন করবে।

print(student.get("name"))       # Parvej
print(student.get("age"))        # 22
print(student.get("country"))    # None (key নেই তাই None রিটার্ন হলো)
print(student.get("country", "Bangladesh"))  # Bangladesh (default value)

🔹 6. update() মেথড

👉 এক dictionary-তে অন্য dictionary যোগ করতে, অথবা value আপডেট করতে ব্যবহার করা হয়।

student.update({"age": 23})  
print(student)  
# {'name': 'Parvej', 'age': 23, 'city': 'Comilla'}

student.update({"country": "Bangladesh"})  
print(student)  
# {'name': 'Parvej', 'age': 23, 'city': 'Comilla', 'country': 'Bangladesh'}

🔹 7. Extra Dictionary Methods
Method	কাজ
pop(key)	নির্দিষ্ট key মুছে ফেলে
popitem()	random key-value pair মুছে ফেলে
clear()	পুরো dictionary খালি করে
copy()	dictionary এর shallow copy তৈরি করে
student.pop("city")
print(student)  

| Method               | কাজ                          |
| -------------------- | ---------------------------- |
| `dict.keys()`        | সব keys return করে           |
| `dict.values()`      | সব values return করে         |
| `dict.items()`       | সব key-value pair return করে |
| `dict.update({...})` | নতুন data add/update করে     |
| `dict.pop(key)`      | নির্দিষ্ট key remove করে     |
| `dict.clear()`       | পুরো dictionary খালি করে     |


# {'name': 'Parvej', 'age': 23, 'country': 'Bangladesh'}

student.clear()
print(student)  # {}


✅ সংক্ষেপে:

keys() → সব key

values() → সব value

items() → সব key-value pair

get(key, default) → নিরাপদে value পাওয়া যায়

update() → নতুন key যোগ বা পুরাতন key আপডেট