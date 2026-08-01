# 📘 Module 08: JavaScript Conditionals & Decision Making

---

# 📑 Table of Contents

- [Boolean Recap](#boolean-recap)
- [Why Do We Need Conditions?](#why-do-we-need-conditions)
- [The `if` Statement](#the-if-statement)
- [The `if...else` Statement](#the-ifelse-statement)
- [The `else if` Statement](#the-else-if-statement)
- [Nested `if`](#nested-if)
- [Real-World Examples](#real-world-examples)
- [Comparison Operators Review](#comparison-operators-review)
- [`==` vs `===`](#-vs-)
- [`!=` vs `!==`](#-vs--1)
- [Logical Operators](#logical-operators)
- [Combining Multiple Conditions](#combining-multiple-conditions)
- [Nested Conditions](#nested-conditions)
- [Ternary Operator (`? :`)](#ternary-operator--)
- [When to Use Ternary Operator](#when-to-use-ternary-operator)
- [Nested Ternary](#nested-ternary)
- [`switch` Statement](#switch-statement)
- [The `break` Keyword](#the-break-keyword)
- [Fall Through](#fall-through)
- [The `default` Case](#the-default-case)
- [`switch` vs `if...else`](#switch-vs-ifelse)
- [Practice Examples](#practice-examples)
- [Best Practices](#best-practices)
- [Common Beginner Mistakes](#common-beginner-mistakes)
- [Practice Tasks](#practice-tasks)
- [Interview Questions](#interview-questions)
- [What's Next?](#whats-next)

---

# Boolean Recap

A **Boolean** is a data type that has only two possible values.

```js
true
false
```

Example:

```js
let isStudent = true;
let hasLicense = false;
```

Many programming decisions are based on Boolean values.

---

# Why Do We Need Conditions?

Programs often need to make decisions based on different situations.

Examples:

- Is the user logged in?
- Is the age greater than or equal to 18?
- Is the password correct?
- Is the product in stock?

Instead of writing separate programs, we use **conditional statements** to decide what code should run.

---

# The `if` Statement

The `if` statement executes a block of code **only if the condition is true**.

### Syntax

```js
if (condition) {
  // code
}
```

Example:

```js
let age = 20;

if (age >= 18) {
  console.log("You can vote.");
}
```

Output:

```text
You can vote.
```

If the condition is `false`, nothing inside the block runs.

Example:

```js
let age = 15;

if (age >= 18) {
  console.log("You can vote.");
}
```

Output:

```text
(No output)
```

---

# The `if...else` Statement

Use `if...else` when there are **two possible outcomes**.

### Syntax

```js
if (condition) {
  // runs if true
} else {
  // runs if false
}
```

Example:

```js
let age = 16;

if (age >= 18) {
  console.log("Adult");
} else {
  console.log("Minor");
}
```

Output:

```text
Minor
```

---

# The `else if` Statement

Use `else if` when you have **multiple conditions** to check.

### Syntax

```js
if (condition1) {

} else if (condition2) {

} else {

}
```

Example:

```js
let marks = 75;

if (marks >= 80) {
  console.log("A+");
} else if (marks >= 70) {
  console.log("A");
} else if (marks >= 60) {
  console.log("A-");
} else {
  console.log("Needs Improvement");
}
```

Output:

```text
A
```

> ✅ Conditions are checked from top to bottom. As soon as one condition becomes `true`, the remaining conditions are skipped.

---

# Nested `if`

A **Nested `if`** means placing an `if` statement inside another `if` statement.

Example:

```js
let age = 22;
let hasID = true;

if (age >= 18) {
  if (hasID) {
    console.log("Entry Allowed");
  }
}
```

Output:

```text
Entry Allowed
```

Nested `if` is useful when one condition depends on another.

---

# Real-World Examples

## Example 1 — Login Check

```js
let isLoggedIn = true;

if (isLoggedIn) {
  console.log("Welcome Back!");
} else {
  console.log("Please Login.");
}
```

---

## Example 2 — Exam Result

```js
let marks = 45;

if (marks >= 33) {
  console.log("Pass");
} else {
  console.log("Fail");
}
```

---

## Example 3 — Even or Odd

```js
let number = 12;

if (number % 2 === 0) {
  console.log("Even");
} else {
  console.log("Odd");
}
```

---

## Example 4 — Positive, Negative, or Zero

```js
let number = -5;

if (number > 0) {
  console.log("Positive");
} else if (number < 0) {
  console.log("Negative");
} else {
  console.log("Zero");
}
```

---

# 💡 Tips

- Always use `===` instead of `==` unless you specifically need type coercion.
- Keep conditions simple and readable.
- Use proper indentation inside condition blocks.
- Avoid deeply nested `if` statements when a simpler solution exists.

---

# ✅ Key Takeaways

- Boolean values are either `true` or `false`.
- Conditional statements help programs make decisions.
- `if` executes code only when a condition is true.
- `if...else` handles two possible outcomes.
- `else if` is used for multiple conditions.
- Nested `if` allows one condition to depend on another.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 2 — Comparison & Logical Thinking**




# 📘 Module 08: JavaScript Conditionals & Decision Making

## 🧠 Part 2 — Comparison & Logical Thinking

---

# Comparison Operators Review

Comparison operators compare two values and return a **Boolean** (`true` or `false`).

| Operator | Meaning | Example | Result |
|----------|---------|---------|--------|
| `==` | Equal (Loose) | `5 == "5"` | `true` |
| `===` | Strict Equal | `5 === "5"` | `false` |
| `!=` | Not Equal (Loose) | `5 != "5"` | `false` |
| `!==` | Strict Not Equal | `5 !== "5"` | `true` |
| `>` | Greater Than | `10 > 5` | `true` |
| `<` | Less Than | `10 < 5` | `false` |
| `>=` | Greater Than or Equal | `18 >= 18` | `true` |
| `<=` | Less Than or Equal | `15 <= 20` | `true` |

Example:

```js
let age = 20;

console.log(age >= 18);
```

Output:

```text
true
```

---

# `==` vs `===`

Although both operators compare values, they work differently.

## Loose Equality (`==`)

`==` compares values **after automatic type conversion (type coercion)**.

Example:

```js
console.log(5 == "5");
```

Output:

```text
true
```

Why?

```text
"5" → 5
```

Then:

```text
5 == 5
```

Result:

```text
true
```

---

## Strict Equality (`===`)

`===` compares both the **value** and the **data type**.

Example:

```js
console.log(5 === "5");
```

Output:

```text
false
```

Because:

- First value → Number
- Second value → String

Different data types mean the comparison returns `false`.

---

# `!=` vs `!==`

Just like equality operators, inequality operators also have two versions.

Example:

```js
console.log(5 != "5");
```

Output:

```text
false
```

Example:

```js
console.log(5 !== "5");
```

Output:

```text
true
```

> ✅ In modern JavaScript, prefer using `===` and `!==` because they produce more predictable results.

---

# Logical Operators

Logical operators combine multiple conditions.

| Operator | Meaning |
|----------|---------|
| `&&` | AND |
| `\|\|` | OR |
| `!` | NOT |

---

# AND (`&&`)

Returns `true` **only if all conditions are true**.

Example:

```js
let age = 20;
let hasID = true;

console.log(age >= 18 && hasID);
```

Output:

```text
true
```

Another example:

```js
let age = 16;
let hasID = true;

console.log(age >= 18 && hasID);
```

Output:

```text
false
```

---

# OR (`||`)

Returns `true` if **at least one condition is true**.

Example:

```js
let isStudent = false;
let hasCoupon = true;

console.log(isStudent || hasCoupon);
```

Output:

```text
true
```

Another example:

```js
console.log(false || false);
```

Output:

```text
false
```

---

# NOT (`!`)

The NOT operator reverses a Boolean value.

Example:

```js
console.log(!true);
```

Output:

```text
false
```

Example:

```js
let isLoggedIn = false;

console.log(!isLoggedIn);
```

Output:

```text
true
```

---

# Combining Multiple Conditions

Logical operators can be combined to solve more complex problems.

Example:

```js
let age = 22;
let hasLicense = true;

if (age >= 18 && hasLicense) {
  console.log("You can drive.");
}
```

Output:

```text
You can drive.
```

---

Example:

```js
let isAdmin = false;
let isModerator = true;

if (isAdmin || isModerator) {
  console.log("Access Granted");
}
```

Output:

```text
Access Granted
```

---

# Nested Conditions

Sometimes one condition depends on another.

Example:

```js
let isLoggedIn = true;
let isPremium = false;

if (isLoggedIn) {
  if (isPremium) {
    console.log("Premium Content");
  } else {
    console.log("Free Content");
  }
}
```

Output:

```text
Free Content
```

---

# Real-World Practice

## Example 1 — Voting Eligibility

```js
let age = 19;
let citizen = true;

if (age >= 18 && citizen) {
  console.log("Eligible to Vote");
} else {
  console.log("Not Eligible");
}
```

---

## Example 2 — Login System

```js
let username = "admin";
let password = "12345";

if (username === "admin" && password === "12345") {
  console.log("Login Successful");
} else {
  console.log("Invalid Credentials");
}
```

---

## Example 3 — Free Delivery

```js
let totalPrice = 1200;

if (totalPrice >= 1000) {
  console.log("Free Delivery");
} else {
  console.log("Delivery Charge Applies");
}
```

---

## Example 4 — Weekend Check

```js
let day = "Friday";

if (day === "Friday" || day === "Saturday") {
  console.log("Weekend");
} else {
  console.log("Working Day");
}
```

---

# 🚫 Common Mistakes

## Using `=` instead of `===`

❌ Wrong

```js
if (age = 18) {

}
```

✅ Correct

```js
if (age === 18) {

}
```

---

## Using `==` unnecessarily

❌

```js
if (5 == "5") {

}
```

✅

```js
if (5 === "5") {

}
```

---

## Writing overly complex conditions

❌

```js
if ((age >= 18 && hasID) || (isAdmin && isVerified)) {

}
```

When conditions become too complex, split them into smaller variables for better readability.

---

# 💡 Tips

- Prefer `===` and `!==`.
- Use `&&` when **all conditions** must be true.
- Use `||` when **any one condition** is enough.
- Use `!` to reverse a Boolean value.
- Keep conditional expressions simple and readable.

---

# ✅ Key Takeaways

- Comparison operators return Boolean values.
- `===` checks both value and data type.
- `!==` is the strict version of "not equal".
- `&&` requires every condition to be true.
- `||` requires at least one condition to be true.
- `!` reverses a Boolean value.
- Logical operators help solve real-world decision-making problems.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 3 — Ternary Operator & Switch Statement**




# 📘 Module 08: JavaScript Conditionals & Decision Making

## ⚡ Part 3 — Ternary Operator & Switch Statement

---

# Ternary Operator (`? :`)

The **Ternary Operator** is a shorter way to write a simple `if...else` statement.

### Syntax

```js
condition ? valueIfTrue : valueIfFalse;
```

Example:

```js
let age = 20;

let message = age >= 18 ? "Adult" : "Minor";

console.log(message);
```

Output:

```text
Adult
```

Equivalent `if...else`:

```js
let age = 20;

let message;

if (age >= 18) {
  message = "Adult";
} else {
  message = "Minor";
}

console.log(message);
```

---

# When to Use Ternary Operator

✅ Good for:

- Simple conditions
- Assigning values
- Returning values
- Short, readable expressions

Example:

```js
let marks = 80;

let result = marks >= 33 ? "Pass" : "Fail";

console.log(result);
```

Output:

```text
Pass
```

---

# Nested Ternary

A ternary operator can be placed inside another ternary operator.

Example:

```js
let marks = 75;

let grade =
  marks >= 80
    ? "A+"
    : marks >= 70
    ? "A"
    : marks >= 60
    ? "A-"
    : "Fail";

console.log(grade);
```

Output:

```text
A
```

> ⚠ Nested ternary operators can quickly become difficult to read. Use them only for simple cases.

---

# `switch` Statement

The `switch` statement is used when one variable needs to be compared against multiple possible values.

Instead of writing many `else if` statements, `switch` often makes the code cleaner.

### Syntax

```js
switch (expression) {
  case value1:
    // code
    break;

  case value2:
    // code
    break;

  default:
    // code
}
```

---

# Example 1 — Weekday

```js
let day = "Friday";

switch (day) {
  case "Monday":
    console.log("Start of the week");
    break;

  case "Friday":
    console.log("Weekend is near");
    break;

  default:
    console.log("Regular Day");
}
```

Output:

```text
Weekend is near
```

---

# Example 2 — Grade

```js
let grade = "A";

switch (grade) {
  case "A":
    console.log("Excellent");
    break;

  case "B":
    console.log("Good");
    break;

  case "C":
    console.log("Average");
    break;

  default:
    console.log("Invalid Grade");
}
```

Output:

```text
Excellent
```

---

# The `break` Keyword

The `break` keyword stops the execution of the `switch` statement after a matching case.

Example:

```js
let fruit = "Apple";

switch (fruit) {
  case "Apple":
    console.log("Apple");
    break;

  case "Banana":
    console.log("Banana");
    break;
}
```

Output:

```text
Apple
```

Without `break`, JavaScript continues executing the following cases.

---

# Fall Through

If `break` is omitted, execution continues into the next case.

Example:

```js
let day = "Monday";

switch (day) {
  case "Monday":
    console.log("Monday");

  case "Tuesday":
    console.log("Tuesday");

  default:
    console.log("Other Day");
}
```

Output:

```text
Monday
Tuesday
Other Day
```

This behavior is called **Fall Through**.

> 💡 In most situations, you should use `break` to avoid unintended execution.

---

# The `default` Case

The `default` block runs when no case matches.

Example:

```js
let color = "Blue";

switch (color) {
  case "Red":
    console.log("Red");
    break;

  case "Green":
    console.log("Green");
    break;

  default:
    console.log("Unknown Color");
}
```

Output:

```text
Unknown Color
```

---

# `switch` vs `if...else`

| `switch` | `if...else` |
|----------|-------------|
| Best for checking one variable against many values | Best for complex conditions |
| Cleaner for fixed values | More flexible |
| Uses `case` and `break` | Uses conditions |

### Use `switch` when:

- Menu options
- Days of the week
- Months
- Grades
- Fixed values

### Use `if...else` when:

- Range checks
- Multiple logical conditions
- Complex decision-making

---

# Practice Examples

## Example 1 — Traffic Light

```js
let light = "Green";

switch (light) {
  case "Red":
    console.log("Stop");
    break;

  case "Yellow":
    console.log("Ready");
    break;

  case "Green":
    console.log("Go");
    break;

  default:
    console.log("Invalid Signal");
}
```

---

## Example 2 — Even or Odd (Ternary)

```js
let number = 9;

let result = number % 2 === 0 ? "Even" : "Odd";

console.log(result);
```

Output:

```text
Odd
```

---

## Example 3 — Login Status

```js
let isLoggedIn = true;

let message = isLoggedIn
  ? "Welcome Back!"
  : "Please Login";

console.log(message);
```

---

## Example 4 — Month Name

```js
let month = 2;

switch (month) {
  case 1:
    console.log("January");
    break;

  case 2:
    console.log("February");
    break;

  case 3:
    console.log("March");
    break;

  default:
    console.log("Invalid Month");
}
```

---

# 🚫 Common Mistakes

## Forgetting `break`

❌

```js
case "A":
  console.log("A");
```

Without `break`, execution continues to the next case.

---

## Overusing Nested Ternary

❌ Hard to Read

```js
let result =
  a
    ? b
      ? c
      : d
    : e;
```

✅ If the logic becomes complicated, use `if...else` instead.

---

## Using `switch` for Range Checks

❌

```js
switch (marks >= 80) {

}
```

✅ Use `if...else` for conditions involving ranges.

---

# 💡 Tips

- Use the ternary operator for short and simple conditions.
- Avoid deeply nested ternary operators.
- Always add `break` inside `switch` unless you intentionally want fall-through behavior.
- Use `switch` when comparing one variable with multiple fixed values.

---

# ✅ Key Takeaways

- The ternary operator is a concise alternative to `if...else`.
- Use nested ternary operators carefully.
- `switch` is useful for checking multiple fixed values.
- `break` prevents fall-through.
- `default` handles unmatched cases.
- Choose `switch` or `if...else` based on the type of condition.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 4 — Module Summary & TOC**





# 📘 Module 08: JavaScript Conditionals & Decision Making

## 🎯 Part 4 — Module Summary

---

# 📖 Module Summary

Congratulations! 🎉

You have completed **Module 08 – JavaScript Conditionals & Decision Making**.

In this module, you learned how JavaScript makes decisions based on different conditions. These concepts are essential because almost every real-world application uses conditional logic.

You learned:

- Boolean values
- `if` statement
- `if...else`
- `else if`
- Nested `if`
- Comparison operators
- Logical operators
- Ternary operator (`? :`)
- `switch` statement
- `break`
- `default`

These concepts will be used frequently in upcoming topics like loops, functions, arrays, objects, and DOM manipulation.

---

# 💡 Best Practices

- ✅ Prefer `===` and `!==` over `==` and `!=`.
- ✅ Keep conditions short and readable.
- ✅ Use meaningful variable names.
- ✅ Avoid deeply nested `if` statements whenever possible.
- ✅ Use the ternary operator only for simple conditions.
- ✅ Always use `break` in a `switch` statement unless fall-through is intentional.
- ✅ Choose the right conditional statement for the problem.

---

# 🚫 Common Beginner Mistakes

## 1. Using `=` instead of `===`

❌ Wrong

```js
if (age = 18) {

}
```

✅ Correct

```js
if (age === 18) {

}
```

---

## 2. Forgetting Curly Braces

❌

```js
if (age >= 18)
console.log("Adult");
```

✅

```js
if (age >= 18) {
  console.log("Adult");
}
```

Even if braces are optional for a single statement, using them improves readability and prevents bugs.

---

## 3. Writing Complex Conditions

❌

```js
if ((a && b) || (c && d) || (e && f)) {

}
```

✅ Break large conditions into smaller variables.

```js
const isEligible = age >= 18 && hasID;

if (isEligible) {
  console.log("Allowed");
}
```

---

## 4. Forgetting `break` in `switch`

❌

```js
case "A":
  console.log("Excellent");
```

Without `break`, JavaScript continues executing the next case.

---

## 5. Overusing Nested Ternary Operators

❌

```js
let result =
  a
    ? b
      ? c
      : d
    : e;
```

✅ Use `if...else` when the logic becomes difficult to read.

---

# 🎯 Practice Tasks

## Task 1

Create a variable named `age`.

Print:

- "Adult" if age is 18 or above.
- "Minor" otherwise.

---

## Task 2

Create a variable named `marks`.

Print:

- A+
- A
- A-
- B
- Fail

using `if...else if`.

---

## Task 3

Use a **Ternary Operator** to print:

- "Even"
- "Odd"

based on a number.

---

## Task 4

Create a `switch` statement for the days of the week.

Example:

```text
Monday
Tuesday
Wednesday
Thursday
Friday
Saturday
Sunday
```

Print a suitable message for each day.

---

## Task 5

Create a login system.

Conditions:

- Username is `"admin"`
- Password is `"12345"`

If both are correct:

```text
Login Successful
```

Otherwise:

```text
Invalid Credentials
```

---

# ❓ Interview Questions

### 1. What is a conditional statement?

A conditional statement allows a program to execute different code based on whether a condition is `true` or `false`.

---

### 2. What is the difference between `if`, `if...else`, and `else if`?

- `if` → Executes code only when the condition is true.
- `if...else` → Handles two possible outcomes.
- `else if` → Checks multiple conditions.

---

### 3. What is the difference between `==` and `===`?

- `==` compares values after type conversion.
- `===` compares both value and data type.

---

### 4. What are logical operators?

Logical operators combine or modify Boolean expressions.

Examples:

- `&&`
- `||`
- `!`

---

### 5. What is the ternary operator?

A shorthand version of an `if...else` statement.

Syntax:

```js
condition ? valueIfTrue : valueIfFalse;
```

---

### 6. When should you use a `switch` statement?

Use `switch` when comparing a single variable against multiple fixed values.

---

### 7. What is the purpose of `break`?

`break` stops the execution of a `switch` statement after a matching case.

---

### 8. What happens if `break` is omitted?

Execution continues to the next case. This behavior is called **Fall Through**.

---

# 📚 What's Next?

In the next module, you'll learn one of the most important concepts in JavaScript:

- Loops
- `for` Loop
- `while` Loop
- `do...while`
- `break`
- `continue`
- Nested Loops
- Loop Problem Solving

Loops allow you to execute the same block of code repeatedly, making your programs more efficient.

---

<div align="center">

### ⭐ If these notes helped you, consider giving this repository a star!

**Happy Coding! 🚀**

</div>
