# 📚 Programming Hero - Smart Notes

## Class 3-1

# 🎨 CSS Basics: Inline, Internal & External Styles

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [🎨 What is CSS?](#-what-is-css)
- [🤔 Why Use CSS?](#-why-use-css)
- [⚖️ HTML vs CSS](#️-html-vs-css)
- [🧩 CSS Syntax](#-css-syntax)
- [💬 CSS Comments](#-css-comments)
- [🎨 Three Ways to Add CSS](#-three-ways-to-add-css)
- [1️⃣ Inline CSS](#1️⃣-inline-css)
- [2️⃣ Internal CSS](#2️⃣-internal-css)
- [3️⃣ External CSS](#3️⃣-external-css-)
- [📊 Comparison](#-comparison)
- [💡 Best Practices](#-best-practices)
- [📚 Quick Revision](#-quick-revision)
- [📌 CSS Cheat Sheet](#-css-cheat-sheet)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- What is CSS?
- Why CSS is Used
- HTML vs CSS
- CSS Syntax
- CSS Comments

---

# 🎨 What is CSS?

**CSS (Cascading Style Sheets)** is a stylesheet language used to style HTML webpages.

It controls how HTML elements look, including their:

- Colors
- Fonts
- Spacing
- Sizes
- Layout

> 💡 HTML creates the structure, while CSS makes it beautiful.

---

# 🤔 Why Use CSS?

CSS helps make websites more attractive and user-friendly.

Some common uses of CSS are:

- 🎨 Add colors
- 🔠 Change fonts
- 📏 Control spacing
- 📦 Create layouts
- ✨ Improve the overall design

---

# ⚖️ HTML vs CSS

| HTML | CSS |
|------|------|
| Creates the webpage structure | Styles the webpage |
| Uses HTML tags | Uses selectors and properties |
| Defines content | Controls appearance |

---

# 🧩 CSS Syntax

A CSS rule consists of a **selector**, a **property**, and a **value**.

```css
h1 {
    color: blue;
}
```

### Explanation

- **Selector:** `h1`
- **Property:** `color`
- **Value:** `blue`

---

# 💬 CSS Comments

Comments are ignored by the browser and are used to write notes.

```css
/* This is a CSS comment */
```

---

# 📌 Quick Revision

| Term | Meaning |
|------|---------|
| Selector | Selects the HTML element |
| Property | Defines what to change |
| Value | Sets the property's value |

---

# ✅ Key Points

- CSS is used to style HTML webpages.
- HTML provides the structure, while CSS controls the design.
- Every CSS rule contains a selector, property, and value.
- Comments help organize CSS code but are not displayed in the browser.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 🎨 Three Ways to Add CSS

CSS can be added to an HTML document in **three different ways**.

---

# 1️⃣ Inline CSS

Inline CSS is written directly inside an HTML element using the `style` attribute.

### Example

```html
<h1 style="color: red;">Welcome!</h1>
```

### ✅ Advantages

- Easy for small changes.
- Useful for testing styles quickly.

### ❌ Disadvantages

- Makes HTML messy.
- Difficult to maintain.
- Not recommended for large projects.

### 🎨 Output Preview

```text
Welcome!   ← Red Heading
```

---

# 2️⃣ Internal CSS

Internal CSS is written inside the `<style>` tag, usually within the `<head>` section of an HTML document.

### Example

```html
<head>
    <style>
        h1 {
            color: blue;
        }
    </style>
</head>
```

### ✅ Advantages

- Styles multiple elements on the same page.
- Keeps HTML cleaner than Inline CSS.

### ❌ Disadvantages

- Works only for a single HTML page.
- Not suitable for multi-page websites.

### 🎨 Output Preview

```text
Welcome!   ← Blue Heading
```

---

# 3️⃣ External CSS ⭐

External CSS stores all styles in a separate `.css` file and links it to the HTML document.

### HTML

```html
<link rel="stylesheet" href="style.css">
```

### CSS (`style.css`)

```css
h1 {
    color: green;
}
```

### ✅ Advantages

- Keeps HTML clean.
- Easy to maintain.
- Reusable across multiple pages.
- Best practice for real-world projects.

### ❌ Disadvantages

- Requires an extra CSS file.

### 🎨 Output Preview

```text
Welcome!   ← Green Heading
```

---

# 📊 Comparison

| Inline | Internal | External |
|---------|----------|----------|
| One element | One page | Multiple pages |
| Uses `style` attribute | Uses `<style>` tag | Uses a separate `.css` file |
| Not recommended | Good for small pages | ⭐ Best Practice |

---

# ✅ Key Points

- Inline CSS is best for quick testing.
- Internal CSS is suitable for a single page.
- External CSS is the recommended approach for most websites.

---

[⬆️ Back to Table of Contents](#-table-of-contents)


# 💡 Best Practices

Follow these practices to write clean and maintainable CSS:

- Prefer **External CSS** for most projects.
- Keep HTML and CSS in separate files.
- Write clean and properly indented code.
- Add comments when necessary.
- Use meaningful selectors and organize your styles logically.

---

# 📚 Quick Revision

## CSS Syntax

```css
selector {
    property: value;
}
```

---

## Three Ways to Add CSS

| Method | Best For |
|---------|----------|
| Inline CSS | Quick testing or one-time styling |
| Internal CSS | Small single-page websites |
| External CSS | ⭐ Multi-page and professional websites |

---

# 📌 CSS Cheat Sheet

| Syntax | Purpose |
|---------|----------|
| `style=""` | Apply Inline CSS |
| `<style>` | Write Internal CSS |
| `<link rel="stylesheet" href="style.css">` | Connect an External CSS file |
| `selector { property: value; }` | Basic CSS rule |
| `/* comment */` | Write a CSS comment |

---

# 🎯 Key Takeaways

- ✅ CSS makes webpages visually attractive.
- ✅ HTML creates the structure, while CSS controls the design.
- ✅ A CSS rule consists of a **selector**, **property**, and **value**.
- ✅ CSS can be added using **Inline**, **Internal**, or **External** methods.
- ✅ **External CSS** is the most recommended approach for building real-world websites.

---

[⬆️ Back to Table of Contents](#-table-of-contents)
