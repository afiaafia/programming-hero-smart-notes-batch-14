# 📘 Module 11: JavaScript Objects

## 📖 Part 1 — Object Fundamentals

> **Programming Hero | Milestone 03 | Module 11**

---

# 📑 Table of Contents

- [What is an Object?](#what-is-an-object)
- [Why Do We Need Objects?](#why-do-we-need-objects)
- [Creating Objects](#creating-objects)
- [Object Syntax](#object-syntax)
- [Key-Value Pairs](#key-value-pairs)
- [Accessing Properties](#accessing-properties)
- [Dot Notation](#dot-notation)
- [Bracket Notation](#bracket-notation)
- [Basic Examples](#basic-examples)
- [Updating Properties](#updating-properties)
- [Adding New Properties](#adding-new-properties)
- [Deleting Properties](#deleting-properties)
- [Nested Objects](#nested-objects)
- [Object Methods](#object-methods)
- [`Object.keys()`](#object-keys)
- [`Object.values()`](#object-values)
- [`for...in` Loop](#for-in-loop)
- [Looping Through Objects](#looping-through-objects)
- [Combining Arrays & Objects](#combining-arrays-and-objects)
- [Real-World Examples](#real-world-examples)
- [Mini Practice Problems](#mini-practice-problems)
- [Common Object Operations](#common-object-operations)
- [Best Practices](#best-practices)
- [Common Beginner Mistakes](#common-beginner-mistakes)
- [Practice Tasks](#practice-tasks)
- [Interview Questions](#interview-questions)
- [What's Next?](#whats-next)

---

<a id="what-is-an-object"></a>

# What is an Object?

An **Object** is a data structure used to store **related information as key-value pairs**.

Unlike an array, where data is accessed using an **index**, an object stores data using **keys (property names)**.

Example:

```js
let student = {
  name: "Alice",
  age: 20,
  grade: "A"
};
```

Here:

- `name`, `age`, and `grade` are **keys (properties)**.
- `"Alice"`, `20`, and `"A"` are their **values**.

Objects make it easier to represent real-world entities.

---

<a id="why-do-we-need-objects"></a>

# Why Do We Need Objects?

Imagine you're storing information about a student.

Without an object:

```js
let studentName = "Alice";
let studentAge = 20;
let studentGrade = "A";
```

These variables are related but stored separately.

Using an object:

```js
let student = {
  name: "Alice",
  age: 20,
  grade: "A"
};
```

Now all related information is grouped together.

### Common Uses of Objects

- User profiles
- Product information
- Student records
- Orders
- Cars
- Books
- API responses

---

<a id="creating-objects"></a>

# Creating Objects

Objects are created using **curly braces `{}`**.

### Empty Object

```js
let person = {};
```

---

### Object with Properties

```js
let person = {
  name: "Afia",
  age: 20,
  country: "Bangladesh"
};
```

---

### Object with Different Data Types

```js
let user = {
  name: "Alice",
  age: 22,
  isStudent: true,
  city: "Dhaka"
};
```

Objects can store different types of values.

---

<a id="object-syntax"></a>

# Object Syntax

General syntax:

```js
let objectName = {
  key1: value1,
  key2: value2,
  key3: value3
};
```

Example:

```js
let laptop = {
  brand: "Dell",
  model: "Inspiron",
  price: 65000
};
```

Each property consists of:

```text
key : value
```

Properties are separated by commas.

---

<a id="key-value-pairs"></a>

# Key-Value Pairs

An object is made up of **key-value pairs**.

Example:

```js
let book = {
  title: "JavaScript Basics",
  author: "John",
  pages: 250
};
```

| Key | Value |
|------|-------|
| `title` | `"JavaScript Basics"` |
| `author` | `"John"` |
| `pages` | `250` |

Each key should be unique within an object.

---

<a id="accessing-properties"></a>

# Accessing Properties

Object properties can be accessed in two ways:

- Dot Notation
- Bracket Notation

Example object:

```js
let student = {
  name: "Alice",
  age: 20,
  grade: "A"
};
```

---

<a id="dot-notation"></a>

# Dot Notation

Dot notation is the most common way to access object properties.

Syntax:

```js
objectName.propertyName
```

Example:

```js
let student = {
  name: "Alice",
  age: 20
};

console.log(student.name);
console.log(student.age);
```

Output:

```text
Alice
20
```

Use dot notation when the property name is known.

---

<a id="bracket-notation"></a>

# Bracket Notation

Bracket notation accesses properties using square brackets.

Syntax:

```js
objectName["propertyName"]
```

Example:

```js
let student = {
  name: "Alice",
  age: 20
};

console.log(student["name"]);
console.log(student["age"]);
```

Output:

```text
Alice
20
```

---

### When to Use Bracket Notation

Bracket notation is useful when the property name is stored in a variable.

Example:

```js
let student = {
  name: "Alice",
  age: 20
};

let key = "name";

console.log(student[key]);
```

Output:

```text
Alice
```

---

### Dot Notation vs Bracket Notation

| Dot Notation | Bracket Notation |
|--------------|------------------|
| `student.name` | `student["name"]` |
| Easy to read | More flexible |
| Property name must be written directly | Property name can come from a variable |

---

<a id="basic-examples"></a>

# Basic Examples

## Example 1 — Student Object

```js
let student = {
  name: "Alice",
  age: 20,
  department: "CSE"
};

console.log(student);
```

---

## Example 2 — Print a Property

```js
let car = {
  brand: "Toyota",
  model: "Corolla"
};

console.log(car.brand);
```

Output:

```text
Toyota
```

---

## Example 3 — Access Using Bracket Notation

```js
let phone = {
  brand: "Samsung",
  color: "Black"
};

console.log(phone["color"]);
```

Output:

```text
Black
```

---

## Example 4 — Using a Variable

```js
let laptop = {
  brand: "HP",
  ram: "16GB"
};

let property = "ram";

console.log(laptop[property]);
```

Output:

```text
16GB
```

---

# 💡 Tips

- Use objects to represent a single real-world entity.
- Store related information together.
- Use meaningful property names.
- Prefer dot notation when the property name is known.
- Use bracket notation when the property name comes from a variable.

---

# ✅ Key Takeaways

- An object stores data as **key-value pairs**.
- Objects are created using curly braces `{}`.
- Each property has a unique key and a corresponding value.
- Properties can be accessed using dot notation or bracket notation.
- Objects are ideal for representing structured, real-world data.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 2 — Working with Objects**




# 📘 Module 11: JavaScript Objects

## 📖 Part 2 — Working with Objects

> **Programming Hero | Milestone 03 | Module 11**

---

<a id="updating-properties"></a>

# Updating Properties

Object properties can be updated by assigning a new value.

### Using Dot Notation

```js
let student = {
  name: "Alice",
  age: 20
};

student.age = 21;

console.log(student);
```

Output:

```text
{
  name: "Alice",
  age: 21
}
```

---

### Using Bracket Notation

```js
let student = {
  name: "Alice",
  age: 20
};

student["age"] = 22;

console.log(student);
```

Output:

```text
{
  name: "Alice",
  age: 22
}
```

---

<a id="adding-new-properties"></a>

# Adding New Properties

New properties can be added to an existing object.

### Using Dot Notation

```js
let car = {
  brand: "Toyota"
};

car.model = "Corolla";

console.log(car);
```

Output:

```text
{
  brand: "Toyota",
  model: "Corolla"
}
```

---

### Using Bracket Notation

```js
let car = {
  brand: "Toyota"
};

car["year"] = 2024;

console.log(car);
```

Output:

```text
{
  brand: "Toyota",
  year: 2024
}
```

---

<a id="deleting-properties"></a>

# Deleting Properties

The `delete` keyword removes a property from an object.

### Syntax

```js
delete objectName.property;
```

### Example

```js
let student = {
  name: "Alice",
  age: 20,
  grade: "A"
};

delete student.grade;

console.log(student);
```

Output:

```text
{
  name: "Alice",
  age: 20
}
```

---

### Using Bracket Notation

```js
let phone = {
  brand: "Samsung",
  color: "Black"
};

delete phone["color"];

console.log(phone);
```

Output:

```text
{
  brand: "Samsung"
}
```

---

<a id="nested-objects"></a>

# Nested Objects

An object can contain another object as one of its properties.

Example:

```js
let student = {
  name: "Alice",
  age: 20,
  address: {
    city: "Dhaka",
    country: "Bangladesh"
  }
};

console.log(student);
```

---

### Access Nested Properties

```js
console.log(student.address.city);
console.log(student.address.country);
```

Output:

```text
Dhaka
Bangladesh
```

---

### Another Example

```js
let employee = {
  id: 101,
  personalInfo: {
    name: "Rahim",
    department: "HR"
  }
};

console.log(employee.personalInfo.name);
```

Output:

```text
Rahim
```

---

<a id="object-methods"></a>

# Object Methods

Objects can store functions as properties.

When a function is stored inside an object, it is called a **method**.

Example:

```js
let person = {
  name: "Alice",

  greet: function () {
    console.log("Hello!");
  }
};

person.greet();
```

Output:

```text
Hello!
```

---

### Another Example

```js
let calculator = {

  add: function (a, b) {
    return a + b;
  }

};

console.log(calculator.add(10, 20));
```

Output:

```text
30
```

---

<a id="object-keys"></a>

# `Object.keys()`

The `Object.keys()` method returns an array containing all the keys of an object.

### Syntax

```js
Object.keys(objectName);
```

Example:

```js
let student = {
  name: "Alice",
  age: 20,
  grade: "A"
};

console.log(Object.keys(student));
```

Output:

```text
["name", "age", "grade"]
```

---

<a id="object-values"></a>

# `Object.values()`

The `Object.values()` method returns an array containing all the values of an object.

### Syntax

```js
Object.values(objectName);
```

Example:

```js
let student = {
  name: "Alice",
  age: 20,
  grade: "A"
};

console.log(Object.values(student));
```

Output:

```text
["Alice", 20, "A"]
```

---

# `Object.keys()` vs `Object.values()`

| `Object.keys()` | `Object.values()` |
|-----------------|-------------------|
| Returns property names | Returns property values |
| Output is an array of keys | Output is an array of values |

Example:

```js
let product = {
  name: "Laptop",
  price: 65000
};

console.log(Object.keys(product));
console.log(Object.values(product));
```

Output:

```text
["name", "price"]

["Laptop", 65000]
```

---

# 📝 Practice Examples

## Example 1 — Update a Property

```js
let user = {
  name: "Afia",
  age: 20
};

user.age = 21;

console.log(user);
```

---

## Example 2 — Add a New Property

```js
let book = {
  title: "JavaScript Basics"
};

book.author = "John";

console.log(book);
```

---

## Example 3 — Delete a Property

```js
let laptop = {
  brand: "Dell",
  ram: "16GB",
  color: "Silver"
};

delete laptop.color;

console.log(laptop);
```

---

## Example 4 — Print All Keys

```js
let country = {
  name: "Bangladesh",
  capital: "Dhaka",
  currency: "Taka"
};

console.log(Object.keys(country));
```

Output:

```text
["name", "capital", "currency"]
```

---

## Example 5 — Print All Values

```js
let country = {
  name: "Bangladesh",
  capital: "Dhaka",
  currency: "Taka"
};

console.log(Object.values(country));
```

Output:

```text
["Bangladesh", "Dhaka", "Taka"]
```

---

# 💡 Tips

- Use dot notation for known property names.
- Use bracket notation when the property name comes from a variable.
- Group related data using nested objects.
- Use methods to define object behavior.
- Use `Object.keys()` and `Object.values()` when you need all keys or values.

---

# ✅ Key Takeaways

- Object properties can be updated or added at any time.
- The `delete` keyword removes properties from an object.
- Objects can contain other objects.
- Objects can also contain functions called methods.
- `Object.keys()` returns all property names.
- `Object.values()` returns all property values.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 3 — Iterating Through Objects**





# 📘 Module 11: JavaScript Objects

## 📖 Part 3 — Iterating Through Objects

> **Programming Hero | Milestone 03 | Module 11**

---

<a id="for-in-loop"></a>

# `for...in` Loop

The `for...in` loop is used to iterate through the **properties (keys)** of an object.

### Syntax

```js
for (let key in objectName) {
  // code
}
```

Example:

```js
let student = {
  name: "Alice",
  age: 20,
  grade: "A"
};

for (let key in student) {
  console.log(key);
}
```

Output:

```text
name
age
grade
```

---

# Access Property Values

To access the value of each property, use bracket notation.

```js
let student = {
  name: "Alice",
  age: 20,
  grade: "A"
};

for (let key in student) {
  console.log(student[key]);
}
```

Output:

```text
Alice
20
A
```

---

# Print Both Keys and Values

```js
let student = {
  name: "Alice",
  age: 20,
  grade: "A"
};

for (let key in student) {
  console.log(key, ":", student[key]);
}
```

Output:

```text
name : Alice
age : 20
grade : A
```

---

<a id="looping-through-objects"></a>

# Looping Through Objects

Objects can also be traversed using `Object.keys()` and `Object.values()`.

---

### Using `Object.keys()`

```js
let car = {
  brand: "Toyota",
  model: "Corolla",
  year: 2024
};

let keys = Object.keys(car);

for (let key of keys) {
  console.log(key);
}
```

Output:

```text
brand
model
year
```

---

### Using `Object.values()`

```js
let car = {
  brand: "Toyota",
  model: "Corolla",
  year: 2024
};

let values = Object.values(car);

for (let value of values) {
  console.log(value);
}
```

Output:

```text
Toyota
Corolla
2024
```

---

### Print Keys and Values Together

```js
let product = {
  name: "Laptop",
  price: 65000,
  stock: 25
};

let keys = Object.keys(product);

for (let key of keys) {
  console.log(key, ":", product[key]);
}
```

Output:

```text
name : Laptop
price : 65000
stock : 25
```

---

<a id="combining-arrays-and-objects"></a>

# Combining Arrays & Objects

Arrays and objects are often used together in real-world applications.

Example:

```js
let students = [
  {
    name: "Alice",
    age: 20
  },
  {
    name: "Bob",
    age: 22
  },
  {
    name: "Charlie",
    age: 21
  }
];
```

Print all student names:

```js
for (let student of students) {
  console.log(student.name);
}
```

Output:

```text
Alice
Bob
Charlie
```

---

### Another Example

```js
let products = [
  {
    name: "Laptop",
    price: 65000
  },
  {
    name: "Mouse",
    price: 800
  }
];

for (let product of products) {
  console.log(product.name, "-", product.price);
}
```

Output:

```text
Laptop - 65000
Mouse - 800
```

---

<a id="real-world-examples"></a>

# Real-World Examples

## Example 1 — Print User Information

```js
let user = {
  name: "Afia",
  age: 20,
  country: "Bangladesh"
};

for (let key in user) {
  console.log(key + ": " + user[key]);
}
```

Output:

```text
name: Afia
age: 20
country: Bangladesh
```

---

## Example 2 — Student Database

```js
let students = [
  {
    name: "Alice",
    grade: "A"
  },
  {
    name: "Bob",
    grade: "B"
  }
];

for (let student of students) {
  console.log(student.name, "-", student.grade);
}
```

Output:

```text
Alice - A
Bob - B
```

---

## Example 3 — Product List

```js
let products = [
  {
    name: "Laptop",
    price: 65000
  },
  {
    name: "Keyboard",
    price: 2500
  },
  {
    name: "Mouse",
    price: 800
  }
];

for (let product of products) {
  console.log(product.name);
}
```

Output:

```text
Laptop
Keyboard
Mouse
```

---

<a id="mini-practice-problems"></a>

# Mini Practice Problems

## Problem 1 — Print All Object Keys

```js
let person = {
  name: "Rahim",
  age: 25,
  city: "Dhaka"
};

for (let key in person) {
  console.log(key);
}
```

---

## Problem 2 — Print All Object Values

```js
let person = {
  name: "Rahim",
  age: 25,
  city: "Dhaka"
};

for (let key in person) {
  console.log(person[key]);
}
```

---

## Problem 3 — Print Keys and Values

```js
let book = {
  title: "JavaScript",
  pages: 300
};

for (let key in book) {
  console.log(key, ":", book[key]);
}
```

---

<a id="common-object-operations"></a>

# Common Object Operations

| Operation | Example |
|-----------|---------|
| Create an object | `let user = {}` |
| Read a property | `user.name` |
| Update a property | `user.name = "Afia"` |
| Add a property | `user.country = "Bangladesh"` |
| Delete a property | `delete user.age` |
| Get all keys | `Object.keys(user)` |
| Get all values | `Object.values(user)` |
| Loop through properties | `for (let key in user)` |

---

# 💡 Tips

- Use `for...in` to iterate through object properties.
- Use bracket notation inside a `for...in` loop to access property values.
- Use `Object.keys()` or `Object.values()` when you need arrays of keys or values.
- Arrays and objects are often used together in real-world projects.
- Keep object structures simple and meaningful.

---

# ✅ Key Takeaways

- `for...in` loops through the keys of an object.
- Property values are accessed using `object[key]` inside a loop.
- `Object.keys()` returns an array of keys.
- `Object.values()` returns an array of values.
- Arrays and objects are commonly combined to represent structured data.
- Understanding objects is essential for working with APIs, JSON, and modern JavaScript.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 4 — Module Summary**





# 📘 Module 11: JavaScript Objects

## 🎯 Part 4 — Module Summary

> **Programming Hero | Milestone 03 | Module 11**

---

# 📖 Module Summary

Congratulations! 🎉

You have completed **Module 11 – JavaScript Objects**.

In this module, you learned how to store and manage related data using objects. Unlike arrays, which organize data by index, objects organize data using **key-value pairs**, making them ideal for representing real-world entities.

You learned:

- What an Object is
- Why Objects are useful
- Creating Objects
- Object Syntax
- Key-Value Pairs
- Accessing Properties
- Dot Notation
- Bracket Notation
- Updating Properties
- Adding New Properties
- Deleting Properties
- Nested Objects
- Object Methods
- `Object.keys()`
- `Object.values()`
- `for...in` Loop
- Looping Through Objects
- Combining Arrays & Objects
- Real-World Object Examples

These concepts are fundamental for working with APIs, JSON, DOM Manipulation, and modern JavaScript applications.

---

<a id="best-practices"></a>

# 💡 Best Practices

- ✅ Use meaningful property names.
- ✅ Group related data inside a single object.
- ✅ Prefer dot notation when the property name is known.
- ✅ Use bracket notation when the property name comes from a variable.
- ✅ Keep object structures clean and easy to understand.
- ✅ Use nested objects only when necessary.
- ✅ Use `Object.keys()` and `Object.values()` when working with collections of object data.

---

<a id="common-beginner-mistakes"></a>

# 🚫 Common Beginner Mistakes

## 1. Confusing Arrays and Objects

❌ Wrong

```js
let student = {
  name: "Alice",
  age: 20
};

console.log(student[0]);
```

Output:

```text
undefined
```

Objects use **property names**, not numeric indexes.

✅ Correct

```js
console.log(student.name);
```

---

## 2. Forgetting Quotes in Bracket Notation

❌

```js
student[name];
```

JavaScript treats `name` as a variable.

✅

```js
student["name"];
```

---

## 3. Using Dot Notation with Variables

❌

```js
let key = "age";

console.log(student.key);
```

Output:

```text
undefined
```

✅

```js
console.log(student[key]);
```

---

## 4. Forgetting the `delete` Keyword

❌

```js
student.age;
```

This only accesses the property.

✅

```js
delete student.age;
```

---

## 5. Expecting `Object.keys()` to Return Values

```js
let user = {
  name: "Afia",
  age: 20
};

console.log(Object.keys(user));
```

Output:

```text
["name", "age"]
```

Remember:

- `Object.keys()` → Keys
- `Object.values()` → Values

---

<a id="practice-tasks"></a>

# 🎯 Practice Tasks

## Task 1

Create an object that stores:

- Name
- Age
- Country

Print the entire object.

---

## Task 2

Print the value of the `name` property using:

- Dot notation
- Bracket notation

---

## Task 3

Update the `age` property.

Print the updated object.

---

## Task 4

Add a new property called `profession`.

---

## Task 5

Delete the `country` property.

---

## Task 6

Print all property names using `Object.keys()`.

---

## Task 7

Print all property values using `Object.values()`.

---

## Task 8

Use a `for...in` loop to print:

```text
key : value
```

---

## Task 9

Create an object containing another object.

Print one nested property.

---

## Task 10

Create an array of three student objects and print the name of each student.

---

<a id="interview-questions"></a>

# ❓ Interview Questions

### 1. What is an Object?

An object is a data structure that stores related data as **key-value pairs**.

---

### 2. What is the difference between an Array and an Object?

- Arrays store data using numeric indexes.
- Objects store data using property names (keys).

---

### 3. What is the difference between dot notation and bracket notation?

- Dot notation is used when the property name is known.
- Bracket notation is useful when the property name is stored in a variable.

---

### 4. How do you update an object property?

```js
object.property = newValue;
```

or

```js
object["property"] = newValue;
```

---

### 5. How do you delete a property?

Use the `delete` keyword.

```js
delete object.property;
```

---

### 6. What does `Object.keys()` return?

It returns an array containing all property names (keys).

---

### 7. What does `Object.values()` return?

It returns an array containing all property values.

---

### 8. What is a nested object?

A nested object is an object stored inside another object.

---

### 9. What is an object method?

An object method is a function stored as a property inside an object.

---

### 10. Which loop is commonly used to iterate through object properties?

The `for...in` loop.

---

<a id="whats-next"></a>

# 📚 What's Next?

In the next module, you'll learn about **JavaScript Functions**, one of the most powerful concepts in programming.

You'll explore topics such as:

- What is a Function?
- Function Declaration
- Function Parameters
- Function Arguments
- Return Statement
- Function Scope
- Built-in Functions
- Real-World Function Examples

Functions help you write reusable, organized, and maintainable code.

---

<div align="center">

### ⭐ If these notes helped you, consider giving this repository a star!

**Happy Coding! 🚀**

</div>
