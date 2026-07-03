# 📚 Programming Hero - Smart Notes

## Class 3-2

# 🎯 CSS Selectors: Tag & Class Selector

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [🎯 What is a CSS Selector?](#-what-is-a-css-selector)
- [🤔 Why Use Selectors?](#-why-use-selectors)
- [🏷️ Tag Selector](#️-tag-selector)
- [🏷️ Class Selector](#️-class-selector)
- [🔍 Selector Visual](#-selector-visual)
- [📊 Tag Selector vs Class Selector](#-tag-selector-vs-class-selector)
- [🎨 Inline CSS Practice](#-inline-css-practice)
- [🎨 Internal CSS Practice](#-internal-css-practice)
- [🧪 Combining Different CSS Methods](#-combining-different-css-methods)
- [💡 Best Practices](#-best-practices)
- [📚 Quick Revision](#-quick-revision)
- [📌 CSS Cheat Sheet](#-css-cheat-sheet)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- What is a CSS Selector?
- Why Selectors are Used
- Tag Selector
- Class Selector
- Difference Between Tag & Class Selectors

---

# 🎯 What is a CSS Selector?

A **CSS Selector** is used to select HTML elements so that CSS styles can be applied to them.

Without selectors, CSS wouldn't know which element to style.

> 💡 Simply put, a selector tells CSS **"which HTML element should be styled."**

---

# 🤔 Why Use Selectors?

Selectors help you:

- Style specific HTML elements.
- Reuse the same styles.
- Keep your code clean and organized.
- Make website design easier to manage.

---

# 🏷️ Tag Selector

A **Tag Selector** selects **all HTML elements** with the same tag name.

### HTML

```html
<h1>Welcome</h1>
<h1>Hello</h1>
```

### CSS

```css
h1 {
    color: blue;
}
```

### 🎨 Output Preview

```text
Welcome   ← Blue
Hello     ← Blue
```

> 💡 Every `<h1>` element will receive the same style.

---

# 🏷️ Class Selector

A **Class Selector** styles only the elements that have a specific `class` attribute.

### HTML

```html
<h1 class="title">Welcome</h1>
<p class="title">Hello World</p>
```

### CSS

```css
.title {
    color: red;
}
```

> 💡 The `.` (dot) is used before the class name.

### 🎨 Output Preview

```text
Welcome      ← Red
Hello World  ← Red
```

---

# 🔍 Selector Visual

```text
Tag Selector
     │
     ▼
h1 { }

Styles every <h1>

----------------------

Class Selector
     │
     ▼
.title { }

Styles every element with class="title"
```

---

# 📊 Tag Selector vs Class Selector

| Tag Selector | Class Selector |
|--------------|----------------|
| Selects by HTML tag | Selects by class name |
| Styles all matching tags | Styles only selected elements |
| Example: `h1` | Example: `.title` |

---

# ✅ Key Points

- CSS selectors tell the browser which elements to style.
- A Tag Selector affects all matching HTML tags.
- A Class Selector affects only elements with a specific class.
- Class Selectors are more flexible and reusable than Tag Selectors.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 🎨 Inline CSS Practice

Inline CSS applies styles directly to an HTML element using the `style` attribute.

### Example

```html
<h2 style="color: green;">Welcome to Tasty Bites</h2>
```

### 🎨 Output Preview

```text
Welcome to Tasty Bites   ← Green Heading
```

### 📌 Features

- Applied to a single element.
- Highest priority among basic CSS methods.
- Not recommended for large projects.

---

# 🎨 Internal CSS Practice

Internal CSS is written inside the `<style>` tag, usually in the `<head>` section.

### HTML

```html
<head>
    <style>
        h2 {
            color: blue;
        }

        .special {
            color: red;
        }
    </style>
</head>
```

### HTML Body

```html
<h2>Today's Menu</h2>

<p class="special">
    Special Offer Today!
</p>
```

### 🎨 Output Preview

```text
Today's Menu         ← Blue

Special Offer Today! ← Red
```

---

# 🧪 Combining Different CSS Methods

You can use multiple CSS methods in the same HTML file.

### Example

```html
<head>
    <style>
        h1 {
            color: blue;
        }

        .offer {
            color: red;
        }
    </style>
</head>

<body>

<h1>Welcome</h1>

<p class="offer">
    20% OFF Today!
</p>

<h2 style="color: green;">
    Enjoy Your Meal
</h2>

</body>
```

### 🎨 Output Preview

```text
Welcome            ← Blue

20% OFF Today!     ← Red

Enjoy Your Meal    ← Green
```

---

# 📌 Summary

| CSS Method | Where It Is Written |
|------------|---------------------|
| Inline CSS | Inside the `style` attribute |
| Internal CSS | Inside the `<style>` tag |
| Tag Selector | Selects HTML tags |
| Class Selector | Selects elements with a specific class |

---

# ✅ Key Points

- Inline CSS styles only one element.
- Internal CSS styles multiple elements on the same page.
- Tag Selectors target HTML tags.
- Class Selectors target specific elements using the `class` attribute.
- Different CSS methods can be used together when needed.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 💡 Best Practices

Follow these tips to write clean and organized CSS:

- ✅ Prefer **Class Selectors** over Tag Selectors when possible.
- ✅ Avoid using too much **Inline CSS**.
- ✅ Use **Internal CSS** only for small projects or practice.
- ✅ Give classes meaningful names (e.g., `.title`, `.menu-item`, `.offer`).
- ✅ Keep your HTML clean and your CSS organized.

---

# 📚 Quick Revision

### CSS Selector

A selector tells CSS **which HTML element to style**.

---

### Types of Selectors Learned

| Selector | Example | Selects |
|----------|---------|----------|
| Tag Selector | `h1` | All `<h1>` elements |
| Class Selector | `.title` | All elements with `class="title"` |

---

### Ways to Add CSS

| Method | Example |
|---------|----------|
| Inline CSS | `style=""` |
| Internal CSS | `<style>...</style>` |

> 💡 **External CSS** was introduced in the previous class and is the recommended approach for real-world projects.

---

# 📌 CSS Cheat Sheet

| Syntax | Purpose |
|---------|----------|
| `h1 { }` | Tag Selector |
| `.title { }` | Class Selector |
| `style=""` | Inline CSS |
| `<style>...</style>` | Internal CSS |
| `color: blue;` | Change text color |
| `background-color: yellow;` | Change background color |

---

# 🎯 Key Takeaways

- ✅ CSS Selectors are used to choose which HTML elements will be styled.
- ✅ A **Tag Selector** styles all matching HTML tags.
- ✅ A **Class Selector** styles only elements with a specific class.
- ✅ **Inline CSS** is useful for quick styling but should be used sparingly.
- ✅ **Internal CSS** is suitable for styling a single webpage.
- ✅ **Class Selectors** are more flexible and reusable than **Tag Selectors**.

---

[⬆️ Back to Table of Contents](#-table-of-contents)
