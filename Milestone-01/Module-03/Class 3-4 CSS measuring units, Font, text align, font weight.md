# 📚 Programming Hero - Smart Notes

## Class 3-4

# 📏 CSS Measuring Units, Font & Text Styling

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [📏 What are CSS Measuring Units?](#-what-are-css-measuring-units)
- [📐 Common CSS Units](#-common-css-units)
- [🔤 Font Family](#-font-family)
- [📏 Font Size](#-font-size)
- [⚖️ Font Weight](#️-font-weight)
- [📍 Text Align](#-text-align)
- [💡 Best Practices](#-best-practices)
- [📚 Quick Revision](#-quick-revision)
- [📌 CSS Cheat Sheet](#-css-cheat-sheet)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- What are CSS Measuring Units?
- Common CSS Units
- `px`
- `%`
- `em`
- `rem`
- When to Use Different Units

---

# 📏 What are CSS Measuring Units?

CSS Measuring Units are used to define the **size** of HTML elements.

They are commonly used for:

- Font size
- Width
- Height
- Margin
- Padding
- Spacing

> 💡 Different units are suitable for different situations.

---

# 📐 Common CSS Units

## 1️⃣ Pixels (`px`)

`px` (Pixel) is an **absolute unit**.

It always represents a fixed size.

### Example

```css
font-size: 20px;
```

### 🎨 Output Preview

```text
Small Text

Larger Text (20px)
```

> 💡 Best for fixed-size elements.

---

## 2️⃣ Percentage (`%`)

`%` is a **relative unit**.

Its size depends on the parent element.

### Example

```css
width: 80%;
```

> 💡 `80%` means the element takes 80% of its parent's width.

---

## 3️⃣ em

`em` is a relative unit based on the **font size of its parent element**.

### Example

```css
font-size: 2em;
```

If the parent font size is **16px**, then:

```text
2em = 32px
```

> 💡 Changing the parent font size also changes the child element's size.

---

## 4️⃣ rem

`rem` stands for **Root em**.

It is based on the font size of the root (`<html>`) element.

### Example

```css
font-size: 2rem;
```

If the root font size is **16px**, then:

```text
2rem = 32px
```

> 💡 `rem` provides more consistent sizing across the webpage.

---

# 📊 Unit Comparison

| Unit | Type | Common Use |
|------|------|------------|
| `px` | Absolute | Fixed sizes |
| `%` | Relative | Responsive width & height |
| `em` | Relative | Size based on parent |
| `rem` | Relative | Size based on root element |

---

# 📌 Quick Revision

```text
px   → Fixed Size

%    → Relative to Parent

em   → Relative to Parent Font Size

rem  → Relative to Root Font Size
```

---

# ✅ Key Points

- CSS units define the size of elements.
- `px` provides fixed sizing.
- `%` adjusts based on the parent element.
- `em` depends on the parent's font size.
- `rem` depends on the root (`html`) font size and is commonly used in modern websites.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 🔤 Font Family

The `font-family` property is used to set the font style of text.

### Example

```css
h1 {
    font-family: Arial, sans-serif;
}
```

> 💡 If the first font isn't available, the browser uses the next one in the list.

### 🎨 Output Preview

```text
Welcome to Tasty Bites
(Font: Arial)
```

---

# 📏 Font Size

The `font-size` property changes the size of text.

### Example

```css
p {
    font-size: 24px;
}
```

### 🎨 Output Preview

```text
Normal Text

Larger Text (24px)
```

---

# ⚖️ Font Weight

The `font-weight` property controls how thick or bold the text appears.

### Example

```css
h2 {
    font-weight: bold;
}
```

or

```css
h2 {
    font-weight: 700;
}
```

### Common Values

| Value | Appearance |
|--------|------------|
| `100` | Thin |
| `400` | Normal |
| `700` | Bold |
| `900` | Extra Bold |

### 🎨 Output Preview

```text
Thin Text

Normal Text

Bold Text

Extra Bold Text
```

---

# 📍 Text Align

The `text-align` property controls the horizontal alignment of text.

### Example

```css
h1 {
    text-align: center;
}
```

### Common Values

```css
text-align: left;
text-align: center;
text-align: right;
text-align: justify;
```

### 🎨 Output Preview

```text
Left
────────────────────

      Center

                 Right

Justified text stretches evenly across the width.
```

---

# 📌 Summary

| Property | Purpose |
|----------|----------|
| `font-family` | Changes the font style |
| `font-size` | Changes the text size |
| `font-weight` | Makes text thinner or bolder |
| `text-align` | Aligns text horizontally |

---

# ✅ Key Points

- `font-family` sets the text font.
- `font-size` controls text size.
- `font-weight` controls text thickness.
- `text-align` aligns text to the left, center, right, or justifies it.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 💡 Best Practices

Follow these tips to make your text readable and professional:

- ✅ Use readable fonts like **Arial**, **Verdana**, or **sans-serif**.
- ✅ Prefer **`rem`** for scalable font sizes in modern websites.
- ✅ Use **bold** only to highlight important content.
- ✅ Keep text alignment consistent throughout the page.
- ✅ Choose font sizes that are comfortable to read.

---

# 📚 Quick Revision

## Common CSS Units

| Unit | Use |
|------|-----|
| `px` | Fixed size |
| `%` | Relative to parent |
| `em` | Relative to parent font size |
| `rem` | Relative to root (`html`) font size |

---

## Font Properties

| Property | Example |
|----------|---------|
| `font-family` | `Arial, sans-serif` |
| `font-size` | `24px` |
| `font-weight` | `700` or `bold` |
| `text-align` | `center` |

---

# 📌 CSS Cheat Sheet

| Syntax | Purpose |
|---------|----------|
| `font-family: Arial, sans-serif;` | Set the font family |
| `font-size: 20px;` | Set the text size |
| `font-weight: bold;` | Make text bold |
| `font-weight: 700;` | Set bold using a numeric value |
| `text-align: center;` | Center-align text |
| `text-align: justify;` | Justify text |

---

# 🎯 Key Takeaways

- ✅ CSS units control the size of elements and text.
- ✅ `px` is a fixed unit, while `%`, `em`, and `rem` are relative units.
- ✅ `font-family` changes the appearance of text.
- ✅ `font-size` controls how large or small text appears.
- ✅ `font-weight` controls text thickness.
- ✅ `text-align` controls the horizontal alignment of text.
- ✅ `rem` is commonly preferred for responsive and consistent typography.

---

[⬆️ Back to Table of Contents](#-table-of-contents)
