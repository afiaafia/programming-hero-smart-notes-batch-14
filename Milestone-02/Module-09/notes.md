# 📘 Module 09: JavaScript Loops

## 🔄 Part 1 — Loop Fundamentals

> **Programming Hero | Milestone 02 | Module 09**

---

# 📑 Table of Contents

- [What is a Loop?](#what-is-a-loop)
- [Why Do We Need Loops?](#why-do-we-need-loops)
- [Types of Loops](#types-of-loops)
- [The `for` Loop](#for-loop)
- [Loop Flow](#loop-flow)
- [Printing Numbers](#printing-numbers)
- [Basic Examples](#basic-examples)
- [The `while` Loop](#while-loop)
- [The `do...while` Loop](#do-while-loop)
- [The `break` Statement](#break-statement)
- [The `continue` Statement](#continue-statement)
- [Infinite Loop](#infinite-loop)
- [The `for` Loop vs `while` Loop](#for-vs-while)
- [Real-World Examples](#real-world-examples)
- [Nested Loops](#nested-loops)
- [Pattern Printing](#pattern-printing)
- [Sum of Numbers](#sum-of-numbers)
- [Even & Odd Numbers](#even-and-odd-numbers)
- [Multiplication Table](#multiplication-table)
- [Countdown Timer](#countdown-timer)
- [Loop Practice Problems](#loop-practice-problems)
- [Best Practices](#best-practices)
- [Common Beginner Mistakes](#common-beginner-mistakes)
- [Practice Tasks](#practice-tasks)
- [Interview Questions](#interview-questions)
- [What's Next?](#whats-next)

---

<a id="what-is-a-loop"></a>

# What is a Loop?

A **loop** is a programming structure that allows a block of code to execute **repeatedly** until a specified condition becomes false.

Instead of writing the same code multiple times, we can use a loop to automate repetitive tasks.

### Without a Loop

```js
console.log(1);
console.log(2);
console.log(3);
console.log(4);
console.log(5);
```

### With a Loop

```js
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

Both programs produce the same output, but the loop version is shorter, cleaner, and easier to maintain.

---

<a id="why-do-we-need-loops"></a>

# Why Do We Need Loops?

Loops help us avoid writing repetitive code.

Imagine printing numbers from **1 to 1000**.

Without loops, you would need to write:

```js
console.log(1);
console.log(2);
console.log(3);
...
console.log(1000);
```

Using a loop:

```js
for (let i = 1; i <= 1000; i++) {
  console.log(i);
}
```

### Common Uses of Loops

- Printing numbers
- Processing arrays
- Reading user data
- Generating patterns
- Running calculations
- Repeating tasks

---

<a id="types-of-loops"></a>

# Types of Loops

JavaScript provides several types of loops.

| Loop | Purpose |
|------|---------|
| `for` | Repeat a known number of times |
| `while` | Repeat while a condition is true |
| `do...while` | Execute at least once before checking the condition |
| `for...of` | Iterate over iterable objects (Arrays, Strings, etc.) |
| `for...in` | Iterate over object properties |

> ✅ In this module, we'll focus mainly on `for`, `while`, and `do...while`.

---

<a id="for-loop"></a>

# The `for` Loop

The **`for` loop** is the most commonly used loop in JavaScript.

It is ideal when you already know how many times the loop should execute.

### Syntax

```js
for (initialization; condition; update) {
  // code to execute
}
```

Example:

```js
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

Output:

```text
1
2
3
4
5
```

---

# Understanding the Three Parts

A `for` loop has three parts.

```js
for (let i = 1; i <= 5; i++) {

}
```

### 1. Initialization

```js
let i = 1;
```

Creates the loop variable.

Runs **only once**.

---

### 2. Condition

```js
i <= 5
```

The loop continues while this condition is `true`.

When it becomes `false`, the loop stops.

---

### 3. Update

```js
i++
```

Updates the loop variable after each iteration.

---

<a id="loop-flow"></a>

# Loop Flow

The execution order of a `for` loop is:

```text
Initialization
      ↓
Check Condition
      ↓
True?
 ┌────┴────┐
 │         │
Yes       No
 │         │
 ↓         ↓
Run Code   Stop
 │
 ↓
Update
 │
 └──────────────→ Check Condition Again
```

Understanding this flow makes debugging loops much easier.

---

<a id="printing-numbers"></a>

# Printing Numbers

## Print 1 to 5

```js
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

Output:

```text
1
2
3
4
5
```

---

## Print 5 to 1

```js
for (let i = 5; i >= 1; i--) {
  console.log(i);
}
```

Output:

```text
5
4
3
2
1
```

---

## Print 1 to 10

```js
for (let i = 1; i <= 10; i++) {
  console.log(i);
}
```

---

## Print Even Numbers

```js
for (let i = 2; i <= 10; i += 2) {
  console.log(i);
}
```

Output:

```text
2
4
6
8
10
```

---

## Print Odd Numbers

```js
for (let i = 1; i <= 10; i += 2) {
  console.log(i);
}
```

Output:

```text
1
3
5
7
9
```

---

<a id="basic-examples"></a>

# Basic Examples

## Example 1 — Print Hello

```js
for (let i = 1; i <= 5; i++) {
  console.log("Hello");
}
```

Output:

```text
Hello
Hello
Hello
Hello
Hello
```

---

## Example 2 — Print Squares

```js
for (let i = 1; i <= 5; i++) {
  console.log(i * i);
}
```

Output:

```text
1
4
9
16
25
```

---

## Example 3 — Print Multiples of 5

```js
for (let i = 5; i <= 25; i += 5) {
  console.log(i);
}
```

Output:

```text
5
10
15
20
25
```

---

## Example 4 — Countdown

```js
for (let i = 10; i >= 1; i--) {
  console.log(i);
}
```

Output:

```text
10
9
8
7
6
5
4
3
2
1
```

---

# 💡 Tips

- Choose meaningful variable names when possible.
- Keep loop conditions simple and easy to understand.
- Avoid changing the loop variable inside the loop body unless necessary.
- Make sure the update statement eventually makes the condition false.

---

# ✅ Key Takeaways

- A loop executes the same block of code repeatedly.
- Loops reduce repetitive code.
- The `for` loop is ideal when the number of iterations is known.
- Every `for` loop has three parts:
  - Initialization
  - Condition
  - Update
- The loop stops when its condition becomes `false`.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 2 — `while` Loop & Loop Control**




# 📘 Module 09: JavaScript Loops

## 🔁 Part 2 — `while` Loop & Loop Control

> **Programming Hero | Milestone 02 | Module 09**

---

<a id="while-loop"></a>

# The `while` Loop

A **`while` loop** repeatedly executes a block of code **as long as the condition remains `true`**.

Unlike the `for` loop, a `while` loop is commonly used when **the number of iterations is unknown**.

### Syntax

```js
while (condition) {
  // code
}
```

Example:

```js
let i = 1;

while (i <= 5) {
  console.log(i);
  i++;
}
```

Output:

```text
1
2
3
4
5
```

---

# How `while` Loop Works

Execution Flow:

```text
Initialization
      ↓
Check Condition
      ↓
True?
 ┌────┴────┐
 │         │
Yes       No
 │         │
 ↓         ↓
Run Code   Stop
 │
 ↓
Update Variable
 │
 └────────────→ Check Condition Again
```

Unlike a `for` loop, the **initialization** and **update** are written separately.

---

# `for` vs `while`

| `for` Loop | `while` Loop |
|------------|--------------|
| Best when the number of iterations is known | Best when the number of iterations is unknown |
| Initialization, condition, and update are written together | Initialization and update are written separately |
| More compact | More flexible |

### `for` Example

```js
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

### `while` Example

```js
let i = 1;

while (i <= 5) {
  console.log(i);
  i++;
}
```

Both produce the same output.

---

<a id="do-while-loop"></a>

# The `do...while` Loop

The **`do...while` loop** executes the code **at least once**, even if the condition is `false`.

### Syntax

```js
do {
  // code
} while (condition);
```

Example:

```js
let i = 1;

do {
  console.log(i);
  i++;
} while (i <= 5);
```

Output:

```text
1
2
3
4
5
```

---

# Difference Between `while` and `do...while`

### `while`

Checks the condition **before** executing the code.

```js
let i = 6;

while (i <= 5) {
  console.log(i);
}
```

Output:

```text
(No output)
```

---

### `do...while`

Executes the code first, then checks the condition.

```js
let i = 6;

do {
  console.log(i);
} while (i <= 5);
```

Output:

```text
6
```

---

<a id="break-statement"></a>

# The `break` Statement

The `break` statement immediately terminates a loop.

Example:

```js
for (let i = 1; i <= 10; i++) {

  if (i === 6) {
    break;
  }

  console.log(i);
}
```

Output:

```text
1
2
3
4
5
```

The loop stops as soon as `i` becomes `6`.

---

# When to Use `break`

Common use cases:

- Searching for an item
- Stopping after finding a match
- Exiting an infinite loop
- Ending a loop early

Example:

```js
let passwordFound = true;

while (true) {

  if (passwordFound) {
    break;
  }

}
```

---

<a id="continue-statement"></a>

# The `continue` Statement

The `continue` statement skips the current iteration and moves to the next one.

Example:

```js
for (let i = 1; i <= 5; i++) {

  if (i === 3) {
    continue;
  }

  console.log(i);
}
```

Output:

```text
1
2
4
5
```

The value `3` is skipped.

---

# `break` vs `continue`

| `break` | `continue` |
|----------|------------|
| Stops the entire loop | Skips only the current iteration |
| Loop ends immediately | Loop continues with the next iteration |

Example:

### Using `break`

```js
for (let i = 1; i <= 5; i++) {

  if (i === 3) {
    break;
  }

  console.log(i);
}
```

Output:

```text
1
2
```

---

### Using `continue`

```js
for (let i = 1; i <= 5; i++) {

  if (i === 3) {
    continue;
  }

  console.log(i);
}
```

Output:

```text
1
2
4
5
```

---

<a id="infinite-loop"></a>

# Infinite Loop

An **Infinite Loop** is a loop that never ends because its condition never becomes `false`.

Example:

```js
let i = 1;

while (i <= 5) {
  console.log(i);
}
```

❌ Problem:

```js
i++;
```

is missing.

The condition always remains `true`.

---

### Correct Version

```js
let i = 1;

while (i <= 5) {
  console.log(i);
  i++;
}
```

---

# How to Avoid Infinite Loops

- Always update the loop variable.
- Ensure the condition can eventually become `false`.
- Test loops with small values first.
- Use `break` when necessary.

---

<a id="real-world-examples"></a>

# Real-World Examples

## Example 1 — Print Even Numbers

```js
let i = 2;

while (i <= 10) {
  console.log(i);
  i += 2;
}
```

---

## Example 2 — Countdown

```js
let i = 5;

while (i >= 1) {
  console.log(i);
  i--;
}
```

---

## Example 3 — Skip Even Numbers

```js
for (let i = 1; i <= 10; i++) {

  if (i % 2 === 0) {
    continue;
  }

  console.log(i);
}
```

Output:

```text
1
3
5
7
9
```

---

## Example 4 — Stop at First Multiple of 7

```js
for (let i = 1; i <= 20; i++) {

  if (i % 7 === 0) {
    console.log(i);
    break;
  }

}
```

Output:

```text
7
```

---

# 💡 Tips

- Use `for` when the number of iterations is known.
- Use `while` when the stopping condition depends on runtime.
- Remember that `do...while` always executes at least once.
- Use `break` to exit a loop early.
- Use `continue` to skip only the current iteration.
- Always verify that your loop can terminate.

---

# ✅ Key Takeaways

- `while` repeats as long as its condition is `true`.
- `do...while` executes at least once.
- `break` exits the loop immediately.
- `continue` skips the current iteration.
- Infinite loops occur when the condition never becomes `false`.
- Choose the appropriate loop based on the problem.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 3 — Nested Loops & Problem Solving**




# 📘 Module 09: JavaScript Loops

## 🔄 Part 3 — Nested Loops & Problem Solving

> **Programming Hero | Milestone 02 | Module 09**

---

<a id="nested-loops"></a>

# Nested Loops

A **Nested Loop** is a loop inside another loop.

The outer loop executes first. For every iteration of the outer loop, the inner loop runs completely.

### Syntax

```js
for (let i = 1; i <= 3; i++) {

  for (let j = 1; j <= 3; j++) {
    console.log(i, j);
  }

}
```

Output:

```text
1 1
1 2
1 3
2 1
2 2
2 3
3 1
3 2
3 3
```

---

# How Nested Loops Work

Execution Flow:

```text
Outer Loop (i = 1)
    ↓
Inner Loop
1 1
1 2
1 3

Outer Loop (i = 2)
    ↓
Inner Loop
2 1
2 2
2 3

Outer Loop (i = 3)
    ↓
Inner Loop
3 1
3 2
3 3
```

The inner loop completes all of its iterations before the outer loop moves to the next iteration.

---

<a id="pattern-printing"></a>

# Pattern Printing

Nested loops are commonly used to print patterns.

## Example 1 — Square Pattern

```js
for (let i = 1; i <= 3; i++) {

  let row = "";

  for (let j = 1; j <= 3; j++) {
    row += "* ";
  }

  console.log(row);
}
```

Output:

```text
* * *
* * *
* * *
```

---

## Example 2 — Number Pattern

```js
for (let i = 1; i <= 5; i++) {

  let row = "";

  for (let j = 1; j <= i; j++) {
    row += j + " ";
  }

  console.log(row);
}
```

Output:

```text
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

---

## Example 3 — Star Triangle

```js
for (let i = 1; i <= 5; i++) {

  let row = "";

  for (let j = 1; j <= i; j++) {
    row += "*";
  }

  console.log(row);
}
```

Output:

```text
*
**
***
****
*****
```

---

<a id="sum-of-numbers"></a>

# Sum of Numbers

Loops are often used to calculate totals.

Example:

```js
let sum = 0;

for (let i = 1; i <= 5; i++) {
  sum += i;
}

console.log(sum);
```

Output:

```text
15
```

---

## Sum of Even Numbers

```js
let sum = 0;

for (let i = 2; i <= 10; i += 2) {
  sum += i;
}

console.log(sum);
```

Output:

```text
30
```

---

<a id="even-and-odd-numbers"></a>

# Even & Odd Numbers

## Print Even Numbers

```js
for (let i = 1; i <= 10; i++) {

  if (i % 2 === 0) {
    console.log(i);
  }

}
```

Output:

```text
2
4
6
8
10
```

---

## Print Odd Numbers

```js
for (let i = 1; i <= 10; i++) {

  if (i % 2 !== 0) {
    console.log(i);
  }

}
```

Output:

```text
1
3
5
7
9
```

---

<a id="multiplication-table"></a>

# Multiplication Table

Example:

```js
let number = 5;

for (let i = 1; i <= 10; i++) {
  console.log(`${number} × ${i} = ${number * i}`);
}
```

Output:

```text
5 × 1 = 5
5 × 2 = 10
5 × 3 = 15
...
5 × 10 = 50
```

---

<a id="countdown-timer"></a>

# Countdown Timer

Example:

```js
for (let i = 10; i >= 1; i--) {
  console.log(i);
}

console.log("🚀 Liftoff!");
```

Output:

```text
10
9
8
...
1
🚀 Liftoff!
```

---

<a id="loop-practice-problems"></a>

# Loop Practice Problems

## Problem 1 — Print Numbers from 1 to 50

```js
for (let i = 1; i <= 50; i++) {
  console.log(i);
}
```

---

## Problem 2 — Print Multiples of 3

```js
for (let i = 3; i <= 30; i += 3) {
  console.log(i);
}
```

---

## Problem 3 — Count Even Numbers

```js
let count = 0;

for (let i = 1; i <= 20; i++) {

  if (i % 2 === 0) {
    count++;
  }

}

console.log(count);
```

Output:

```text
10
```

---

## Problem 4 — Find the Largest Number

```js
let numbers = [15, 22, 9, 48, 31];

let largest = numbers[0];

for (let i = 1; i < numbers.length; i++) {

  if (numbers[i] > largest) {
    largest = numbers[i];
  }

}

console.log(largest);
```

Output:

```text
48
```

> 💡 **Note:** Arrays will be covered in detail in a later module. For now, focus on understanding how the loop compares each value.

---

# 💡 Tips

- Nested loops are useful for patterns, tables, and grids.
- Use a separate variable (like `sum` or `count`) to store calculated results.
- Keep nested loops as simple as possible to improve readability.
- Be careful with nested loops on large datasets, as they can increase execution time.

---

# ✅ Key Takeaways

- A nested loop is a loop inside another loop.
- The inner loop finishes all iterations before the outer loop continues.
- Loops can calculate sums, counts, and other values.
- Nested loops are commonly used for pattern printing.
- Loops are essential for solving real-world programming problems efficiently.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 4 — Module Summary**





# 📘 Module 09: JavaScript Loops

## 🎯 Part 4 — Module Summary

> **Programming Hero | Milestone 02 | Module 09**

---

# 📖 Module Summary

Congratulations! 🎉

You have completed **Module 09 – JavaScript Loops**.

In this module, you learned how to execute the same block of code repeatedly using different types of loops. Loops are one of the most fundamental concepts in programming and are used extensively in real-world applications.

You learned:

- What a loop is
- Why loops are important
- Types of loops in JavaScript
- `for` loop
- `while` loop
- `do...while` loop
- `break`
- `continue`
- Infinite loops
- Nested loops
- Pattern printing
- Loop-based problem solving

These concepts will be used frequently when working with Arrays, Objects, Functions, DOM, and Algorithms.

---

<a id="best-practices"></a>

# 💡 Best Practices

- ✅ Choose the right loop for the problem.
- ✅ Use meaningful variable names (`i`, `j`, `count`, `sum`, etc.).
- ✅ Keep loop conditions simple and readable.
- ✅ Always ensure the loop condition can eventually become `false`.
- ✅ Avoid unnecessary nested loops.
- ✅ Use `break` only when an early exit is required.
- ✅ Use `continue` only when skipping the current iteration improves readability.
- ✅ Test loops with small data before using large datasets.

---

<a id="common-beginner-mistakes"></a>

# 🚫 Common Beginner Mistakes

## 1. Forgetting to Update the Loop Variable

❌ Wrong

```js
let i = 1;

while (i <= 5) {
  console.log(i);
}
```

This creates an infinite loop.

✅ Correct

```js
let i = 1;

while (i <= 5) {
  console.log(i);
  i++;
}
```

---

## 2. Incorrect Loop Condition

❌

```js
for (let i = 1; i >= 10; i++) {
  console.log(i);
}
```

The condition is false from the beginning, so the loop never runs.

---

## 3. Off-by-One Error

❌

```js
for (let i = 1; i < 10; i++) {
  console.log(i);
}
```

Prints:

```text
1–9
```

✅

```js
for (let i = 1; i <= 10; i++) {
  console.log(i);
}
```

Prints:

```text
1–10
```

---

## 4. Modifying the Loop Variable Unexpectedly

❌

```js
for (let i = 1; i <= 10; i++) {

  i += 3;

}
```

Changing the loop variable inside the loop can make the behavior difficult to understand.

---

## 5. Deeply Nested Loops

Too many nested loops reduce readability and may affect performance.

Whenever possible, simplify the logic.

---

<a id="practice-tasks"></a>

# 🎯 Practice Tasks

## Task 1

Print numbers from **1 to 20** using a `for` loop.

---

## Task 2

Print all even numbers from **1 to 50**.

---

## Task 3

Print all odd numbers from **1 to 50**.

---

## Task 4

Calculate the sum of numbers from **1 to 100**.

Expected Output:

```text
5050
```

---

## Task 5

Print the multiplication table of **7**.

Example:

```text
7 × 1 = 7
...
7 × 10 = 70
```

---

## Task 6

Print this pattern:

```text
*
**
***
****
*****
```

---

## Task 7

Count how many numbers between **1 and 100** are divisible by **5**.

---

## Task 8

Using a loop, find the largest number in this array:

```js
[10, 35, 8, 99, 42]
```

---

<a id="interview-questions"></a>

# ❓ Interview Questions

### 1. What is a loop?

A loop is a programming structure that repeatedly executes a block of code until a specified condition becomes false.

---

### 2. What is the difference between `for` and `while`?

- `for` is best when the number of iterations is known.
- `while` is best when the number of iterations is unknown.

---

### 3. What is a `do...while` loop?

A `do...while` loop executes the code block **at least once**, then checks the condition.

---

### 4. What is an infinite loop?

An infinite loop is a loop whose condition never becomes `false`, causing it to run forever.

---

### 5. What does `break` do?

`break` immediately terminates the current loop.

---

### 6. What does `continue` do?

`continue` skips the current iteration and moves to the next one.

---

### 7. What is a nested loop?

A nested loop is a loop inside another loop.

---

### 8. Where are loops commonly used?

Loops are commonly used for:

- Processing arrays
- Reading data
- Searching
- Calculations
- Pattern printing
- Repetitive tasks

---

<a id="whats-next"></a>

# 📚 What's Next?

In the next module, you'll learn one of the most important JavaScript data structures:

- Arrays
- Creating Arrays
- Accessing Elements
- Updating Elements
- Array Methods
- Looping Through Arrays
- Real-World Array Problems

Arrays and loops work together in almost every JavaScript application, so the next module builds directly on what you've learned here.

---

<div align="center">

### ⭐ If these notes helped you, consider giving this repository a star!

**Happy Coding! 🚀**

</div>
