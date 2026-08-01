# 📘 Module 07: JavaScript Basics
## 🚀 Part 1 — Introduction to JavaScript

> **Programming Hero | Milestone 02 | Module 07**

---

# 📚 Table of Contents

- [What is JavaScript?](#-what-is-javascript)
- [Why Learn JavaScript?](#-why-learn-javascript)
- [Where Does JavaScript Run?](#-where-does-javascript-run)
- [JavaScript Engine](#-javascript-engine)
- [How JavaScript Works](#-how-javascript-works)
- [Ways to Run JavaScript](#-ways-to-run-javascript)
- [Internal vs External JavaScript](#-internal-vs-external-javascript)
- [console.log()](#-consolelog)
- [Comments](#-comments)
- [Variables](#-variables)
- [let](#-let)
- [const](#-const)
- [var (Legacy)](#-var-legacy)
- [let vs const vs var](#-let-vs-const-vs-var)
- [Variable Naming Rules](#-variable-naming-rules)
- [Naming Convention](#-naming-convention)
- [Data Types](#-data-types)
- [Primitive Data Types](#-primitive-data-types)
- [typeof Operator](#-typeof-operator)
- [Type Conversion](#-type-conversion)
- [Truthy & Falsy Values](#-truthy--falsy-values)
- [Operators](#-what-is-an-operator)
- [Arithmetic Operators](#-arithmetic-operators)
- [String Concatenation](#-string-concatenation)
- [Assignment Operators](#-assignment-operators)
- [Comparison Operators](#-comparison-operators)
- [== vs ===](#-vs-)
- [Logical Operators](#-logical-operators)
- [Increment & Decrement](#-increment--decrement)
- [Pre-Increment vs Post-Increment](#-pre-increment-vs-post-increment)
- [Operator Precedence](#-operator-precedence)
- [Practice Examples](#-practice-examples)
- [Common Beginner Mistakes](#-common-beginner-mistakes)
- [Best Practices](#-best-practices)
- [Practice Tasks](#-practice-tasks)
- [Interview Questions](#-interview-questions)
- [What's Next?](#-whats-next)

---

# 📌 What is JavaScript?

**JavaScript (JS)** is a **high-level**, **interpreted**, and **dynamic programming language** that makes websites **interactive**.

HTML creates the **structure**, CSS adds the **design**, and JavaScript adds the **functionality**.

### Example

| Technology | Purpose |
|------------|---------|
| HTML | Structure |
| CSS | Styling |
| JavaScript | Interactivity |

Without JavaScript, a website would mostly be static.

---

# 🤔 Why Learn JavaScript?

JavaScript is one of the most popular programming languages in the world.

### It allows you to build:

- 🌐 Interactive Websites
- 📱 Mobile Applications
- 💻 Desktop Applications
- 🖥 Backend Applications (Node.js)
- 🤖 AI & Automation Tools
- 🎮 Browser Games
- ☁ Cloud Functions

### Why developers love JavaScript

- Beginner-friendly
- Huge community
- Millions of libraries
- Works in every browser
- Can be used for both Frontend and Backend

---

# 🌍 Where Does JavaScript Run?

Originally, JavaScript only ran inside web browsers.

Today it can run in many environments.

### Browser

Examples:

- Google Chrome
- Microsoft Edge
- Firefox
- Safari

JavaScript inside the browser controls:

- Button clicks
- Forms
- Animations
- DOM Manipulation
- API Calls

### Outside the Browser

Using **Node.js**, JavaScript can run on your computer or server.

This allows developers to create:

- REST APIs
- Backend servers
- CLI Tools
- Automation scripts

---

# ⚙ JavaScript Engine

A browser cannot understand JavaScript directly.

Instead, it uses a **JavaScript Engine**.

The engine reads your JavaScript code, converts it into machine-understandable instructions, and executes it.

### Popular JavaScript Engines

| Browser | Engine |
|----------|--------|
| Chrome | V8 |
| Edge | V8 |
| Firefox | SpiderMonkey |
| Safari | JavaScriptCore |

---

# 🔄 How JavaScript Works

Basic flow:

```text
JavaScript Code
        ↓
JavaScript Engine
        ↓
Machine Instructions
        ↓
Output
```

Example:

```js
console.log("Hello World");
```

Output:

```text
Hello World
```

---

# 🛠 Ways to Run JavaScript

## 1. Browser Console ✅ (Best for Beginners)

Open Developer Tools.

Shortcut:

### Windows

```text
F12
or
Ctrl + Shift + I
```

Go to the **Console** tab.

Now write:

```js
console.log("Hello JavaScript");
```

---

## 2. HTML File

Create an HTML file.

```html
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript</title>
</head>
<body>

<script>
console.log("Hello");
</script>

</body>
</html>
```

---

## 3. External JavaScript File

Create a file:

```text
script.js
```

Example:

```js
console.log("Hello from script.js");
```

Connect it with HTML.

```html
<script src="script.js"></script>
```

---

# 📄 Internal vs External JavaScript

## Internal JavaScript

Written inside the HTML file.

Example:

```html
<script>
console.log("Internal JS");
</script>
```

### Advantages

- Easy for very small projects
- Quick testing

### Disadvantages

- Difficult to maintain
- Not reusable
- Makes HTML messy

---

## External JavaScript

Written in a separate `.js` file.

Example:

```html
<script src="script.js"></script>
```

### Advantages

- Clean code
- Reusable
- Easier debugging
- Better project organization

✅ This is the recommended approach for real-world projects.

---

# 🖥 console.log()

`console.log()` prints data to the browser console.

Example:

```js
console.log("Programming Hero");
```

Output:

```text
Programming Hero
```

Multiple values:

```js
console.log("Age:", 20);
```

---

# 💬 Comments

Comments are ignored by JavaScript.

They help explain the code.

## Single-line Comment

```js
// This is a comment
console.log("Hello");
```

## Multi-line Comment

```js
/*
This is
a multi-line
comment
*/
```

---

# 📦 Variables (Introduction)

A **variable** is a container used to store data.

Think of it like a labeled box.

Example:

```text
Name → Afia
Age → 20
Country → Bangladesh
```

In JavaScript:

```js
let name = "Afia";
```

Here,

- `let` → creates a variable
- `name` → variable name
- `"Afia"` → stored value

We'll learn `let`, `const`, and `var` in detail in **Part 2**.

---

# ✅ Key Takeaways

- JavaScript makes websites interactive.
- It runs inside browsers using a JavaScript Engine.
- It can also run outside the browser with Node.js.
- Use an external `.js` file for real projects.
- `console.log()` is used for debugging and displaying output.
- Comments improve code readability.
- Variables store data for later use.

---

➡ Continue to **Part 2 — Variables & Data Types**




# 📘 Module 07: JavaScript Basics
## 📦 Part 2 — Variables & Data Types

> **Programming Hero | Milestone 02 | Module 07**

---

# 📦 Variables

A **variable** is a named container used to store data.

You can think of it as a labeled box that holds a value.

Example:

```text
Name → Afia
Age → 20
Country → Bangladesh
```

In JavaScript:

```js
let name = "Afia";
```

Here,

- `let` → Keyword
- `name` → Variable Name
- `"Afia"` → Value

---

# 🔑 let

`let` is used to declare a variable whose value **can change later**.

Example:

```js
let city = "Dhaka";

city = "Manikganj";

console.log(city);
```

Output:

```text
Manikganj
```

### Use `let` when:

- The value may change.
- Counters
- User input
- Game score
- Loop variables

Example:

```js
let score = 0;

score = score + 10;
```

---

# 🔒 const

`const` is used when the value **should never be reassigned**.

Example:

```js
const country = "Bangladesh";

console.log(country);
```

Trying to change it:

```js
const country = "Bangladesh";

country = "India";
```

Output:

```text
TypeError: Assignment to constant variable.
```

### Use `const` when:

- PI value
- API URL
- Website name
- Fixed configuration
- Any value that should not change

Example:

```js
const PI = 3.1416;
```

---

# ⚠ var (Legacy)

Before ES6 (2015), developers mainly used `var`.

Today, `let` and `const` are preferred.

Example:

```js
var age = 20;
```

### Why `var` is avoided

- Function scoped
- Can be redeclared
- Hoisting can cause unexpected behavior
- Makes code harder to debug

Example:

```js
var x = 10;
var x = 20;

console.log(x);
```

Output:

```text
20
```

This is allowed with `var`, but **not** with `let` or `const`.

> 💡 In modern JavaScript, use **`const` by default**. Use **`let` only when the value needs to change**. Avoid using `var` in new projects.

---

# ⚖ let vs const vs var

| Feature | let | const | var |
|---------|-----|--------|------|
| Reassign Value | ✅ Yes | ❌ No | ✅ Yes |
| Redeclare | ❌ No | ❌ No | ✅ Yes |
| Scope | Block | Block | Function |
| Hoisted | ✅ Yes (TDZ) | ✅ Yes (TDZ) | ✅ Yes |
| Modern Use | ✅ Recommended | ✅ Recommended | ❌ Avoid |

---

# 📝 Variable Naming Rules

A variable name:

✅ Can contain

- Letters
- Numbers
- `_`
- `$`

Example:

```js
let userName;
let user_age;
let totalPrice;
let $price;
```

---

❌ Cannot

Start with a number

```js
let 10age;
```

Contain spaces

```js
let my name;
```

Use reserved keywords

```js
let let;
let const;
let function;
```

---

# 🏷 Naming Convention

Use **camelCase** in JavaScript.

✅ Good

```js
let firstName;
let lastName;
let totalPrice;
let userAge;
```

❌ Bad

```js
let firstname;
let FIRSTNAME;
let total_price;
```

---

# 📊 Data Types

A **Data Type** defines what kind of value is stored inside a variable.

Example:

```js
let age = 20;
```

Here,

`20` is a **Number**.

---

# 🌟 Primitive Data Types

JavaScript has **7 Primitive Data Types**.

| Data Type | Example |
|-----------|---------|
| String | `"Hello"` |
| Number | `25` |
| Boolean | `true` |
| Undefined | `undefined` |
| Null | `null` |
| BigInt | `123456789n` |
| Symbol | `Symbol()` |

---

## 1️⃣ String

Stores text.

```js
let name = "Afia";
```

---

## 2️⃣ Number

Stores integers and decimals.

```js
let age = 20;

let price = 99.99;
```

---

## 3️⃣ Boolean

Represents two values.

```js
true
false
```

Example:

```js
let isLoggedIn = true;
```

---

## 4️⃣ Undefined

A variable declared but not assigned a value.

```js
let age;

console.log(age);
```

Output:

```text
undefined
```

---

## 5️⃣ Null

Represents an intentionally empty value.

```js
let user = null;
```

---

## 6️⃣ BigInt

Used for very large integers.

```js
let big = 123456789123456789123n;
```

---

## 7️⃣ Symbol

Creates a unique identifier.

```js
let id = Symbol("id");
```

Mostly used in advanced JavaScript.

---

# 🔍 typeof Operator

`typeof` returns the data type of a value.

Example:

```js
let age = 20;

console.log(typeof age);
```

Output:

```text
number
```

More examples:

```js
typeof "Hello"
```

Output:

```text
string
```

```js
typeof true
```

Output:

```text
boolean
```

```js
typeof undefined
```

Output:

```text
undefined
```

```js
typeof null
```

Output:

```text
object
```

> ⚠ This is a historical bug in JavaScript. Although `typeof null` returns `"object"`, `null` is actually a primitive data type.

---

# 🔄 Type Conversion

Sometimes we need to convert one data type into another.

## Convert String → Number

```js
Number("25");
```

Output:

```text
25
```

---

## Convert Number → String

```js
String(25);
```

Output:

```text
"25"
```

---

## Convert to Boolean

```js
Boolean(1);
```

Output:

```text
true
```

```js
Boolean(0);
```

Output:

```text
false
```

---

# ✅ Truthy & Falsy Values

## Falsy Values

These values are treated as `false` in JavaScript:

- `false`
- `0`
- `-0`
- `0n`
- `""`
- `null`
- `undefined`
- `NaN`

Everything else is considered **Truthy**.

Example:

```js
Boolean("Hello");
```

Output:

```text
true
```

---

# ✅ Key Takeaways

- Variables store data.
- Use `const` by default.
- Use `let` when the value will change.
- Avoid `var` in modern JavaScript.
- JavaScript has 7 primitive data types.
- `typeof` is used to check a value's data type.
- Type conversion can be done using `Number()`, `String()`, and `Boolean()`.
- Understand the difference between Truthy and Falsy values.

---

➡ Continue to **Part 3 — Operators & Practice**




# 📘 Module 07: JavaScript Basics
## ⚡ Part 3 — Operators & Practice

> **Programming Hero | Milestone 02 | Module 07**

---

# ➕ What is an Operator?

An **operator** is a symbol that performs an operation on one or more values (operands).

Example:

```js
10 + 5
```

Here,

- `10` → Operand
- `+` → Operator
- `5` → Operand

---

# ➕ Arithmetic Operators

Arithmetic operators are used for mathematical calculations.

| Operator | Meaning | Example | Result |
|----------|---------|---------|--------|
| `+` | Addition | `10 + 5` | `15` |
| `-` | Subtraction | `10 - 5` | `5` |
| `*` | Multiplication | `10 * 5` | `50` |
| `/` | Division | `10 / 2` | `5` |
| `%` | Modulus (Remainder) | `10 % 3` | `1` |
| `**` | Exponentiation | `2 ** 3` | `8` |

Example:

```js
let a = 15;
let b = 4;

console.log(a + b);
console.log(a - b);
console.log(a * b);
console.log(a / b);
console.log(a % b);
```

---

# ➕ String Concatenation

The `+` operator also joins strings.

```js
let firstName = "Afia";
let lastName = "Mubassira";

console.log(firstName + " " + lastName);
```

Output:

```text
Afia Mubassira
```

---

# 📝 Assignment Operators

Assignment operators assign values to variables.

| Operator | Example | Meaning |
|----------|---------|---------|
| `=` | `x = 5` | Assign |
| `+=` | `x += 2` | `x = x + 2` |
| `-=` | `x -= 2` | `x = x - 2` |
| `*=` | `x *= 2` | `x = x * 2` |
| `/=` | `x /= 2` | `x = x / 2` |
| `%=` | `x %= 2` | `x = x % 2` |

Example:

```js
let score = 10;

score += 5;

console.log(score);
```

Output:

```text
15
```

---

# ⚖ Comparison Operators

Comparison operators compare two values and return a Boolean (`true` or `false`).

| Operator | Meaning |
|----------|---------|
| `==` | Equal (Loose) |
| `===` | Strict Equal |
| `!=` | Not Equal |
| `!==` | Strict Not Equal |
| `>` | Greater Than |
| `<` | Less Than |
| `>=` | Greater Than or Equal |
| `<=` | Less Than or Equal |

Example:

```js
console.log(10 > 5);
```

Output:

```text
true
```

---

## `==` vs `===`

### Loose Equality (`==`)

Compares values after type conversion.

```js
console.log(5 == "5");
```

Output:

```text
true
```

---

### Strict Equality (`===`)

Compares both value and data type.

```js
console.log(5 === "5");
```

Output:

```text
false
```

> ✅ Prefer `===` and `!==` in modern JavaScript because they avoid unexpected type coercion.

---

# 🔗 Logical Operators

Logical operators combine multiple conditions.

| Operator | Meaning |
|----------|---------|
| `&&` | AND |
| `||` | OR |
| `!` | NOT |

---

## AND (`&&`)

Returns `true` only if **both conditions** are true.

```js
let age = 20;

console.log(age > 18 && age < 30);
```

Output:

```text
true
```

---

## OR (`||`)

Returns `true` if **at least one condition** is true.

```js
let isStudent = false;
let hasID = true;

console.log(isStudent || hasID);
```

Output:

```text
true
```

---

## NOT (`!`)

Reverses a Boolean value.

```js
console.log(!true);
```

Output:

```text
false
```

---

# 🔼 Increment & Decrement

## Increment (`++`)

Increases a value by **1**.

```js
let count = 5;

count++;

console.log(count);
```

Output:

```text
6
```

---

## Decrement (`--`)

Decreases a value by **1**.

```js
let count = 5;

count--;

console.log(count);
```

Output:

```text
4
```

---

# ⚠ Pre-Increment vs Post-Increment

## Post-Increment (`x++`)

Returns the current value first, then increases it.

```js
let x = 5;

console.log(x++);
console.log(x);
```

Output:

```text
5
6
```

---

## Pre-Increment (`++x`)

Increases the value first, then returns it.

```js
let x = 5;

console.log(++x);
```

Output:

```text
6
```

---

# 🎯 Operator Precedence

JavaScript follows mathematical precedence rules.

Example:

```js
console.log(5 + 2 * 3);
```

Output:

```text
11
```

Because multiplication (`*`) is evaluated before addition (`+`).

Use parentheses to control execution order.

```js
console.log((5 + 2) * 3);
```

Output:

```text
21
```

---

# 💻 Practice Examples

## Example 1

```js
let price = 500;
let quantity = 3;

console.log(price * quantity);
```

Output:

```text
1500
```

---

## Example 2

```js
let age = 20;

console.log(age >= 18);
```

Output:

```text
true
```

---

## Example 3

```js
let marks = 85;

console.log(marks >= 80 && marks <= 100);
```

Output:

```text
true
```

---

## Example 4

```js
let username = "Afia";

console.log(typeof username);
```

Output:

```text
string
```

---

# 🚫 Common Beginner Mistakes

### ❌ Using `=` instead of `==` or `===`

Wrong:

```js
if (age = 18) {

}
```

Correct:

```js
if (age === 18) {

}
```

---

### ❌ Using `==` when `===` is expected

```js
5 == "5"
```

Although this returns `true`, using `===` is safer.

---

### ❌ Forgetting to declare variables

Wrong:

```js
age = 20;
```

Correct:

```js
let age = 20;
```

---

### ❌ Dividing by zero

```js
console.log(10 / 0);
```

Output:

```text
Infinity
```

---

# 🎯 Mini Practice

## Practice 1

Create two variables:

```js
let num1 = 20;
let num2 = 10;
```

Print:

- Addition
- Subtraction
- Multiplication
- Division
- Modulus

---

## Practice 2

Store your:

- Name
- Age
- Country

Print all values using `console.log()`.

---

## Practice 3

Check whether your age is greater than or equal to 18.

---

## Practice 4

Create a variable:

```js
const PI = 3.1416;
```

Print its data type using `typeof`.

---

# ✅ Key Takeaways

- Operators perform different types of operations on values.
- Arithmetic operators are used for calculations.
- Assignment operators update variable values.
- Comparison operators return Boolean values.
- Prefer `===` instead of `==`.
- Logical operators combine conditions.
- `++` and `--` increase or decrease values by one.
- Parentheses help control operator precedence.
- Practice is the best way to understand operators.

---

➡ Continue to **Part 4 — Module Summary & TOC**






# 📘 Module 07: JavaScript Basics
## 🎯 Part 4 — Module Summary & TOC

> **Programming Hero | Milestone 02 | Module 07**

---

# 📖 Module Summary

Congratulations! 🎉

You have completed the fundamentals of JavaScript. This module introduced the core concepts that every JavaScript developer should understand before moving to conditions, loops, functions, objects, arrays, and the DOM.

You learned:

- What JavaScript is
- Why JavaScript is important
- Where JavaScript runs
- JavaScript Engine
- Internal & External JavaScript
- `console.log()`
- Comments
- Variables
- `let`, `const`, `var`
- Primitive Data Types
- `typeof`
- Type Conversion
- Operators

These topics form the foundation of everything you'll learn in the upcoming modules.

---

# 🧠 Common Beginner Mistakes

## 1. Using `var` in modern JavaScript

❌ Avoid:

```js
var name = "Afia";
```

✅ Prefer:

```js
const name = "Afia";
```

or

```js
let name = "Afia";
```

---

## 2. Forgetting to declare variables

❌

```js
age = 20;
```

✅

```js
let age = 20;
```

---

## 3. Using `==` instead of `===`

❌

```js
5 == "5"
```

✅

```js
5 === "5"
```

---

## 4. Confusing `null` and `undefined`

```js
let age;

console.log(age);
```

Output:

```text
undefined
```

```js
let user = null;
```

`undefined` means **no value assigned**, while `null` means **an intentionally empty value**.

---

## 5. Giving poor variable names

❌

```js
let a;
let x;
let abc;
```

✅

```js
let totalPrice;
let userName;
let isLoggedIn;
```

Choose meaningful variable names to improve code readability.

---

# 💡 Best Practices

- ✅ Use `const` by default.
- ✅ Use `let` only when the value needs to change.
- ❌ Avoid `var` in modern projects.
- ✅ Use meaningful variable names.
- ✅ Use `===` instead of `==`.
- ✅ Keep your code clean and properly indented.
- ✅ Write comments only when they add useful context.
- ✅ Practice writing code instead of just reading notes.

---

# 🎯 Practice Tasks

## Task 1

Create variables for:

- Name
- Age
- Country
- Is Student

Print all values using `console.log()`.

---

## Task 2

Perform the following operations:

```text
25 + 5
25 - 5
25 * 5
25 / 5
25 % 5
```

---

## Task 3

Check the data type of the following values:

```js
"Programming Hero"
100
true
undefined
null
```

using `typeof`.

---

## Task 4

Convert:

```text
"100" → Number
100 → String
0 → Boolean
1 → Boolean
```

---

## Task 5

Predict the output before running the code.

```js
console.log(10 == "10");
console.log(10 === "10");
console.log(typeof null);
console.log(Boolean(""));
console.log(Boolean("JavaScript"));
```

---

# ❓ Interview Questions

### 1. What is JavaScript?

A high-level programming language used to make websites interactive.

---

### 2. What is the difference between HTML, CSS, and JavaScript?

- HTML → Structure
- CSS → Styling
- JavaScript → Functionality

---

### 3. What is the difference between `let`, `const`, and `var`?

- `let` → Can be reassigned
- `const` → Cannot be reassigned
- `var` → Legacy keyword (avoid in modern JavaScript)

---

### 4. What is a JavaScript Engine?

A program that executes JavaScript code inside browsers.

Example:

- V8
- SpiderMonkey
- JavaScriptCore

---

### 5. What does `typeof` do?

It returns the data type of a value.

---

### 6. Why should we prefer `===` over `==`?

Because `===` compares both **value** and **data type**, making comparisons more predictable.

---

### 7. What is the difference between `null` and `undefined`?

- `undefined` → Variable declared but not assigned a value.
- `null` → An intentionally empty value.

---

### 8. What are Truthy and Falsy values?

Falsy values:

```text
false
0
-0
0n
""
null
undefined
NaN
```

Everything else is Truthy.

---

# 📚 What's Next?

In the next module, you'll continue your JavaScript journey by learning concepts such as:

- Conditional Statements (`if`, `else`, `else if`)
- Nested Conditions
- Logical Problem Solving
- Loops
- More Hands-on Practice

---

# 🎉 Congratulations!

You have successfully completed **Module 07 – JavaScript Basics**.

Keep practicing every concept with small programs. Consistent practice is the fastest way to become confident in JavaScript.

---

<div align="center">

### ⭐ If these notes helped you, consider giving this repository a star!

**Happy Coding! 🚀**

</div>
