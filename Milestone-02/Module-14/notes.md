# 📘 Module 14: JavaScript Debugging & Error Handling

## 📖 Part 1 — Bug Basics & Error Understanding

> **Programming Hero | Milestone 03 | Module 14**

---

# 📑 Table of Contents

- [What is a Bug?](#what-is-a-bug)
- [Why Bugs Happen](#why-bugs-happen)
- [What is Debugging?](#what-is-debugging)
- [Syntax Error](#syntax-error)
- [Reference Error](#reference-error)
- [Type Error](#type-error)
- [Logical Error](#logical-error)
- [Reading Error Messages](#reading-error-messages)
- [Using console.log() for Debugging](#using-console-log-for-debugging)
- [Debugging Broken Conditionals](#debugging-broken-conditionals)
- [Finding Logic Mistakes](#finding-logic-mistakes)
- [Debugging Broken Loops](#debugging-broken-loops)
- [Infinite Loop Problems](#infinite-loop-problems)
- [Debugging Array Problems](#debugging-array-problems)
- [Index Errors](#index-errors)
- [Debugging Broken Functions](#debugging-broken-functions)
- [Parameter & Argument Issues](#parameter-argument-issues)
- [Return Value Problems](#return-value-problems)
- [VS Code Debugger](#vs-code-debugger)
- [Breakpoints](#breakpoints)
- [Step Over](#step-over)
- [Step Into](#step-into)
- [Step Out](#step-out)
- [Full Debugging Process](#full-debugging-process)
- [Best Practices](#best-practices)
- [Common Beginner Mistakes](#common-beginner-mistakes)
- [Practice Tasks](#practice-tasks)
- [Interview Questions](#interview-questions)
- [What's Next?](#whats-next)

---

<a id="what-is-a-bug"></a>

# What is a Bug?

A **bug** is an error or mistake in a program that causes unexpected behavior or incorrect results.

Simply:

> A bug is when your code does not work as expected.

Example:

```js
let age = 20;

if (age = 18) {
  console.log("Adult");
}
```

Expected:

```text
Adult only when age is 18
```

But the code has a mistake.

The problem:

```js
=
```

is an assignment operator, not a comparison operator.

Correct:

```js
if (age === 18) {
  console.log("Adult");
}
```

---

<a id="why-bugs-happen"></a>

# Why Bugs Happen

Bugs can happen for many reasons:

- Mistyping code
- Wrong logic
- Incorrect variable usage
- Wrong conditions
- Incorrect loop conditions
- Unexpected input
- Misunderstanding requirements
- Forgetting edge cases

Example:

```js
let total = price + tax;
```

If `price` or `tax` is not defined, the program will fail.

---

# Bugs Are Normal in Programming

Every developer writes code with bugs.

Professional developers are not people who never make mistakes.

They are people who can:

- Find bugs quickly
- Understand errors
- Debug systematically
- Improve their code

---

<a id="what-is-debugging"></a>

# What is Debugging?

**Debugging** is the process of finding, analyzing, and fixing bugs in code.

The general debugging process:

```
Problem occurs

↓

Read the error

↓

Find the cause

↓

Fix the code

↓

Test again
```

---

## Example Debugging Process

Problem:

```js
function add(a, b) {
  return a - b;
}

console.log(add(5, 3));
```

Output:

```text
2
```

Expected:

```text
8
```

---

Finding the issue:

The function is subtracting instead of adding.

Bug:

```js
return a - b;
```

Fix:

```js
return a + b;
```

---

<a id="syntax-error"></a>

# Syntax Error

A **Syntax Error** happens when JavaScript code does not follow the correct language rules.

The browser or JavaScript engine cannot understand the code.

Example:

```js
console.log("Hello"
```

Problem:

Missing closing bracket.

Correct:

```js
console.log("Hello");
```

---

Another Example:

❌

```js
function greet( {
  console.log("Hello");
}
```

The function syntax is incorrect.

---

### Common Causes

- Missing brackets `{}`
- Missing parentheses `()`
- Missing quotes
- Wrong keywords
- Typographical mistakes

---

<a id="reference-error"></a>

# Reference Error

A **Reference Error** occurs when you try to use a variable or function that does not exist.

Example:

```js
console.log(username);
```

Output:

```text
ReferenceError: username is not defined
```

Because `username` was never created.

---

Correct:

```js
let username = "Afia";

console.log(username);
```

Output:

```text
Afia
```

---

### Common Causes

- Misspelled variable names
- Using variables before declaring them
- Calling functions that do not exist

Example:

```js
console.log(userName);
```

But the variable is:

```js
let username = "Alex";
```

JavaScript treats them as different names.

---

<a id="type-error"></a>

# Type Error

A **Type Error** occurs when an operation is performed on an inappropriate data type.

Example:

```js
let number = 10;

number.toUpperCase();
```

Output:

```text
TypeError
```

Because numbers do not have a `toUpperCase()` method.

---

Another Example:

```js
let user = null;

console.log(user.name);
```

Output:

```text
TypeError
```

Because `null` does not contain properties.

---

### Common Causes

- Calling methods that do not exist
- Using incorrect data types
- Accessing properties from `null` or `undefined`

---

<a id="logical-error"></a>

# Logical Error

A **Logical Error** happens when the code runs without errors, but produces the wrong result.

This is one of the hardest bugs to find.

Example:

```js
function multiply(a, b) {

  return a + b;

}

console.log(multiply(5, 3));
```

Output:

```text
8
```

But expected:

```text
15
```

The code works, but the logic is wrong.

---

### Common Causes

- Wrong formula
- Wrong condition
- Incorrect algorithm
- Wrong operator

Example:

❌

```js
if (marks > 33)
```

Correct:

```js
if (marks >= 33)
```

---

<a id="reading-error-messages"></a>

# Reading Error Messages

Error messages are not just problems; they are clues.

Example:

```text
ReferenceError: age is not defined
```

Break it down:

```
ReferenceError
      |
      ↓
Type of problem


age is not defined
      |
      ↓
Problem location
```

---

## Common Error Format

```text
Error Type: Description

File Name

Line Number

Code Location
```

Example:

```text
TypeError: Cannot read properties of undefined
at script.js:10
```

Meaning:

- Error type → TypeError
- File → script.js
- Line → 10

---

<a id="using-console-log-for-debugging"></a>

# Using `console.log()` for Debugging

`console.log()` is one of the simplest debugging tools.

It helps us see:

- Variable values
- Function execution
- Data changes
- Program flow

---

## Example

Problem:

```js
function calculate(a, b) {

  let result = a * b;

  return result;
}

console.log(calculate(5, 10));
```

If output is wrong, check values:

```js
function calculate(a, b) {

  console.log(a);
  console.log(b);

  let result = a * b;

  console.log(result);

  return result;
}

calculate(5, 10);
```

Output:

```text
5
10
50
```

Now we can understand what is happening.

---

## Checking Program Flow

Example:

```js
console.log("Start");

let number = 10;

console.log(number);

console.log("End");
```

Output:

```text
Start
10
End
```

This helps understand which parts of code are running.

---

# 📝 Practice Problems

## Problem 1

Find the bug:

```js
let name = "JavaScript"

console.log(Name);
```

---

## Problem 2

Find the bug:

```js
let age = 20;

if(age = 18){
  console.log("Adult");
}
```

---

## Problem 3

Find the bug:

```js
let numbers = null;

console.log(numbers.length);
```

---

# 💡 Tips

- Read error messages carefully.
- Do not randomly change code; understand the problem first.
- Use `console.log()` to inspect values.
- Check line numbers mentioned in errors.
- Remember: every bug has a reason.

---

# ✅ Key Takeaways

- A bug is a mistake that causes unexpected behavior.
- Debugging means finding and fixing bugs.
- Syntax errors stop code execution.
- Reference errors happen when something does not exist.
- Type errors happen when operations are used incorrectly.
- Logical errors produce wrong results without showing errors.
- Error messages help identify problems.
- `console.log()` is a simple but powerful debugging tool.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 2 — Debugging Conditions, Loops & Arrays**




# 📘 Module 14: JavaScript Debugging & Error Handling

## 📖 Part 2 — Debugging Conditions, Loops & Arrays

> **Programming Hero | Milestone 03 | Module 14**

---

<a id="debugging-broken-conditionals"></a>

# Debugging Broken Conditionals

Conditional statements (`if`, `else if`, `else`) are used to make decisions.

A small mistake in a condition can completely change the program output.

---

## Example 1 — Wrong Comparison Operator

### ❌ Broken Code

```js
let age = 18;

if (age = 18) {
  console.log("Adult");
}
```

### Problem:

```js
=
```

is an assignment operator.

It changes the value instead of comparing.

---

### ✅ Fixed Code

```js
let age = 18;

if (age === 18) {
  console.log("Adult");
}
```

Output:

```text
Adult
```

---

<a id="finding-logic-mistakes"></a>

# Finding Logic Mistakes

Logical errors are difficult because the program runs but produces the wrong output.

Example:

### Problem:

A student passes if marks are 40 or above.

---

### ❌ Wrong Logic

```js
let marks = 40;

if (marks > 40) {
  console.log("Passed");
}
else {
  console.log("Failed");
}
```

Output:

```text
Failed
```

But 40 should pass.

---

### Why?

Condition:

```js
marks > 40
```

means:

```
Only numbers greater than 40
```

40 is excluded.

---

### ✅ Correct Logic

```js
if (marks >= 40) {
  console.log("Passed");
}
else {
  console.log("Failed");
}
```

---

# Debugging Conditional Steps

When debugging a condition:

### Step 1 — Check Input

```js
console.log(marks);
```

---

### Step 2 — Check Condition

Ask:

```
Is this condition logically correct?
```

---

### Step 3 — Test Different Values

Example:

```text
marks = 39
marks = 40
marks = 50
```

---

<a id="debugging-broken-loops"></a>

# Debugging Broken Loops

Loops are used to repeat tasks.

Common loop bugs:

- Wrong starting point
- Wrong ending condition
- Infinite loop
- Skipping values

---

## Example 1 — Wrong Loop Condition

### Goal:

Print numbers from 1 to 5.

---

### ❌ Broken Code

```js
for(let i = 1; i < 5; i++) {
  console.log(i);
}
```

Output:

```text
1
2
3
4
```

Problem:

The loop stops before 5.

---

### ✅ Fixed Code

```js
for(let i = 1; i <= 5; i++) {
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

<a id="infinite-loop-problems"></a>

# Infinite Loop Problems

An infinite loop happens when a loop never stops.

Example:

```js
let i = 1;

while(i <= 5) {
  console.log(i);
}
```

Output:

```text
1
1
1
1
...
```

---

## Problem:

The value of `i` never changes.

---

### Fixed Code:

```js
let i = 1;

while(i <= 5) {

  console.log(i);

  i++;

}
```

---

# Debugging Loop Process

When a loop does not work:

Check:

### 1. Starting Value

```js
let i = 0;
```

---

### 2. Condition

```js
i < array.length
```

---

### 3. Update Step

```js
i++
```

---

Example:

```js
for(let i = 0; i < 5; i++) {
  console.log(i);
}
```

Three important parts:

```
Start
 |
 ↓
let i = 0

Condition
 |
 ↓
i < 5

Update
 |
 ↓
i++
```

---

<a id="debugging-array-problems"></a>

# Debugging Array Problems

Arrays are common sources of bugs.

Common array problems:

- Wrong index
- Incorrect length
- Changing original data accidentally
- Accessing unavailable elements

---

## Example 1 — Wrong Index

### Code:

```js
let fruits = [
  "Apple",
  "Banana",
  "Mango"
];

console.log(fruits[3]);
```

Output:

```text
undefined
```

---

## Why?

Array indexes start from `0`.

```
Apple  → 0
Banana → 1
Mango  → 2
```

Index `3` does not exist.

---

### Fixed:

```js
console.log(fruits[2]);
```

Output:

```text
Mango
```

---

<a id="index-errors"></a>

# Index Errors

A common mistake is using the wrong array boundary.

Example:

### ❌ Wrong

```js
let numbers = [10,20,30];

for(let i = 0; i <= numbers.length; i++) {

  console.log(numbers[i]);

}
```

Output:

```text
10
20
30
undefined
```

---

Problem:

Array length is:

```text
3
```

But indexes are:

```text
0, 1, 2
```

---

### ✅ Correct

```js
for(let i = 0; i < numbers.length; i++) {

  console.log(numbers[i]);

}
```

---

# Debugging Array with Console

Example:

```js
let numbers = [5,10,15];

console.log(numbers);

for(let number of numbers) {

  console.log(number);

}
```

Output:

```text
[5,10,15]
5
10
15
```

This helps verify:

- Array values
- Loop execution
- Data changes

---

# Full Debugging Example

## Problem:

Find the sum of array values.

### ❌ Broken Code

```js
function sum(numbers) {

  let total = 0;

  for(let i = 0; i <= numbers.length; i++) {

    total += numbers[i];

  }

  return total;
}

console.log(sum([10,20,30]));
```

Output:

```text
NaN
```

---

## Debugging

Add:

```js
console.log(numbers[i]);
```

Output:

```text
10
20
30
undefined
```

Problem found:

Loop runs one extra time.

---

## ✅ Fixed Code

```js
function sum(numbers) {

  let total = 0;

  for(let i = 0; i < numbers.length; i++) {

    total += numbers[i];

  }

  return total;
}

console.log(sum([10,20,30]));
```

Output:

```text
60
```

---

# 📝 Practice Problems

## Problem 1

Fix the condition:

```js
let score = 50;

if(score = 50){
  console.log("Correct");
}
```

---

## Problem 2

Fix the loop:

```js
for(let i = 1; i < 10; i--){
  console.log(i);
}
```

---

## Problem 3

Find the array bug:

```js
let colors = ["red", "blue"];

console.log(colors[2]);
```

---

# 💡 Tips

- Check conditions carefully.
- Test boundary values.
- Use `console.log()` to inspect variables.
- For loops, always check:
  - Start value
  - Condition
  - Update
- Remember array indexes start from `0`.

---

# ✅ Key Takeaways

- Conditional bugs usually come from incorrect operators or logic.
- Loop bugs often happen because of wrong conditions or updates.
- Infinite loops occur when the stopping condition is never reached.
- Array bugs commonly happen because of incorrect indexes.
- Debugging requires checking values, logic, and program flow step-by-step.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 3 — Debugging Functions & VS Code Debugger**




# 📘 Module 14: JavaScript Debugging & Error Handling

## 📖 Part 3 — Debugging Functions & VS Code Debugger

> **Programming Hero | Milestone 03 | Module 14**

---

<a id="debugging-broken-functions"></a>

# Debugging Broken Functions

Functions are one of the most common places where bugs appear.

Common function-related bugs:

- Wrong parameters
- Missing arguments
- Incorrect return values
- Wrong logic inside function
- Function not being called

---

## Example 1 — Wrong Return Value

### ❌ Broken Code

```js
function multiply(a, b) {

  return a + b;

}

console.log(multiply(5, 3));
```

Output:

```text
8
```

Expected:

```text
15
```

---

## Finding the Bug

Check the function logic:

```js
return a + b;
```

The function name says `multiply`, but it is adding values.

---

### ✅ Fixed Code

```js
function multiply(a, b) {

  return a * b;

}

console.log(multiply(5, 3));
```

Output:

```text
15
```

---

<a id="parameter-argument-issues"></a>

# Parameter & Argument Issues

Parameters are variables inside function definitions.

Arguments are values passed when calling a function.

---

## Example

```js
function greet(name) {

  console.log("Hello " + name);

}

greet("Afia");
```

Here:

```text
name → Parameter

"Afia" → Argument
```

---

## Missing Argument Bug

### Code:

```js
function greet(name) {

  console.log("Hello " + name);

}

greet();
```

Output:

```text
Hello undefined
```

---

## Fix:

Provide the required argument.

```js
greet("Afia");
```

---

# Debugging Function Execution

When a function does not work:

Check:

### 1. Is the function being called?

Example:

```js
function sayHello(){

 console.log("Hello");

}
```

The function exists but never runs.

Need:

```js
sayHello();
```

---

### 2. Are parameters receiving correct values?

Use:

```js
console.log(parameter);
```

Example:

```js
function add(a, b){

 console.log(a);
 console.log(b);

 return a + b;

}

add(5,10);
```

Output:

```text
5
10
```

---

### 3. Is the function returning the correct value?

Example:

```js
function square(number){

 return number * number;

}

console.log(square(5));
```

Output:

```text
25
```

---

<a id="return-value-problems"></a>

# Return Value Problems

A common beginner mistake is confusing:

- `console.log()`
- `return`

---

## ❌ Wrong Example

```js
function add(a, b){

 console.log(a + b);

}

let result = add(5,10);

console.log(result);
```

Output:

```text
15
undefined
```

---

## Why?

`console.log()` only displays the value.

It does not send the value back.

---

## ✅ Correct Example

```js
function add(a, b){

 return a + b;

}

let result = add(5,10);

console.log(result);
```

Output:

```text
15
```

---

# Debugging Function Step-by-Step

Example:

```js
function calculatePrice(price, quantity){

 let total = price * quantity;

 return total;

}

console.log(calculatePrice(100,5));
```

If output is wrong:

---

## Step 1 — Check Inputs

```js
console.log(price);
console.log(quantity);
```

---

## Step 2 — Check Calculation

```js
console.log(total);
```

---

## Step 3 — Check Return

```js
return total;
```

---

<a id="vs-code-debugger"></a>

# VS Code Debugger

`console.log()` is useful, but professional developers often use debugging tools.

VS Code has a built-in debugger that allows us to:

- Pause code execution
- Check variable values
- Run code step-by-step
- Understand program flow

---

# Starting Debugger in VS Code

Steps:

1. Open your JavaScript file in VS Code.
2. Click beside a line number to create a breakpoint.
3. Run the debugger.
4. The program will pause at that line.

---

<a id="breakpoints"></a>

# Breakpoints

A breakpoint tells the debugger:

> Stop the program here so I can inspect what is happening.

Example:

```js
let price = 100;

let quantity = 5;

let total = price * quantity;

console.log(total);
```

You can place a breakpoint on:

```js
let total = price * quantity;
```

The program will pause before executing that line.

---

# Inspecting Variables

When the debugger pauses, you can see:

```text
price = 100

quantity = 5

total = undefined
```

After execution:

```text
total = 500
```

This helps find where values become incorrect.

---

<a id="step-over"></a>

# Step Over

Step Over executes the current line and moves to the next line.

Example:

```js
let a = 10;

let b = 20;

let sum = a + b;
```

Using Step Over:

```
Line 1 executes

↓

Line 2 executes

↓

Line 3 executes
```

---

<a id="step-into"></a>

# Step Into

Step Into moves inside a function to see how it works.

Example:

```js
function add(a,b){

 return a+b;

}

add(5,10);
```

Step Into enters:

```js
function add()
```

and shows the internal execution.

---

<a id="step-out"></a>

# Step Out

Step Out finishes the current function and returns to the previous location.

Example:

You entered:

```js
add()
```

After checking the function:

Step Out returns back to:

```js
add(5,10);
```

---

<a id="full-debugging-process"></a>

# Applying the Full Debugging Process

A complete debugging workflow:

---

## Step 1 — Reproduce the Problem

Make sure the bug happens consistently.

---

## Step 2 — Read the Error

Understand:

- Error type
- Message
- File location
- Line number

---

## Step 3 — Check Values

Use:

```js
console.log()
```

or debugger.

---

## Step 4 — Find the Root Cause

Do not only fix the symptom.

Find why it happened.

---

## Step 5 — Fix and Test

After fixing:

- Test old cases
- Test new cases
- Check edge cases

---

# Example Full Debugging

Problem:

```js
function discount(price){

 return price - 10%;

}

console.log(discount(100));
```

---

## Finding Issue:

The calculation is incorrect.

Correct formula:

```text
price - (price * discount percentage)
```

---

## Fixed:

```js
function discount(price){

 return price - (price * 0.10);

}

console.log(discount(100));
```

Output:

```text
90
```

---

# 📝 Practice Problems

## Problem 1

Find the bug:

```js
function divide(a,b){

 return a*b;

}
```

Expected:

Division result.

---

## Problem 2

Fix:

```js
function greet(name){

 console.log("Hello");

}

greet("Alex");
```

---

## Problem 3

Debug:

```js
function calculate(a,b){

 let result = a+b;

 console.log(result);

}

let output = calculate(5,5);

console.log(output);
```

---

# 💡 Tips

- Debugging is a process, not random guessing.
- Understand the error before fixing it.
- Use breakpoints for complex problems.
- Check data flow inside functions.
- Always test after fixing bugs.

---

# ✅ Key Takeaways

- Functions can fail because of wrong parameters, logic, or return values.
- `console.log()` helps inspect values during execution.
- VS Code debugger allows step-by-step code analysis.
- Breakpoints pause program execution.
- Step Over, Step Into, and Step Out help understand code flow.
- A professional debugging process finds the root cause instead of temporary fixes.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 4 — Module Summary**




# 📘 Module 14: JavaScript Debugging & Error Handling

## 🎯 Part 4 — Module Summary

> **Programming Hero | Milestone 03 | Module 14**

---

# 📖 Module Summary

Congratulations! 🎉

You have completed **Module 14 – JavaScript Debugging & Error Handling**.

Debugging is one of the most important skills for every developer. Writing code is only one part of programming; finding and fixing problems efficiently is equally important.

In this module, you learned:

- What is a Bug
- Why Bugs Happen
- What is Debugging
- Different Types of Errors:
  - Syntax Error
  - Reference Error
  - Type Error
  - Logical Error
- Reading Error Messages
- Using `console.log()` for Debugging
- Debugging Conditional Problems
- Debugging Loop Problems
- Debugging Array Problems
- Debugging Function Problems
- Parameter & Argument Issues
- Return Value Problems
- VS Code Debugger
- Breakpoints
- Step Over
- Step Into
- Step Out
- Complete Debugging Process

These debugging skills will be useful throughout your developer journey because real-world projects always contain bugs.

---

<a id="best-practices"></a>

# 💡 Best Practices

- ✅ Read the error message carefully before changing code.
- ✅ Understand the root cause instead of fixing only the output.
- ✅ Use meaningful variable names to make debugging easier.
- ✅ Use `console.log()` strategically.
- ✅ Test code with different inputs.
- ✅ Check edge cases.
- ✅ Use debugger tools for complex problems.
- ✅ Reproduce the bug before trying to fix it.
- ✅ Remove unnecessary debugging code before finalizing projects.

---

<a id="common-beginner-mistakes"></a>

# 🚫 Common Beginner Mistakes

## 1. Ignoring Error Messages

Many beginners see an error and immediately rewrite code.

Better approach:

```
Read error
↓
Understand problem
↓
Find cause
↓
Fix
```

---

## 2. Randomly Changing Code

Changing multiple lines without understanding makes debugging harder.

Example:

❌

```text
Change code
Run
Change another code
Run
Repeat
```

Better:

```
Identify one possible cause
Test it
Confirm result
```

---

## 3. Using Too Many Console Logs

`console.log()` is useful, but too many logs make code confusing.

❌

```js
console.log(a);
console.log(b);
console.log(c);
console.log(d);
console.log(e);
```

Use logs only where necessary.

---

## 4. Not Testing Edge Cases

A program may work for normal inputs but fail for unusual cases.

Example:

```js
function divide(a,b){
 return a/b;
}
```

What happens when:

```js
divide(10,0)
```

Always think about possible edge cases.

---

## 5. Fixing Symptoms Instead of Causes

Example:

Problem:

```text
Output is wrong
```

Bad approach:

Changing random values until output looks correct.

Good approach:

Find why the logic is producing the wrong result.

---

<a id="practice-tasks"></a>

# 🎯 Practice Tasks

## Task 1 — Fix Syntax Errors

Find and fix errors:

```js
console.log("Hello World"
```

---

## Task 2 — Fix Reference Errors

Debug:

```js
let username = "Alex";

console.log(userName);
```

---

## Task 3 — Fix Conditional Bugs

Debug:

```js
let temperature = 30;

if(temperature = 30){

 console.log("Hot");

}
```

---

## Task 4 — Fix Loop Bugs

Debug:

```js
for(let i = 0; i <= 5; i++){

 console.log(i);

}
```

Check if the output is expected.

---

## Task 5 — Fix Array Bug

Debug:

```js
let numbers = [10,20,30];

console.log(numbers[5]);
```

---

## Task 6 — Fix Function Bug

Debug:

```js
function square(number){

 console.log(number * number);

}

let result = square(5);

console.log(result);
```

---

## Task 7 — Use VS Code Debugger

Create a small program:

```js
function calculateTotal(price, quantity){

 let total = price * quantity;

 return total;

}

console.log(calculateTotal(100,5));
```

Practice:

- Add breakpoint
- Inspect variables
- Use Step Over
- Check execution flow

---

<a id="interview-questions"></a>

# ❓ Interview Questions

### 1. What is a bug?

A bug is an error or mistake in a program that causes unexpected behavior.

---

### 2. What is debugging?

Debugging is the process of finding, analyzing, and fixing bugs in code.

---

### 3. What are the common types of errors in JavaScript?

Common errors:

- Syntax Error
- Reference Error
- Type Error
- Logical Error

---

### 4. What is the difference between Syntax Error and Logical Error?

**Syntax Error:**

The code structure is invalid, so the program cannot run.

**Logical Error:**

The code runs, but produces incorrect results.

---

### 5. What is a Reference Error?

A Reference Error happens when JavaScript cannot find a variable or function that is being used.

---

### 6. Why is `console.log()` useful for debugging?

It helps inspect values, understand program flow, and find where problems occur.

---

### 7. What is a breakpoint?

A breakpoint pauses program execution at a specific line so developers can inspect the code.

---

### 8. Difference between Step Over and Step Into?

**Step Over:**

Executes the current line and moves forward.

**Step Into:**

Moves inside a function to see its internal execution.

---

### 9. Why should developers learn debugging?

Because real-world applications contain bugs, and developers need to identify and fix them efficiently.

---

### 10. What is the debugging process?

A common process:

1. Reproduce the problem
2. Read the error
3. Find the cause
4. Fix the issue
5. Test again

---

<a id="whats-next"></a>

# 📚 What's Next?

In the upcoming modules, you will start learning more modern JavaScript concepts.

You will explore:

- Modern JavaScript syntax
- ES6 features
- Cleaner ways to write JavaScript
- More advanced programming techniques

These concepts will help you write shorter, cleaner, and more professional JavaScript code.

---

<div align="center">

### ⭐ If these notes helped you, consider giving this repository a star!

**Happy Coding! 🚀**

</div>
