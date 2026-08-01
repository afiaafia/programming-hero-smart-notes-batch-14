# 📘 Module 10: JavaScript Arrays

## 📖 Part 1 — Array Fundamentals

> **Programming Hero | Milestone 03 | Module 10**

---

# 📑 Table of Contents

- [What is an Array?](#what-is-an-array)
- [Why Do We Need Arrays?](#why-do-we-need-arrays)
- [Creating Arrays](#creating-arrays)
- [Array Syntax](#array-syntax)
- [Array Index](#array-index)
- [Accessing Elements](#accessing-elements)
- [Updating Elements](#updating-elements)
- [Array Length](#array-length)
- [Basic Examples](#basic-examples)
- [Array Methods](#array-methods)
- [`push()`](#push-method)
- [`pop()`](#pop-method)
- [`shift()`](#shift-method)
- [`unshift()`](#unshift-method)
- [`includes()`](#includes-method)
- [`indexOf()`](#indexof-method)
- [`slice()`](#slice-method)
- [`splice()`](#splice-method)
- [Looping Through Arrays](#looping-through-arrays)
- [`for` Loop with Arrays](#for-loop-with-arrays)
- [`for...of` Loop](#for-of-loop)
- [Sum of Array Elements](#sum-of-array-elements)
- [Find Maximum Value](#find-maximum-value)
- [Find Minimum Value](#find-minimum-value)
- [Count Even & Odd Numbers](#count-even-and-odd-numbers)
- [Search an Element](#search-an-element)
- [Real-World Problems](#real-world-problems)
- [Best Practices](#best-practices)
- [Common Beginner Mistakes](#common-beginner-mistakes)
- [Practice Tasks](#practice-tasks)
- [Interview Questions](#interview-questions)
- [What's Next?](#whats-next)

---

<a id="what-is-an-array"></a>

# What is an Array?

An **Array** is a special data structure in JavaScript used to store **multiple values in a single variable**.

Instead of creating separate variables for related data, we can store them together in an array.

### Without an Array

```js
let student1 = "Alice";
let student2 = "Bob";
let student3 = "Charlie";
```

### With an Array

```js
let students = ["Alice", "Bob", "Charlie"];
```

Using an array makes your code cleaner, more organized, and easier to manage.

---

<a id="why-do-we-need-arrays"></a>

# Why Do We Need Arrays?

Imagine you're building a student management system.

Without arrays:

```js
let student1 = "Alice";
let student2 = "Bob";
let student3 = "Charlie";
let student4 = "David";
let student5 = "Emma";
```

Managing hundreds of students like this would be difficult.

With an array:

```js
let students = ["Alice", "Bob", "Charlie", "David", "Emma"];
```

Now all related data is stored in one place.

### Common Uses of Arrays

- Storing student names
- Product lists
- Shopping carts
- Scores and marks
- User information
- Messages
- Todo lists

---

<a id="creating-arrays"></a>

# Creating Arrays

Arrays are created using **square brackets `[]`**.

### Empty Array

```js
let fruits = [];
```

---

### Array with Values

```js
let fruits = ["Apple", "Banana", "Orange"];
```

---

### Number Array

```js
let numbers = [10, 20, 30, 40];
```

---

### Mixed Data Types

JavaScript arrays can store different types of data.

```js
let data = ["Afia", 20, true, null];
```

Although this is allowed, it's generally better to keep similar types of data together for better readability.

---

<a id="array-syntax"></a>

# Array Syntax

General syntax:

```js
let arrayName = [value1, value2, value3];
```

Example:

```js
let colors = ["Red", "Green", "Blue"];
```

Arrays can contain:

- Strings
- Numbers
- Booleans
- Objects
- Other Arrays
- Even Functions

Example:

```js
let example = [
  "JavaScript",
  2026,
  true
];
```

---

<a id="array-index"></a>

# Array Index

Every element in an array has an **index**.

> **JavaScript arrays use Zero-Based Indexing.**

That means indexing starts from **0**, not **1**.

Example:

```js
let fruits = ["Apple", "Banana", "Orange"];
```

| Index | Value |
|------:|-------|
| 0 | Apple |
| 1 | Banana |
| 2 | Orange |

Visual representation:

```text
Index :   0        1         2
        --------------------------
Value : Apple | Banana | Orange
```

---

<a id="accessing-elements"></a>

# Accessing Elements

Use square brackets with the index number to access an element.

Syntax:

```js
arrayName[index]
```

Example:

```js
let fruits = ["Apple", "Banana", "Orange"];

console.log(fruits[0]);
console.log(fruits[1]);
console.log(fruits[2]);
```

Output:

```text
Apple
Banana
Orange
```

---

### Accessing an Invalid Index

```js
let fruits = ["Apple", "Banana"];

console.log(fruits[5]);
```

Output:

```text
undefined
```

If an index doesn't exist, JavaScript returns `undefined`.

---

<a id="updating-elements"></a>

# Updating Elements

Array elements can be changed using their index.

Example:

```js
let fruits = ["Apple", "Banana", "Orange"];

fruits[1] = "Mango";

console.log(fruits);
```

Output:

```text
["Apple", "Mango", "Orange"]
```

---

<a id="array-length"></a>

# Array Length

The `.length` property returns the total number of elements in an array.

Example:

```js
let fruits = ["Apple", "Banana", "Orange"];

console.log(fruits.length);
```

Output:

```text
3
```

Example:

```js
let numbers = [10, 20, 30, 40, 50];

console.log(numbers.length);
```

Output:

```text
5
```

---

<a id="basic-examples"></a>

# Basic Examples

## Example 1 — Student List

```js
let students = ["Alice", "Bob", "Charlie"];

console.log(students);
```

---

## Example 2 — Print the First Element

```js
let colors = ["Red", "Green", "Blue"];

console.log(colors[0]);
```

Output:

```text
Red
```

---

## Example 3 — Update an Element

```js
let numbers = [10, 20, 30];

numbers[2] = 100;

console.log(numbers);
```

Output:

```text
[10, 20, 100]
```

---

## Example 4 — Find Array Length

```js
let cities = ["Dhaka", "Chattogram", "Khulna", "Rajshahi"];

console.log(cities.length);
```

Output:

```text
4
```

---

# 💡 Tips

- Arrays are ideal for storing multiple related values.
- Remember that array indexing starts from **0**.
- Use meaningful variable names such as `students`, `products`, or `scores`.
- Access elements using their index.
- Use `.length` whenever you need the total number of elements.

---

# ✅ Key Takeaways

- An array stores multiple values in a single variable.
- Arrays are created using square brackets `[]`.
- JavaScript uses **zero-based indexing**.
- Elements are accessed using their index.
- Elements can be updated by assigning a new value.
- The `.length` property returns the number of elements in an array.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 2 — Array Methods**




# 📘 Module 10: JavaScript Arrays

## 📖 Part 2 — Array Methods

> **Programming Hero | Milestone 03 | Module 10**

---

<a id="array-methods"></a>

# Array Methods

JavaScript provides many built-in methods to work with arrays.

These methods allow us to:

- Add elements
- Remove elements
- Search for elements
- Copy arrays
- Modify arrays

Some methods change the original array, while others return a new array.

In this part, we'll learn the most commonly used array methods.

---

<a id="push-method"></a>

# `push()`

The `push()` method adds one or more elements to the **end** of an array.

### Syntax

```js
array.push(element1, element2, ...);
```

### Example

```js
let fruits = ["Apple", "Banana"];

fruits.push("Orange");

console.log(fruits);
```

Output:

```text
["Apple", "Banana", "Orange"]
```

---

### Add Multiple Elements

```js
let numbers = [10, 20];

numbers.push(30, 40);

console.log(numbers);
```

Output:

```text
[10, 20, 30, 40]
```

---

<a id="pop-method"></a>

# `pop()`

The `pop()` method removes the **last element** from an array.

### Syntax

```js
array.pop();
```

### Example

```js
let fruits = ["Apple", "Banana", "Orange"];

fruits.pop();

console.log(fruits);
```

Output:

```text
["Apple", "Banana"]
```

---

### Store the Removed Element

```js
let fruits = ["Apple", "Banana", "Orange"];

let removed = fruits.pop();

console.log(removed);
```

Output:

```text
Orange
```

---

<a id="shift-method"></a>

# `shift()`

The `shift()` method removes the **first element** from an array.

### Example

```js
let colors = ["Red", "Green", "Blue"];

colors.shift();

console.log(colors);
```

Output:

```text
["Green", "Blue"]
```

---

### Store the Removed Element

```js
let colors = ["Red", "Green", "Blue"];

let firstColor = colors.shift();

console.log(firstColor);
```

Output:

```text
Red
```

---

<a id="unshift-method"></a>

# `unshift()`

The `unshift()` method adds one or more elements to the **beginning** of an array.

### Example

```js
let colors = ["Green", "Blue"];

colors.unshift("Red");

console.log(colors);
```

Output:

```text
["Red", "Green", "Blue"]
```

---

### Add Multiple Elements

```js
let numbers = [30, 40];

numbers.unshift(10, 20);

console.log(numbers);
```

Output:

```text
[10, 20, 30, 40]
```

---

<a id="includes-method"></a>

# `includes()`

The `includes()` method checks whether an array contains a specific value.

It returns:

- `true` if the value exists.
- `false` otherwise.

### Syntax

```js
array.includes(value);
```

### Example

```js
let fruits = ["Apple", "Banana", "Orange"];

console.log(fruits.includes("Banana"));
```

Output:

```text
true
```

---

### Value Not Found

```js
let fruits = ["Apple", "Banana"];

console.log(fruits.includes("Mango"));
```

Output:

```text
false
```

---

<a id="indexof-method"></a>

# `indexOf()`

The `indexOf()` method returns the **index** of a value.

If the value does not exist, it returns **`-1`**.

### Syntax

```js
array.indexOf(value);
```

### Example

```js
let fruits = ["Apple", "Banana", "Orange"];

console.log(fruits.indexOf("Banana"));
```

Output:

```text
1
```

---

### Value Not Found

```js
let fruits = ["Apple", "Banana"];

console.log(fruits.indexOf("Mango"));
```

Output:

```text
-1
```

---

<a id="slice-method"></a>

# `slice()`

The `slice()` method returns a **portion of an array**.

It **does not modify** the original array.

### Syntax

```js
array.slice(start, end);
```

- `start` → Starting index (included)
- `end` → Ending index (excluded)

### Example

```js
let numbers = [10, 20, 30, 40, 50];

let result = numbers.slice(1, 4);

console.log(result);
```

Output:

```text
[20, 30, 40]
```

The original array remains unchanged.

---

<a id="splice-method"></a>

# `splice()`

The `splice()` method adds, removes, or replaces elements in an array.

Unlike `slice()`, it **modifies the original array**.

### Syntax

```js
array.splice(start, deleteCount, item1, item2, ...);
```

---

### Remove Elements

```js
let numbers = [10, 20, 30, 40];

numbers.splice(1, 2);

console.log(numbers);
```

Output:

```text
[10, 40]
```

---

### Add Elements

```js
let numbers = [10, 40];

numbers.splice(1, 0, 20, 30);

console.log(numbers);
```

Output:

```text
[10, 20, 30, 40]
```

---

### Replace Elements

```js
let fruits = ["Apple", "Banana", "Orange"];

fruits.splice(1, 1, "Mango");

console.log(fruits);
```

Output:

```text
["Apple", "Mango", "Orange"]
```

---

# `slice()` vs `splice()`

| `slice()` | `splice()` |
|------------|------------|
| Returns a new array | Modifies the original array |
| Original array remains unchanged | Original array changes |
| Used for copying a portion of an array | Used for adding, removing, or replacing elements |

---

# 📝 Practice Examples

## Example 1 — Add a New Student

```js
let students = ["Alice", "Bob"];

students.push("Charlie");

console.log(students);
```

---

## Example 2 — Remove the Last Score

```js
let scores = [80, 85, 90];

scores.pop();

console.log(scores);
```

---

## Example 3 — Check if a City Exists

```js
let cities = ["Dhaka", "Khulna", "Rajshahi"];

console.log(cities.includes("Dhaka"));
```

Output:

```text
true
```

---

## Example 4 — Copy Part of an Array

```js
let months = ["Jan", "Feb", "Mar", "Apr", "May"];

let spring = months.slice(1, 4);

console.log(spring);
```

Output:

```text
["Feb", "Mar", "Apr"]
```

---

# 💡 Tips

- Use `push()` and `pop()` when working with the end of an array.
- Use `shift()` and `unshift()` when working with the beginning of an array.
- Use `includes()` to check if a value exists.
- Use `indexOf()` to find the position of a value.
- Use `slice()` when you need a copy without changing the original array.
- Use `splice()` when you want to modify the original array.

---

# ✅ Key Takeaways

- `push()` adds elements to the end of an array.
- `pop()` removes the last element.
- `shift()` removes the first element.
- `unshift()` adds elements to the beginning.
- `includes()` checks whether a value exists.
- `indexOf()` returns the index of a value.
- `slice()` returns a new array without modifying the original.
- `splice()` modifies the original array by adding, removing, or replacing elements.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 3 — Looping Through Arrays**




# 📘 Module 10: JavaScript Arrays

## 📖 Part 3 — Looping Through Arrays

> **Programming Hero | Milestone 03 | Module 10**

---

<a id="looping-through-arrays"></a>

# Looping Through Arrays

One of the most common operations in JavaScript is **iterating through an array**.

Instead of accessing each element manually:

```js
console.log(fruits[0]);
console.log(fruits[1]);
console.log(fruits[2]);
```

we can use loops to process every element automatically.

Example:

```js
let fruits = ["Apple", "Banana", "Orange"];

for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
```

Output:

```text
Apple
Banana
Orange
```

---

<a id="for-loop-with-arrays"></a>

# `for` Loop with Arrays

The `for` loop is the most commonly used loop for iterating through arrays.

Example:

```js
let colors = ["Red", "Green", "Blue"];

for (let i = 0; i < colors.length; i++) {
  console.log(colors[i]);
}
```

Output:

```text
Red
Green
Blue
```

### Why Use `array.length`?

Instead of writing:

```js
for (let i = 0; i < 3; i++) {

}
```

use:

```js
for (let i = 0; i < colors.length; i++) {

}
```

This makes your code work correctly even if the array size changes.

---

<a id="for-of-loop"></a>

# `for...of` Loop

The `for...of` loop is a simpler way to iterate over array values.

Syntax:

```js
for (let element of array) {
  // code
}
```

Example:

```js
let fruits = ["Apple", "Banana", "Orange"];

for (let fruit of fruits) {
  console.log(fruit);
}
```

Output:

```text
Apple
Banana
Orange
```

### `for` vs `for...of`

| `for` Loop | `for...of` Loop |
|------------|-----------------|
| Uses index | Uses values directly |
| Better when index is needed | Better when only values are needed |
| More flexible | More readable |

---

<a id="sum-of-array-elements"></a>

# Sum of Array Elements

Loops are commonly used to calculate the total of all elements.

Example:

```js
let numbers = [10, 20, 30, 40];

let sum = 0;

for (let number of numbers) {
  sum += number;
}

console.log(sum);
```

Output:

```text
100
```

---

<a id="find-maximum-value"></a>

# Find Maximum Value

Example:

```js
let numbers = [15, 42, 8, 91, 37];

let max = numbers[0];

for (let number of numbers) {

  if (number > max) {
    max = number;
  }

}

console.log(max);
```

Output:

```text
91
```

---

<a id="find-minimum-value"></a>

# Find Minimum Value

Example:

```js
let numbers = [15, 42, 8, 91, 37];

let min = numbers[0];

for (let number of numbers) {

  if (number < min) {
    min = number;
  }

}

console.log(min);
```

Output:

```text
8
```

---

<a id="count-even-and-odd-numbers"></a>

# Count Even & Odd Numbers

## Count Even Numbers

```js
let numbers = [2, 7, 10, 15, 18, 21];

let evenCount = 0;

for (let number of numbers) {

  if (number % 2 === 0) {
    evenCount++;
  }

}

console.log(evenCount);
```

Output:

```text
3
```

---

## Count Odd Numbers

```js
let numbers = [2, 7, 10, 15, 18, 21];

let oddCount = 0;

for (let number of numbers) {

  if (number % 2 !== 0) {
    oddCount++;
  }

}

console.log(oddCount);
```

Output:

```text
3
```

---

<a id="search-an-element"></a>

# Search an Element

There are multiple ways to search for a value in an array.

### Using `includes()`

```js
let fruits = ["Apple", "Banana", "Orange"];

console.log(fruits.includes("Banana"));
```

Output:

```text
true
```

---

### Using `indexOf()`

```js
let fruits = ["Apple", "Banana", "Orange"];

console.log(fruits.indexOf("Orange"));
```

Output:

```text
2
```

---

### Using a Loop

```js
let fruits = ["Apple", "Banana", "Orange"];

let found = false;

for (let fruit of fruits) {

  if (fruit === "Banana") {
    found = true;
    break;
  }

}

console.log(found);
```

Output:

```text
true
```

---

<a id="real-world-problems"></a>

# Real-World Problems

## Example 1 — Print All Products

```js
let products = ["Laptop", "Mouse", "Keyboard"];

for (let product of products) {
  console.log(product);
}
```

---

## Example 2 — Calculate Total Marks

```js
let marks = [75, 82, 91, 88];

let total = 0;

for (let mark of marks) {
  total += mark;
}

console.log(total);
```

Output:

```text
336
```

---

## Example 3 — Find the Highest Score

```js
let scores = [72, 90, 85, 97, 81];

let highest = scores[0];

for (let score of scores) {

  if (score > highest) {
    highest = score;
  }

}

console.log(highest);
```

Output:

```text
97
```

---

## Example 4 — Count Passed Students

```js
let marks = [35, 62, 80, 28, 55];

let passed = 0;

for (let mark of marks) {

  if (mark >= 40) {
    passed++;
  }

}

console.log(passed);
```

Output:

```text
3
```

---

# 💡 Tips

- Use `for...of` when you only need array values.
- Use a `for` loop when you also need the index.
- Always use `.length` instead of hardcoding the array size.
- Initialize variables like `sum`, `count`, `max`, or `min` before the loop starts.
- Use `break` when you can stop searching early.

---

# ✅ Key Takeaways

- Loops make it easy to process every element in an array.
- `for` and `for...of` are the most common loops for arrays.
- Arrays can be used to calculate totals, find maximum or minimum values, and count specific elements.
- Searching can be done with `includes()`, `indexOf()`, or loops.
- Combining arrays and loops is a fundamental JavaScript skill.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 4 — Module Summary**




# 📘 Module 10: JavaScript Arrays

## 🎯 Part 4 — Module Summary

> **Programming Hero | Milestone 03 | Module 10**

---

# 📖 Module Summary

Congratulations! 🎉

You have completed **Module 10 – JavaScript Arrays**.

In this module, you learned how to store, manage, and manipulate collections of data using arrays. Arrays are one of the most commonly used data structures in JavaScript and are essential for building real-world applications.

You learned:

- What an Array is
- Why Arrays are useful
- Creating Arrays
- Array Index
- Accessing Elements
- Updating Elements
- Array Length
- Array Methods
- `push()`
- `pop()`
- `shift()`
- `unshift()`
- `includes()`
- `indexOf()`
- `slice()`
- `splice()`
- Looping through Arrays
- `for` Loop with Arrays
- `for...of` Loop
- Finding Maximum & Minimum Values
- Sum of Array Elements
- Searching Elements
- Real-World Array Problems

These concepts form the foundation for working with Objects, Functions, DOM Manipulation, and modern JavaScript.

---

<a id="best-practices"></a>

# 💡 Best Practices

- ✅ Use meaningful array names such as `students`, `products`, or `scores`.
- ✅ Use `.length` instead of hardcoding the array size.
- ✅ Prefer `for...of` when you only need array values.
- ✅ Use a `for` loop when the index is required.
- ✅ Keep arrays organized by storing similar types of data together.
- ✅ Choose the appropriate array method for the task.
- ✅ Write clean and readable code.

---

<a id="common-beginner-mistakes"></a>

# 🚫 Common Beginner Mistakes

## 1. Forgetting Zero-Based Indexing

❌ Wrong

```js
let fruits = ["Apple", "Banana", "Orange"];

console.log(fruits[1]); // Expecting Apple
```

Output:

```text
Banana
```

✅ Correct

```js
console.log(fruits[0]);
```

---

## 2. Accessing an Invalid Index

```js
let colors = ["Red", "Green"];

console.log(colors[5]);
```

Output:

```text
undefined
```

Always make sure the index exists.

---

## 3. Hardcoding Array Length

❌

```js
for (let i = 0; i < 3; i++) {
  console.log(numbers[i]);
}
```

✅

```js
for (let i = 0; i < numbers.length; i++) {
  console.log(numbers[i]);
}
```

Using `.length` makes the code work correctly even if the array changes.

---

## 4. Confusing `slice()` and `splice()`

- `slice()` returns a new array without changing the original.
- `splice()` modifies the original array.

Understanding this difference helps avoid unexpected bugs.

---

## 5. Forgetting That `indexOf()` Returns `-1`

```js
let fruits = ["Apple", "Banana"];

console.log(fruits.indexOf("Mango"));
```

Output:

```text
-1
```

Always check for `-1` before using the returned index.

---

<a id="practice-tasks"></a>

# 🎯 Practice Tasks

## Task 1

Create an array of five fruits and print the entire array.

---

## Task 2

Print the first and last elements of an array.

---

## Task 3

Replace the second element of an array with a new value.

---

## Task 4

Use:

- `push()`
- `pop()`
- `shift()`
- `unshift()`

on the same array and print the result after each operation.

---

## Task 5

Check whether an array contains `"JavaScript"` using `includes()`.

---

## Task 6

Find the index of `"Banana"` using `indexOf()`.

---

## Task 7

Use a loop to calculate the sum of all numbers in an array.

---

## Task 8

Find the largest number in an array.

---

## Task 9

Find the smallest number in an array.

---

## Task 10

Count how many even and odd numbers are present in an array.

---

<a id="interview-questions"></a>

# ❓ Interview Questions

### 1. What is an Array?

An array is a data structure that stores multiple values in a single variable.

---

### 2. What is Zero-Based Indexing?

In JavaScript, array indexing starts from `0` instead of `1`.

---

### 3. What does the `.length` property return?

It returns the total number of elements in an array.

---

### 4. What is the difference between `push()` and `unshift()`?

- `push()` adds elements to the end.
- `unshift()` adds elements to the beginning.

---

### 5. What is the difference between `pop()` and `shift()`?

- `pop()` removes the last element.
- `shift()` removes the first element.

---

### 6. What is the difference between `slice()` and `splice()`?

- `slice()` returns a new array without modifying the original.
- `splice()` modifies the original array.

---

### 7. When should you use a `for` loop instead of `for...of`?

Use a `for` loop when you need the index of each element or want more control over the iteration.

---

### 8. What does `includes()` return?

It returns `true` if the value exists in the array; otherwise, it returns `false`.

---

### 9. What does `indexOf()` return if a value is not found?

It returns `-1`.

---

<a id="whats-next"></a>

# 📚 What's Next?

In the next module, you'll learn about another essential JavaScript data structure:

- Objects
- Object Properties
- Accessing Object Values
- Updating Objects
- Nested Objects
- Object Methods
- `for...in` Loop
- Real-World Object Examples

Objects allow you to store data using **key-value pairs**, making them ideal for representing real-world entities such as users, products, and orders.

---

<div align="center">

### ⭐ If these notes helped you, consider giving this repository a star!

**Happy Coding! 🚀**

</div>
