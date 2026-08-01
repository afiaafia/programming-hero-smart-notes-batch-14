# 📘 Module 13: JavaScript Problem Solving

## 📖 Part 1 — Number Problem Solving

> **Programming Hero | Milestone 03 | Module 13**

---

# 📑 Table of Contents

- [The Problem-Solving Mindset](#the-problem-solving-mindset)
- [Steps to Solve Programming Problems](#steps-to-solve-programming-problems)
- [Even/Odd Checker](#evenodd-checker)
- [Sum of a Range](#sum-of-a-range)
- [Factorial](#factorial)
- [FizzBuzz](#fizzbuzz)
- [Reverse a String](#reverse-a-string)
- [Count Vowels](#count-vowels)
- [Palindrome Check](#palindrome-check)
- [Count Words](#count-words)
- [Find Largest Value](#find-largest-value)
- [Find Smallest Value](#find-smallest-value)
- [Sum & Average](#sum-and-average)
- [Filter by Condition](#filter-by-condition)
- [Loop Through Objects](#loop-through-objects)
- [Find a Value in an Object](#find-a-value-in-an-object)
- [Combining Function + Loop + Condition](#combining-function-loop-condition)
- [Best Practices](#best-practices)
- [Common Beginner Mistakes](#common-beginner-mistakes)
- [Practice Tasks](#practice-tasks)
- [Interview Questions](#interview-questions)
- [What's Next?](#whats-next)

---

<a id="the-problem-solving-mindset"></a>

# The Problem-Solving Mindset

Programming is not only about writing code. A good programmer first learns how to **think and solve problems**.

Before writing code, we need to understand:

1. What is the problem?
2. What input do we have?
3. What output do we need?
4. What steps are required to solve it?
5. How can we write those steps using code?

A strong problem-solving process helps you write cleaner and more efficient programs.

---

# Example of Problem-Solving Thinking

### Problem:

Find whether a number is even or odd.

Before coding:

### Input:

```text
A number
```

Example:

```text
10
```

### Process:

Check if the number is divisible by 2.

### Output:

```text
Even
```

Then convert the logic into JavaScript.

---

<a id="steps-to-solve-programming-problems"></a>

# Steps to Solve Programming Problems

A common problem-solving approach:

---

## Step 1 — Understand the Problem

Read the problem carefully.

Example:

> Find the sum of numbers from 1 to 10.

Understand:

- Starting number → 1
- Ending number → 10
- Required output → Total sum

---

## Step 2 — Break the Problem into Smaller Steps

Instead of solving everything at once:

```
Find Sum
   |
   ├── Start from 1
   |
   ├── Add each number
   |
   └── Store the result
```

---

## Step 3 — Write the Logic

Example:

```
Create a variable to store sum

Repeat through numbers

Add each number to sum

Return the result
```

---

## Step 4 — Convert Logic into Code

After understanding the solution, write JavaScript code.

---

## Step 5 — Test the Solution

Check with different inputs.

Example:

```text
Input: 5
Output: 15

Input: 10
Output: 55
```

---

<a id="evenodd-checker"></a>

# Even/Odd Checker

A number is:

- **Even** → Divisible by 2
- **Odd** → Not divisible by 2

We use the modulus operator `%`.

Example:

```js
10 % 2
```

Output:

```text
0
```

Because 10 is even.

---

## Logic

```
If number % 2 equals 0
    Number is Even
Otherwise
    Number is Odd
```

---

## JavaScript Solution

```js
function checkEvenOdd(number) {

  if (number % 2 === 0) {
    return "Even";
  }

  return "Odd";
}

console.log(checkEvenOdd(7));
```

Output:

```text
Odd
```

---

### Another Example

```js
console.log(checkEvenOdd(12));
```

Output:

```text
Even
```

---

<a id="sum-of-a-range"></a>

# Sum of a Range

The goal is to find the total of numbers between two values.

Example:

```
1 + 2 + 3 + 4 + 5
```

Output:

```
15
```

---

## Logic

```
Create sum variable = 0

Start loop from starting number

Add each number to sum

Return sum
```

---

## JavaScript Solution

```js
function sumRange(start, end) {

  let sum = 0;

  for (let i = start; i <= end; i++) {
    sum += i;
  }

  return sum;
}

console.log(sumRange(1, 5));
```

Output:

```text
15
```

---

### Another Example

```js
console.log(sumRange(1, 10));
```

Output:

```text
55
```

---

<a id="factorial"></a>

# Factorial

Factorial means multiplying a number by all positive numbers below it.

Example:

```
5! = 5 × 4 × 3 × 2 × 1
```

Output:

```
120
```

---

## Logic

```
Create result = 1

Loop from 1 to number

Multiply result with each value

Return result
```

---

## JavaScript Solution

```js
function factorial(number) {

  let result = 1;

  for (let i = 1; i <= number; i++) {
    result *= i;
  }

  return result;
}

console.log(factorial(5));
```

Output:

```text
120
```

---

### Factorial Examples

```text
3! = 3 × 2 × 1 = 6

4! = 4 × 3 × 2 × 1 = 24

5! = 5 × 4 × 3 × 2 × 1 = 120
```

---

<a id="fizzbuzz"></a>

# FizzBuzz

FizzBuzz is a very popular programming problem.

Rules:

- If number is divisible by 3 → Print `"Fizz"`
- If number is divisible by 5 → Print `"Buzz"`
- If number is divisible by both 3 and 5 → Print `"FizzBuzz"`
- Otherwise → Print the number

---

## Example

For numbers 1 to 15:

```text
1
2
Fizz
4
Buzz
Fizz
7
8
Fizz
Buzz
11
Fizz
13
14
FizzBuzz
```

---

## Logic

```
Check divisible by 15 first

Otherwise check divisible by 3

Otherwise check divisible by 5

Otherwise print the number
```

---

## JavaScript Solution

```js
function fizzBuzz(number) {

  if (number % 15 === 0) {
    return "FizzBuzz";
  }

  else if (number % 3 === 0) {
    return "Fizz";
  }

  else if (number % 5 === 0) {
    return "Buzz";
  }

  else {
    return number;
  }

}

console.log(fizzBuzz(15));
```

Output:

```text
FizzBuzz
```

---

# 📝 Practice Problems

## Problem 1 — Check Even or Odd

Create a function that takes a number and returns:

```text
Even
```

or

```text
Odd
```

---

## Problem 2 — Sum of Numbers

Create a function that finds the sum from 1 to a given number.

Example:

```js
sum(5)
```

Output:

```text
15
```

---

## Problem 3 — Calculate Factorial

Create a function that calculates factorial.

Example:

```js
factorial(4)
```

Output:

```text
24
```

---

## Problem 4 — FizzBuzz

Create a function that follows the FizzBuzz rules.

---

# 💡 Tips

- Understand the problem before writing code.
- Break large problems into smaller steps.
- Write the logic using simple words first.
- Use functions to make solutions reusable.
- Test your code with multiple inputs.

---

# ✅ Key Takeaways

- Problem solving starts before writing code.
- A good programmer focuses on logic, not only syntax.
- Most problems can be solved by breaking them into smaller steps.
- Loops and conditions are powerful tools for solving problems.
- Functions make problem solutions reusable.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 2 — String Problem Solving**




# 📘 Module 13: JavaScript Problem Solving

## 📖 Part 2 — String Problem Solving

> **Programming Hero | Milestone 03 | Module 13**

---

<a id="reverse-a-string"></a>

# Reverse a String

Reversing a string means changing the order of characters from the end to the beginning.

Example:

```
Input:
hello

Output:
olleh
```

---

## Problem-Solving Approach

### Given:

```text
A string
```

### Need:

```text
Reverse order of characters
```

### Logic:

```
Take the string

Loop through characters from last to first

Store each character

Return the reversed string
```

---

## JavaScript Solution (Using Loop)

```js
function reverseString(str) {

  let reversed = "";

  for (let i = str.length - 1; i >= 0; i--) {
    reversed += str[i];
  }

  return reversed;
}

console.log(reverseString("hello"));
```

Output:

```text
olleh
```

---

## Alternative Solution (Using Array Methods)

```js
function reverseString(str) {

  return str
    .split("")
    .reverse()
    .join("");

}

console.log(reverseString("javascript"));
```

Output:

```text
tpircsavaj
```

---

### How It Works

```js
str.split("")
```

Converts string into an array.

Example:

```js
"hello"
```

becomes:

```js
["h", "e", "l", "l", "o"]
```

---

```js
.reverse()
```

Reverses the array:

```js
["o", "l", "l", "e", "h"]
```

---

```js
.join("")
```

Converts array back into a string:

```text
olleh
```

---

<a id="count-vowels"></a>

# Count Vowels

A vowel is one of:

```text
a, e, i, o, u
```

The goal is to count how many vowels exist in a string.

Example:

```
Input:
javascript

Output:
3
```

Because:

```
a
a
i
```

---

## Problem-Solving Approach

### Logic:

```
Create count variable

Loop through each character

Check if character is a vowel

Increase count

Return count
```

---

## JavaScript Solution

```js
function countVowels(str) {

  let count = 0;

  for (let char of str) {

    if (
      char === "a" ||
      char === "e" ||
      char === "i" ||
      char === "o" ||
      char === "u"
    ) {
      count++;
    }

  }

  return count;
}

console.log(countVowels("javascript"));
```

Output:

```text
3
```

---

## Better Approach Using Includes()

The `includes()` method checks whether a value exists inside a string.

Example:

```js
let vowels = "aeiou";

console.log(vowels.includes("a"));
```

Output:

```text
true
```

---

### Solution

```js
function countVowels(str) {

  let count = 0;
  let vowels = "aeiou";

  for (let char of str.toLowerCase()) {

    if (vowels.includes(char)) {
      count++;
    }

  }

  return count;
}

console.log(countVowels("Programming"));
```

Output:

```text
3
```

---

<a id="palindrome-check"></a>

# Palindrome Check

A palindrome is a word that remains the same when reversed.

Examples:

```
madam
level
racecar
```

Reverse করলে same থাকে।

---

## Problem-Solving Approach

Example:

```
Input:
madam
```

Steps:

```
Original string:
madam

Reverse string:
madam

Compare both

If same → Palindrome
Otherwise → Not Palindrome
```

---

## JavaScript Solution

```js
function isPalindrome(str) {

  let reversed = str
    .split("")
    .reverse()
    .join("");

  return str === reversed;
}

console.log(isPalindrome("madam"));
```

Output:

```text
true
```

---

### Another Example

```js
console.log(isPalindrome("hello"));
```

Output:

```text
false
```

---

<a id="count-words"></a>

# Count Words

The goal is to count the number of words in a sentence.

Example:

```
Input:
I love JavaScript

Output:
3
```

---

## Problem-Solving Approach

Words are separated by spaces.

Logic:

```
Take the sentence

Split it by spaces

Count the array length

Return the result
```

---

## JavaScript Solution

```js
function countWords(sentence) {

  let words = sentence.split(" ");

  return words.length;
}

console.log(countWords("I love JavaScript"));
```

Output:

```text
3
```

---

## Handling Extra Spaces

Sometimes sentences contain extra spaces.

Example:

```text
"  I love JavaScript  "
```

Use `trim()`:

```js
function countWords(sentence) {

  let words = sentence.trim().split(" ");

  return words.length;
}

console.log(countWords("  I love JavaScript  "));
```

Output:

```text
3
```

---

# 📝 Practice Problems

## Problem 1 — Reverse a String

Create a function that reverses a string.

Example:

```js
reverseString("hello")
```

Output:

```text
olleh
```

---

## Problem 2 — Count Vowels

Create a function that counts vowels.

Example:

```js
countVowels("education")
```

Output:

```text
5
```

---

## Problem 3 — Check Palindrome

Create a function that checks whether a string is a palindrome.

Example:

```js
isPalindrome("level")
```

Output:

```text
true
```

---

## Problem 4 — Count Words

Create a function that counts words in a sentence.

Example:

```js
countWords("I learn JavaScript")
```

Output:

```text
3
```

---

# 💡 Tips

- Strings are iterable, so you can loop through characters.
- Use `.split()` to convert strings into arrays.
- Use `.reverse()` to reverse arrays.
- Use `.join()` to convert arrays back into strings.
- Use `.toLowerCase()` when comparing text without case sensitivity.
- Break string problems into small logical steps.

---

# ✅ Key Takeaways

- Strings can be manipulated using loops and built-in methods.
- Reversing a string is a common programming problem.
- `includes()` helps check whether a value exists.
- Palindrome problems require comparing original and reversed values.
- `split()` is useful for counting words.
- Problem-solving skills are more important than memorizing syntax.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 3 — Array & Object Problem Solving**





# 📘 Module 13: JavaScript Problem Solving

## 📖 Part 3 — Array & Object Problem Solving

> **Programming Hero | Milestone 03 | Module 13**

---

<a id="find-largest-value"></a>

# Find the Largest Value in an Array

Finding the largest number from an array is a very common programming problem.

Example:

```js
let numbers = [10, 25, 5, 40, 15];
```

Output:

```text
40
```

---

## Problem-Solving Approach

### Logic:

```
Take the first value as largest

Loop through the array

Compare each value with largest

If current value is bigger:
    Update largest

Return largest value
```

---

## JavaScript Solution

```js
function findLargest(numbers) {

  let largest = numbers[0];

  for (let number of numbers) {

    if (number > largest) {
      largest = number;
    }

  }

  return largest;
}

console.log(findLargest([10, 25, 5, 40, 15]));
```

Output:

```text
40
```

---

## Using Math.max()

JavaScript also provides a built-in method:

```js
function findLargest(numbers) {

  return Math.max(...numbers);

}

console.log(findLargest([10, 25, 5, 40, 15]));
```

Output:

```text
40
```

---

<a id="find-smallest-value"></a>

# Find the Smallest Value in an Array

This is similar to finding the largest value.

Example:

```js
let numbers = [10, 25, 5, 40, 15];
```

Output:

```text
5
```

---

## Logic:

```
Take the first value as smallest

Loop through the array

Compare each value

If current value is smaller:
    Update smallest

Return smallest
```

---

## JavaScript Solution

```js
function findSmallest(numbers) {

  let smallest = numbers[0];

  for (let number of numbers) {

    if (number < smallest) {
      smallest = number;
    }

  }

  return smallest;
}

console.log(findSmallest([10, 25, 5, 40, 15]));
```

Output:

```text
5
```

---

## Using Math.min()

```js
function findSmallest(numbers) {

  return Math.min(...numbers);

}

console.log(findSmallest([10, 25, 5, 40, 15]));
```

Output:

```text
5
```

---

<a id="sum-and-average"></a>

# Sum & Average of Array Values

Finding the total and average of numbers is another common problem.

Example:

```js
let numbers = [10, 20, 30];
```

Sum:

```text
60
```

Average:

```text
20
```

---

## Find Sum

### Logic:

```
Create sum = 0

Loop through array

Add each value

Return sum
```

---

## JavaScript Solution

```js
function sumArray(numbers) {

  let sum = 0;

  for (let number of numbers) {
    sum += number;
  }

  return sum;
}

console.log(sumArray([10, 20, 30]));
```

Output:

```text
60
```

---

## Find Average

Formula:

```
Average = Total Sum / Number of Elements
```

---

```js
function average(numbers) {

  let sum = 0;

  for (let number of numbers) {
    sum += number;
  }

  return sum / numbers.length;

}

console.log(average([10, 20, 30]));
```

Output:

```text
20
```

---

<a id="filter-by-condition"></a>

# Filter Array by Condition

Sometimes we need to find specific values from an array based on a condition.

Example:

Find even numbers:

```js
[1, 2, 3, 4, 5, 6]
```

Output:

```text
[2, 4, 6]
```

---

## Logic:

```
Create an empty array

Loop through original array

Check condition

If condition is true:
    Add value to new array

Return new array
```

---

## JavaScript Solution

```js
function filterEven(numbers) {

  let evenNumbers = [];

  for (let number of numbers) {

    if (number % 2 === 0) {
      evenNumbers.push(number);
    }

  }

  return evenNumbers;
}

console.log(filterEven([1, 2, 3, 4, 5, 6]));
```

Output:

```text
[2, 4, 6]
```

---

## Using Array Filter Method

```js
let numbers = [1, 2, 3, 4, 5, 6];

let evenNumbers = numbers.filter(number => number % 2 === 0);

console.log(evenNumbers);
```

Output:

```text
[2, 4, 6]
```

---

<a id="loop-through-objects"></a>

# Loop Through Objects

Objects store data using key-value pairs.

Example:

```js
let student = {
  name: "Alice",
  age: 20,
  grade: "A"
};
```

---

## Using `for...in`

```js
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

<a id="find-a-value-in-an-object"></a>

# Find a Value in an Object

Sometimes we need to search for a specific value inside an object.

Example:

```js
let product = {
  name: "Laptop",
  price: 65000,
  brand: "Dell"
};
```

Find whether the brand is Dell.

---

## Solution

```js
function findValue(object, searchValue) {

  for (let key in object) {

    if (object[key] === searchValue) {
      return true;
    }

  }

  return false;
}

console.log(findValue(product, "Dell"));
```

Output:

```text
true
```

---

<a id="combining-function-loop-condition"></a>

# Combining Function + Loop + Condition

Many real programming problems require using:

- Function
- Loop
- Condition

together.

Example:

Find numbers greater than 10.

---

## Solution

```js
function findGreater(numbers) {

  let result = [];

  for (let number of numbers) {

    if (number > 10) {
      result.push(number);
    }

  }

  return result;
}

console.log(findGreater([5, 12, 20, 8, 15]));
```

Output:

```text
[12, 20, 15]
```

---

# Real-World Practice Problems

## Problem 1 — Find Maximum Price

```js
let products = [
  {
    name: "Laptop",
    price: 65000
  },
  {
    name: "Phone",
    price: 30000
  }
];
```

Find the product with the highest price.

---

## Problem 2 — Filter Students

```js
let students = [
  {
    name: "Alice",
    marks: 85
  },
  {
    name: "Bob",
    marks: 45
  }
];
```

Find students who passed.

---

## Problem 3 — Calculate Total Cart Price

```js
let cart = [
  {
    name: "Book",
    price: 500
  },
  {
    name: "Pen",
    price: 50
  }
];
```

Calculate total price.

---

# 💡 Tips

- Start with simple logic before writing code.
- Use loops when checking every element.
- Use conditions to make decisions.
- Use functions to organize solutions.
- Arrays and objects are commonly combined in real applications.

---

# ✅ Key Takeaways

- Arrays can be solved using loops and conditions.
- Finding maximum/minimum values is a common pattern.
- Sum and average problems require accumulation logic.
- Filtering means selecting values based on conditions.
- Objects can be searched using loops.
- Real-world problems often combine functions, loops, and conditions.

---

⬆️ [Back to Table of Contents](#-table-of-contents)

➡ Continue to **Part 4 — Module Summary**





# 📘 Module 13: JavaScript Problem Solving

## 🎯 Part 4 — Module Summary

> **Programming Hero | Milestone 03 | Module 13**

---

# 📖 Module Summary

Congratulations! 🎉

You have completed **Module 13 – JavaScript Problem Solving**.

In this module, you learned how to approach programming problems step-by-step and convert logical solutions into JavaScript code.

Problem-solving is one of the most important skills for becoming a strong developer. Knowing syntax is not enough; understanding how to break down a problem and create a solution is the key.

In this module, you learned:

- Problem-Solving Mindset
- Steps to Solve Programming Problems
- Even/Odd Checker
- Sum of a Range
- Factorial
- FizzBuzz
- Reverse a String
- Count Vowels
- Palindrome Check
- Count Words
- Find Largest Value
- Find Smallest Value
- Sum & Average of Array
- Filter Array by Condition
- Loop Through Objects
- Find Values in Objects
- Combining Function + Loop + Condition

These concepts build the foundation for advanced programming, DSA, coding interviews, and real-world development.

---

<a id="best-practices"></a>

# 💡 Best Practices

- ✅ Understand the problem before writing code.
- ✅ Write the solution steps in plain language first.
- ✅ Break large problems into smaller tasks.
- ✅ Use functions to create reusable solutions.
- ✅ Choose meaningful variable and function names.
- ✅ Test your solution with different inputs.
- ✅ Focus on logic instead of memorizing code.
- ✅ Keep your code simple and readable.

---

<a id="common-beginner-mistakes"></a>

# 🚫 Common Beginner Mistakes

## 1. Starting Coding Without Understanding the Problem

❌ Wrong approach:

Immediately writing code without knowing:

- Input
- Output
- Required logic

✅ Better approach:

First analyze the problem, then write the solution.

---

## 2. Trying to Solve Everything at Once

Complex problems become easier when divided into smaller steps.

Example:

Instead of:

```
Solve the whole problem
```

Think:

```
Understand input
↓
Create logic
↓
Write code
↓
Test output
```

---

## 3. Forgetting Edge Cases

A solution should handle unusual inputs.

Example:

```js
[]
```

or

```js
0
```

or

```js
""
```

---

## 4. Using Incorrect Loop Conditions

Example:

❌

```js
for(let i = 0; i < numbers.length - 1; i++)
```

This skips the last element.

Always check your loop condition carefully.

---

## 5. Writing Duplicate Code

❌

```js
console.log(square(5));
console.log(square(10));
console.log(square(15));
```

Repeating logic makes code harder to maintain.

✅ Use reusable functions.

---

<a id="practice-tasks"></a>

# 🎯 Practice Tasks

## Number Problems

### Task 1

Create a function that checks whether a number is positive, negative, or zero.

---

### Task 2

Create a function that calculates the sum from 1 to N.

Example:

```js
sum(10)
```

Output:

```text
55
```

---

### Task 3

Create a function that calculates factorial.

Example:

```js
factorial(5)
```

Output:

```text
120
```

---

### Task 4

Implement FizzBuzz from 1 to 100.

---

# String Problems

### Task 5

Create a function to reverse a string.

---

### Task 6

Create a function that counts vowels.

---

### Task 7

Create a function that checks whether a word is a palindrome.

---

### Task 8

Create a function that counts words in a sentence.

---

# Array Problems

### Task 9

Find the largest number in an array.

---

### Task 10

Find the smallest number in an array.

---

### Task 11

Calculate the average value of an array.

---

### Task 12

Filter numbers greater than 50.

---

# Object Problems

### Task 13

Create a function that loops through an object and prints:

```text
key : value
```

---

### Task 14

Create a function that searches for a specific value inside an object.

---

### Task 15

Create an array of objects representing products and calculate the total price.

---

<a id="interview-questions"></a>

# ❓ Interview Questions

### 1. What is problem-solving in programming?

Problem-solving is the process of analyzing a problem, creating a logical solution, and implementing it using code.

---

### 2. What are the basic steps of solving a programming problem?

Steps:

1. Understand the problem
2. Identify input and output
3. Create an algorithm
4. Write code
5. Test the solution

---

### 3. Why are functions useful in problem solving?

Functions help organize logic into reusable blocks and make code easier to maintain.

---

### 4. What is the purpose of a loop in problem solving?

Loops allow us to repeat operations efficiently without writing the same code multiple times.

---

### 5. Why do we use conditions?

Conditions allow programs to make decisions based on different situations.

---

### 6. What is FizzBuzz and why is it popular?

FizzBuzz is a simple programming problem used to test understanding of loops and conditions.

---

### 7. How do you find the largest value in an array?

Compare each value with a stored maximum value and update it when a larger value is found.

---

### 8. How do you reverse a string?

A string can be reversed by looping from the end or using array methods like:

```js
split()
reverse()
join()
```

---

### 9. Why are edge cases important?

Edge cases help ensure that a program works correctly for unusual or unexpected inputs.

---

### 10. What concepts are commonly combined in problem solving?

Usually:

- Functions
- Loops
- Conditions
- Arrays
- Objects

---

<a id="whats-next"></a>

# 📚 What's Next?

In the upcoming modules, you will continue learning more advanced JavaScript concepts.

You will explore:

- Modern JavaScript features
- ES6 syntax
- Cleaner ways to write JavaScript
- More powerful programming techniques

These concepts will help you write professional-level JavaScript code and prepare you for frontend frameworks like React.

---

<div align="center">

### ⭐ If these notes helped you, consider giving this repository a star!

**Happy Coding! 🚀**

</div>
