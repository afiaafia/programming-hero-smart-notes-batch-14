# 📚 Programming Hero - Smart Notes

## Class 3-3

# 🆔 CSS ID Selector, Universal Selector & Background Color

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [🆔 What is an ID Selector?](#-what-is-an-id-selector)
- [🏷️ HTML Example](#️-html-example)
- [🎨 CSS Example](#-css-example)
- [❓ Why is `#` Used?](#-why-is--used)
- [📝 Rules for Using IDs](#-rules-for-using-ids)
- [📊 ID Selector vs Class Selector](#-id-selector-vs-class-selector)
- [🌍 Universal Selector](#-universal-selector)
- [🎨 Background Color](#-background-color)
- [🎨 Common Color Values](#-common-color-values)
- [💡 Best Practices](#-best-practices)
- [📚 Quick Revision](#-quick-revision)
- [📌 CSS Cheat Sheet](#-css-cheat-sheet)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- What is an ID Selector?
- How to Use the `id` Attribute
- ID Naming Rules
- Difference Between ID & Class

---

# 🆔 What is an ID Selector?

An **ID Selector** is used to style **one unique HTML element**.

Unlike a Class Selector, an ID should be used **only once** on a webpage.

> 💡 An ID Selector starts with the `#` symbol.

---

# 🏷️ HTML Example

```html
<h1 id="title">Welcome to Tasty Bites</h1>
```

---

# 🎨 CSS Example

```css
#title {
    color: blue;
}
```

### 🎨 Output Preview

```text
Welcome to Tasty Bites   ← Blue Heading
```

---

# ❓ Why is `#` Used?

In CSS:

- `#` → Selects an **ID**
- `.` → Selects a **Class**
- No symbol → Selects an **HTML Tag**

Example:

```css
#title { }
.title { }
h1 { }
```

---

# 📝 Rules for Using IDs

- ✅ Each ID should be **unique** on a webpage.
- ✅ One element should have only one unique ID.
- ✅ Do not use spaces in an ID name.
- ✅ Use meaningful names like `header`, `footer`, or `menu`.

Example:

```html
<h1 id="header">Welcome</h1>
```

---

# 📊 ID Selector vs Class Selector

| ID Selector | Class Selector |
|--------------|----------------|
| Uses `#` | Uses `.` |
| Styles one unique element | Styles one or more elements |
| Should be unique on a page | Can be reused multiple times |
| Example: `#header` | Example: `.title` |

---

# 🔍 Selector Visual

```text
Tag Selector
     │
     ▼
h1 { }

Class Selector
     │
     ▼
.title { }

ID Selector
     │
     ▼
#header { }
```

---

# ✅ Key Points

- An ID Selector styles a single unique element.
- The `#` symbol is used before an ID name.
- IDs should not be reused for multiple elements.
- Use a Class Selector when the same style is needed in multiple places.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 🌍 Universal Selector

The **Universal Selector** selects **every HTML element** on a webpage.

It is represented by the `*` (asterisk) symbol.

---

# ✨ Syntax

```css
* {
    margin: 0;
    padding: 0;
}
```

> 💡 This applies the same styles to all HTML elements.

---

# 📝 Example

### HTML

```html
<h1>Welcome</h1>

<p>Hello World!</p>

<button>Order Now</button>
```

### CSS

```css
* {
    color: darkblue;
}
```

### 🎨 Output Preview

```text
Welcome        ← Dark Blue

Hello World!   ← Dark Blue

Order Now      ← Dark Blue
```

---

# 🎨 Background Color

The `background-color` property is used to change the background color of an HTML element.

---

# 📝 Example 1: Change the Page Background

### CSS

```css
body {
    background-color: lightblue;
}
```

### 🎨 Output Preview

```text
Entire webpage background → Light Blue
```

---

# 📝 Example 2: Change a Specific Element's Background

### HTML

```html
<div class="offer">
    20% OFF Today!
</div>
```

### CSS

```css
.offer {
    background-color: yellow;
}
```

### 🎨 Output Preview

```text
🟨 20% OFF Today!
```

---

# 🎨 Common Color Values

You can use color names directly in CSS.

```css
color: red;
background-color: yellow;
```

Some common colors are:

- 🔴 Red
- 🔵 Blue
- 🟢 Green
- 🟡 Yellow
- ⚪ White
- ⚫ Black
- 🩶 Gray
- 🩵 LightBlue

---

# 📌 Summary

| Property / Selector | Purpose |
|---------------------|----------|
| `*` | Select all HTML elements |
| `background-color` | Change the background color of an element |
| `body` | Style the entire webpage |
| `.offer` | Style elements with the `offer` class |

---

# ✅ Key Points

- The Universal Selector (`*`) selects every HTML element.
- `background-color` changes an element's background color.
- The `body` selector is commonly used to style the whole webpage.
- Background colors can be applied to the page or to individual elements.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 💡 Best Practices

Follow these guidelines for writing clean and effective CSS:

- ✅ Use **ID Selectors** only for unique elements.
- ✅ Use **Class Selectors** for reusable styles.
- ✅ Use the **Universal Selector (`*`)** carefully, as it affects every element.
- ✅ Choose background colors that make text easy to read.
- ✅ Keep selector names meaningful and consistent.

---

# 📚 Quick Revision

## CSS Selectors Learned So Far

| Selector | Syntax | Selects |
|----------|--------|----------|
| Tag Selector | `h1` | All `<h1>` elements |
| Class Selector | `.title` | Elements with `class="title"` |
| ID Selector | `#header` | One unique element with `id="header"` |
| Universal Selector | `*` | Every HTML element |

---

# 🎨 Background Color

```css
body {
    background-color: lightblue;
}
```

Changes the background color of the selected element.

---

# 📌 CSS Cheat Sheet

| Syntax | Purpose |
|---------|----------|
| `#header { }` | ID Selector |
| `* { }` | Universal Selector |
| `background-color: yellow;` | Change background color |
| `color: blue;` | Change text color |
| `body { }` | Style the entire webpage |

---

# 🎯 Key Takeaways

- ✅ **ID Selectors** (`#`) are used for unique elements.
- ✅ **Universal Selectors** (`*`) apply styles to every HTML element.
- ✅ The `background-color` property changes an element's background color.
- ✅ **Class Selectors** are reusable, while **ID Selectors** should remain unique.
- ✅ Using the right selector makes your CSS cleaner and easier to maintain.

---

[⬆️ Back to Table of Contents](#-table-of-contents)
