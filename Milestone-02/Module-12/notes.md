# 📘 Module 12: JavaScript Functions

## 📖 Part 1 — Function Fundamentals

> **Programming Hero | Milestone 03 | Module 12**

---

# 📑 Table of Contents

- [What is a Function?](#what-is-a-function)
- [Why Do We Need Functions?](#why-do-we-need-functions)
- [Function Declaration](#function-declaration)
- [Function Syntax](#function-syntax)
- [Calling a Function](#calling-a-function)
- [Function Naming Convention](#function-naming-convention)
- [Basic Examples](#basic-examples)
- [Parameters](#parameters)
- [Arguments](#arguments)
- [Single Parameter](#single-parameter)
- [Multiple Parameters](#multiple-parameters)
- [Default Parameters](#default-parameters)
- [Return Statement](#return-statement)
- [`console.log()` vs `return`](#console-log-vs-return)
- [Function Examples](#function-examples)
- [Local Scope](#local-scope)
- [Global Scope](#global-scope)
- [Variable Scope](#variable-scope)
- [Function Reusability](#function-reusability)
- [Real-World Examples](#real-world-examples)
- [Mini Practice Problems](#mini-practice-problems)
- [Common Function Patterns](#common-function-patterns)
- [Best Practices](#best-practices)
- [Common Beginner Mistakes](#common-beginner-mistakes)
- [Practice Tasks](#practice-tasks)
- [Interview Questions](#interview-questions)
- [What's Next?](#whats-next)

---

<a id="what-is-a-function"></a>

# What is a Function?

A **Function** is a reusable block of code that performs a specific task.

Instead of writing the same code multiple times, you can write it once inside a function and use it whenever needed.

Example:

```js
function greet() {
  console.log("Hello, World!");
}
```

The function above stores a piece of reusable code.

---

<a id="why-do-we-need-functions"></a>

# Why Do We Need Functions?

Imagine you need to print the same welcome message five times.

Without a function:

```js
console.log("Welcome!");
console.log("Welcome!");
console.log("Welcome!");
console.log("Welcome!");
console.log("Welcome!");
```

The same code is repeated again and again.

Using a function:

```js
function welcome() {
  console.log("Welcome!");
}

welcome();
welcome();
welcome();
welcome();
welcome();
```

This approach is:

- Easier to read
- Easier to maintain
- Reusable
- Less repetitive

---

<a id="function-declaration"></a>

# Function Declaration

A function declaration defines a function using the `function` keyword.

### Syntax

```js
function functionName() {
  // code
}
```

Example:

```js
function sayHello() {
  console.log("Hello!");
}
```

The function is created, but it will not run until it is called.

---

<a id="function-syntax"></a>

# Function Syntax

A function has four main parts:

```js
function greet() {
  console.log("Hello!");
}
```

| Part | Description |
|------|-------------|
| `function` | Keyword used to declare a function |
| `greet` | Function name |
| `()` | Parameter list |
| `{}` | Function body |

Visual representation:

```text
function greet() {
    // Function Body
}
```

---

<a id="calling-a-function"></a>

# Calling a Function

After creating a function, you must **call (invoke)** it to execute the code inside.

Example:

```js
function greet() {
  console.log("Hello!");
}

greet();
```

Output:

```text
Hello!
```

---

### Calling Multiple Times

One function can be called as many times as needed.

```js
function welcome() {
  console.log("Welcome!");
}

welcome();
welcome();
welcome();
```

Output:

```text
Welcome!
Welcome!
Welcome!
```

---

### Calling Different Functions

```js
function greet() {
  console.log("Hello!");
}

function goodbye() {
  console.log("Goodbye!");
}

greet();
goodbye();
```

Output:

```text
Hello!
Goodbye!
```

---

<a id="function-naming-convention"></a>

# Function Naming Convention

Choose function names that clearly describe what the function does.

### Good Examples

```js
function calculateTotal() {}

function printInvoice() {}

function getUserName() {}

function checkPassword() {}
```

These names explain the purpose of the function.

---

### Poor Examples

```js
function abc() {}

function test() {}

function data() {}
```

These names do not describe the function's purpose.

---

### Use Camel Case

Function names should follow **camelCase**.

```js
function calculateArea() {}

function findLargestNumber() {}

function sendEmail() {}
```

Avoid spaces and special characters in function names.

---

<a id="basic-examples"></a>

# Basic Examples

## Example 1 — Greeting Function

```js
function greet() {
  console.log("Hello, JavaScript!");
}

greet();
```

Output:

```text
Hello, JavaScript!
```

---

## Example 2 — Print a Message

```js
function printMessage() {
  console.log("Learning Functions");
}

printMessage();
```

Output:

```text
Learning Functions
```

---

## Example 3 — Call a Function Multiple Times

```js
function welcome() {
  console.log("Welcome!");
}

welcome();
welcome();
welcome();
```

Output:

```text
Welcome!
Welcome!
Welcome!
```

---

## Example 4 — Two Different Functions

```js
function start() {
  console.log("Program Started");
}

function end() {
  console.log("Program Finished");
}

start();
end();
```

Output:

```text
Program Started
Program Finished
```

---

# 💡 Tips

- Think of a function as a reusable machine that performs one specific task.
- Write a function once and call it whenever needed.
- Keep functions focused on a single responsibility.
- Use meaningful and descriptive function names.
- Follow the camelCase naming convention.

---

# ✅ Key Takeaways

- A function is a reusable block of code.
- Functions are declared using the `function` keyword.
- A function does not run until it is called.
- A function can be called multiple times.
- Good function names make code easier to understand.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 2 — Parameters, Arguments & Return**





# 📘 Module 12: JavaScript Functions

## 📖 Part 2 — Parameters, Arguments & Return

> **Programming Hero | Milestone 03 | Module 12**

---

<a id="parameters"></a>

# Parameters

A **parameter** is a variable declared in a function definition.

It acts as a placeholder that receives values when the function is called.

### Syntax

```js
function functionName(parameter) {
  // code
}
```

Example:

```js
function greet(name) {
  console.log("Hello,", name);
}
```

Here, `name` is a **parameter**.

---

<a id="arguments"></a>

# Arguments

An **argument** is the actual value passed to a function when it is called.

Example:

```js
function greet(name) {
  console.log("Hello,", name);
}

greet("Alice");
```

Output:

```text
Hello, Alice
```

Here:

- `name` → Parameter
- `"Alice"` → Argument

---

### Parameter vs Argument

| Parameter | Argument |
|-----------|----------|
| Variable in the function definition | Actual value passed to the function |
| Created when declaring the function | Provided when calling the function |

Example:

```js
function greet(name) {
  console.log(name);
}

greet("Afia");
```

- `name` → Parameter
- `"Afia"` → Argument

---

<a id="single-parameter"></a>

# Single Parameter

A function can receive one parameter.

Example:

```js
function square(number) {
  console.log(number * number);
}

square(5);
```

Output:

```text
25
```

---

### Another Example

```js
function printCountry(country) {
  console.log(country);
}

printCountry("Bangladesh");
```

Output:

```text
Bangladesh
```

---

<a id="multiple-parameters"></a>

# Multiple Parameters

A function can receive multiple parameters separated by commas.

Example:

```js
function add(a, b) {
  console.log(a + b);
}

add(10, 20);
```

Output:

```text
30
```

---

### Another Example

```js
function introduce(name, age) {
  console.log(name, "is", age, "years old.");
}

introduce("Alice", 20);
```

Output:

```text
Alice is 20 years old.
```

---

<a id="default-parameters"></a>

# Default Parameters

A parameter can have a default value.

If no argument is provided, the default value is used.

### Syntax

```js
function functionName(parameter = defaultValue) {

}
```

Example:

```js
function greet(name = "Guest") {
  console.log("Hello,", name);
}

greet();
greet("Alice");
```

Output:

```text
Hello, Guest
Hello, Alice
```

---

<a id="return-statement"></a>

# Return Statement

The `return` statement sends a value back from a function.

Syntax:

```js
function functionName() {
  return value;
}
```

Example:

```js
function add(a, b) {
  return a + b;
}

let result = add(10, 20);

console.log(result);
```

Output:

```text
30
```

---

### Return Ends the Function

When JavaScript reaches a `return` statement, the function stops executing.

```js
function test() {
  console.log("Start");

  return;

  console.log("End");
}

test();
```

Output:

```text
Start
```

The last `console.log()` never runs.

---

<a id="console-log-vs-return"></a>

# `console.log()` vs `return`

Both are useful, but they serve different purposes.

### Using `console.log()`

```js
function add(a, b) {
  console.log(a + b);
}

add(10, 20);
```

Output:

```text
30
```

The value is displayed but cannot be reused.

---

### Using `return`

```js
function add(a, b) {
  return a + b;
}

let sum = add(10, 20);

console.log(sum);
```

Output:

```text
30
```

The returned value can be stored, reused, or passed to another function.

---

### Difference

| `console.log()` | `return` |
|-----------------|----------|
| Displays output in the console | Sends a value back from the function |
| Cannot be reused directly | Can be stored in a variable |
| Mainly used for debugging | Used to produce results |

---

<a id="function-examples"></a>

# Function Examples

## Example 1 — Add Two Numbers

```js
function add(a, b) {
  return a + b;
}

console.log(add(5, 8));
```

Output:

```text
13
```

---

## Example 2 — Multiply Two Numbers

```js
function multiply(a, b) {
  return a * b;
}

console.log(multiply(6, 4));
```

Output:

```text
24
```

---

## Example 3 — Print a Greeting

```js
function greet(name) {
  console.log("Welcome,", name);
}

greet("Afia");
```

Output:

```text
Welcome, Afia
```

---

## Example 4 — Find the Larger Number

```js
function findLarger(a, b) {

  if (a > b) {
    return a;
  }

  return b;
}

console.log(findLarger(15, 25));
```

Output:

```text
25
```

---

## Example 5 — Calculate Rectangle Area

```js
function rectangleArea(length, width) {
  return length * width;
}

console.log(rectangleArea(8, 5));
```

Output:

```text
40
```

---

# 💡 Tips

- Parameters are variables; arguments are actual values.
- Use meaningful parameter names.
- Use default parameters when appropriate.
- Prefer `return` when the result needs to be reused.
- Use `console.log()` mainly for displaying output or debugging.

---

# ✅ Key Takeaways

- Parameters receive values inside a function.
- Arguments are the values passed when calling a function.
- A function can have one, multiple, or default parameters.
- The `return` statement sends a value back to the caller.
- `console.log()` displays output, while `return` produces reusable results.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 3 — Function Scope & Real-World Practice**





# 📘 Module 12: JavaScript Functions

## 📖 Part 3 — Function Scope & Real-World Practice

> **Programming Hero | Milestone 03 | Module 12**

---

<a id="local-scope"></a>

# Local Scope

A variable declared **inside a function** can only be accessed within that function.

This is called **Local Scope**.

Example:

```js
function greet() {
  let message = "Hello!";
  console.log(message);
}

greet();
```

Output:

```text
Hello!
```

Trying to access `message` outside the function will cause an error.

```js
console.log(message);
```

Output:

```text
ReferenceError: message is not defined
```

---

<a id="global-scope"></a>

# Global Scope

A variable declared **outside any function** is called a **Global Variable**.

It can be accessed from anywhere in the program.

Example:

```js
let country = "Bangladesh";

function showCountry() {
  console.log(country);
}

showCountry();

console.log(country);
```

Output:

```text
Bangladesh
Bangladesh
```

---

### Local vs Global Variables

```js
let language = "JavaScript";

function learn() {
  let topic = "Functions";

  console.log(language);
  console.log(topic);
}

learn();

console.log(language);
```

Output:

```text
JavaScript
Functions
JavaScript
```

Trying to print `topic` outside the function:

```js
console.log(topic);
```

Output:

```text
ReferenceError: topic is not defined
```

---

<a id="variable-scope"></a>

# Variable Scope

**Scope** determines where a variable can be accessed.

There are two main types:

| Scope | Accessible From |
|--------|-----------------|
| Global Scope | Anywhere |
| Local Scope | Inside its function only |

Example:

```js
let x = 10;

function demo() {
  let y = 20;

  console.log(x);
  console.log(y);
}

demo();
```

Output:

```text
10
20
```

---

### Scope Rules

- A local variable cannot be accessed outside its function.
- A function can access global variables.
- Different functions can have variables with the same name.

Example:

```js
function first() {
  let value = 10;
  console.log(value);
}

function second() {
  let value = 20;
  console.log(value);
}

first();
second();
```

Output:

```text
10
20
```

---

<a id="function-reusability"></a>

# Function Reusability

One of the biggest advantages of functions is **reusability**.

Instead of writing the same logic repeatedly, write it once and call it whenever needed.

Example:

```js
function square(number) {
  return number * number;
}

console.log(square(3));
console.log(square(7));
console.log(square(10));
```

Output:

```text
9
49
100
```

---

### Another Example

```js
function greet(name) {
  console.log("Hello,", name);
}

greet("Afia");
greet("Alice");
greet("Bob");
```

Output:

```text
Hello, Afia
Hello, Alice
Hello, Bob
```

---

<a id="real-world-examples"></a>

# Real-World Examples

## Example 1 — Calculate Discount

```js
function calculateDiscount(price, discount) {
  return price - discount;
}

console.log(calculateDiscount(1000, 150));
```

Output:

```text
850
```

---

## Example 2 — Check Adult

```js
function isAdult(age) {

  if (age >= 18) {
    return true;
  }

  return false;
}

console.log(isAdult(20));
```

Output:

```text
true
```

---

## Example 3 — Calculate Average

```js
function average(a, b, c) {
  return (a + b + c) / 3;
}

console.log(average(80, 90, 100));
```

Output:

```text
90
```

---

## Example 4 — Convert Minutes to Seconds

```js
function minutesToSeconds(minutes) {
  return minutes * 60;
}

console.log(minutesToSeconds(5));
```

Output:

```text
300
```

---

<a id="mini-practice-problems"></a>

# Mini Practice Problems

## Problem 1 — Square a Number

Create a function that returns the square of a number.

Example:

```js
square(6);
```

Output:

```text
36
```

---

## Problem 2 — Find the Largest Number

Create a function that returns the larger of two numbers.

Example:

```js
findLargest(20, 15);
```

Output:

```text
20
```

---

## Problem 3 — Check Even Number

Create a function that returns `true` if a number is even; otherwise, return `false`.

Example:

```js
isEven(12);
```

Output:

```text
true
```

---

## Problem 4 — Calculate Rectangle Area

Create a function that returns the area of a rectangle.

Example:

```js
rectangleArea(10, 5);
```

Output:

```text
50
```

---

<a id="common-function-patterns"></a>

# Common Function Patterns

## Function Without Parameters

```js
function hello() {
  console.log("Hello!");
}

hello();
```

---

## Function With Parameters

```js
function greet(name) {
  console.log(name);
}

greet("Afia");
```

---

## Function Returning a Value

```js
function add(a, b) {
  return a + b;
}

console.log(add(10, 20));
```

---

## Function Returning a Boolean

```js
function isPositive(number) {
  return number > 0;
}

console.log(isPositive(8));
```

Output:

```text
true
```

---

# 💡 Tips

- Keep each function focused on a single task.
- Use meaningful function and parameter names.
- Prefer `return` over `console.log()` when the result needs to be reused.
- Avoid creating unnecessary global variables.
- Reuse functions instead of duplicating code.

---

# ✅ Key Takeaways

- Local variables are accessible only inside their function.
- Global variables can be accessed throughout the program.
- Scope controls where variables can be used.
- Functions make code reusable and easier to maintain.
- Real-world programs rely heavily on reusable functions.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 4 — Module Summary**





# 📘 Module 12: JavaScript Functions

## 🎯 Part 4 — Module Summary

> **Programming Hero | Milestone 03 | Module 12**

---

# 📖 Module Summary

Congratulations! 🎉

You have completed **Module 12 – JavaScript Functions**.

Functions are one of the most important concepts in JavaScript. They allow you to organize code into reusable blocks, reduce repetition, and make programs easier to maintain.

In this module, you learned:

- What a Function is
- Why Functions are useful
- Function Declaration
- Function Syntax
- Calling a Function
- Function Naming Convention
- Parameters
- Arguments
- Single Parameter
- Multiple Parameters
- Default Parameters
- Return Statement
- `console.log()` vs `return`
- Local Scope
- Global Scope
- Variable Scope
- Function Reusability
- Real-World Function Examples

These concepts are the foundation for advanced JavaScript topics such as callbacks, arrow functions, asynchronous programming, and modern frameworks like React.

---

<a id="best-practices"></a>

# 💡 Best Practices

- ✅ Give every function a meaningful name.
- ✅ Keep each function focused on a single responsibility.
- ✅ Prefer `return` when a value needs to be reused.
- ✅ Use parameters instead of hardcoding values.
- ✅ Avoid unnecessary global variables.
- ✅ Keep functions short and readable.
- ✅ Reuse functions instead of duplicating code.

---

<a id="common-beginner-mistakes"></a>

# 🚫 Common Beginner Mistakes

## 1. Forgetting to Call the Function

❌ Wrong

```js
function greet() {
  console.log("Hello!");
}
```

The function is declared but never executed.

✅ Correct

```js
greet();
```

---

## 2. Confusing Parameters and Arguments

```js
function greet(name) {
  console.log(name);
}

greet("Afia");
```

Remember:

- `name` → Parameter
- `"Afia"` → Argument

---

## 3. Using `console.log()` Instead of `return`

❌

```js
function add(a, b) {
  console.log(a + b);
}

let result = add(5, 10);

console.log(result);
```

Output:

```text
15
undefined
```

Because `console.log()` only displays the value; it does not return it.

✅

```js
function add(a, b) {
  return a + b;
}
```

---

## 4. Accessing Local Variables Outside the Function

❌

```js
function test() {
  let message = "Hello";
}

console.log(message);
```

Output:

```text
ReferenceError
```

Local variables are only available inside the function.

---

## 5. Writing One Function for Multiple Tasks

❌

```js
function processData() {
  // hundreds of lines of code
}
```

Large functions are difficult to read and maintain.

✅ Split large tasks into smaller reusable functions.

---

<a id="practice-tasks"></a>

# 🎯 Practice Tasks

## Task 1

Create a function that prints:

```text
Hello, JavaScript!
```

---

## Task 2

Create a function that accepts a name and prints:

```text
Hello, <name>
```

---

## Task 3

Create a function that returns the sum of two numbers.

---

## Task 4

Create a function that returns the square of a number.

---

## Task 5

Create a function that returns the area of a rectangle.

---

## Task 6

Create a function that checks whether a number is even.

Return:

- `true` for even numbers
- `false` for odd numbers

---

## Task 7

Create a function that returns the largest of two numbers.

---

## Task 8

Create a function with a default parameter that prints:

```text
Hello, Guest
```

when no argument is provided.

---

## Task 9

Create a function that calculates the average of three numbers.

---

## Task 10

Write a reusable function that converts minutes into seconds.

---

<a id="interview-questions"></a>

# ❓ Interview Questions

### 1. What is a function?

A function is a reusable block of code designed to perform a specific task.

---

### 2. Why do we use functions?

Functions help reduce code duplication, improve readability, and make programs easier to maintain.

---

### 3. What is the difference between a parameter and an argument?

- **Parameter:** A variable declared in the function definition.
- **Argument:** The actual value passed when calling the function.

---

### 4. What is the purpose of the `return` statement?

The `return` statement sends a value back from a function and ends the function's execution.

---

### 5. What is the difference between `console.log()` and `return`?

- `console.log()` displays output in the console.
- `return` sends a value back so it can be stored or reused.

---

### 6. What is local scope?

A local variable can only be accessed inside the function where it is declared.

---

### 7. What is global scope?

A global variable is declared outside a function and can be accessed from anywhere in the program.

---

### 8. Can a function be called multiple times?

Yes. A function can be called as many times as needed.

---

### 9. What is a default parameter?

A default parameter provides a fallback value when no argument is passed.

---

### 10. Why should functions have meaningful names?

Meaningful names improve code readability and make the purpose of a function easier to understand.

---

<a id="whats-next"></a>

# 📚 What's Next?

In the next module, you'll start learning **ES6 (ECMAScript 2015)**, a major update to JavaScript that introduced many modern features.

Topics include:

- `let` and `const`
- Arrow Functions
- Template Literals
- Default Parameters (ES6 style)
- Spread Operator (`...`)
- Rest Parameters
- Destructuring
- Enhanced Object Literals

These features make JavaScript code cleaner, shorter, and easier to maintain.

---

<div align="center">

### ⭐ If these notes helped you, consider giving this repository a star!

**Happy Coding! 🚀**

</div>
