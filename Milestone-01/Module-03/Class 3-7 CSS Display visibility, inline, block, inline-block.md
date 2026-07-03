# 📚 Programming Hero - Smart Notes

## Class 3-7

# 🖥️ CSS Display, Visibility, Inline, Block & Inline-block

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [🖥️ What is the `display` Property?](#️-what-is-the-display-property)
- [📦 Block Elements](#-block-elements)
- [📄 Inline Elements](#-inline-elements)
- [📦 Inline-block Elements](#-inline-block-elements)
- [👻 Visibility](#-visibility)
- [🚫 `display: none`](#-display-none)
- [⭐ Visibility vs Display None](#-visibility-vs-display-none)
- [💡 Best Practices](#-best-practices)
- [📚 Quick Revision](#-quick-revision)
- [📌 CSS Cheat Sheet](#-css-cheat-sheet)
- [🌳 CSS Display Roadmap](#-css-display-roadmap)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- What is the `display` property?
- Block Elements
- Features of Block Elements
- Common Block Elements

---

# 🖥️ What is the `display` Property?

The `display` property defines **how an HTML element is displayed** on a webpage.

It controls:

- Whether an element starts on a new line.
- How much space it occupies.
- How it is arranged with other elements.

---

# 📦 Block Elements

A **Block Element** always starts on a **new line** and takes up the **full available width** by default.

### Common Block Elements

- `<div>`
- `<h1>` to `<h6>`
- `<p>`
- `<section>`
- `<article>`

---

# 📝 Example

### HTML

```html
<div>Box 1</div>
<div>Box 2</div>
<div>Box 3</div>
```

### CSS

```css
div {
    display: block;
    border: 2px solid black;
}
```

---

# 🎨 Output Preview

```text
┌────────────────────┐
│       Box 1        │
└────────────────────┘

┌────────────────────┐
│       Box 2        │
└────────────────────┘

┌────────────────────┐
│       Box 3        │
└────────────────────┘
```

Each element starts on a **new line**.

---

# ⭐ Block Element Visual

```text
───────────────
│   Block 1   │
───────────────

───────────────
│   Block 2   │
───────────────

───────────────
│   Block 3   │
───────────────
```

---

# ✨ Features of Block Elements

- ✅ Starts on a new line.
- ✅ Takes the full available width.
- ✅ `width` and `height` work properly.
- ✅ `margin` and `padding` work on all sides.
- ✅ Suitable for creating page layouts.

---

# 📊 Block Element Summary

| Property | Block Element |
|----------|---------------|
| Starts on a new line | ✅ Yes |
| Takes full width | ✅ Yes |
| Width & Height | ✅ Supported |
| Margin & Padding | ✅ Fully Supported |

---

# 🎯 Memory Trick

```text
Block

Element 1
──────────────

Element 2
──────────────

Element 3
──────────────
```

> 💡 Think of block elements as **stacking vertically**, one below another.

---

# ✅ Key Points

- The `display` property controls how elements appear on a webpage.
- Block elements always start on a new line.
- They occupy the full available width by default.
- Width, height, margin, and padding all work correctly on block elements.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 📄 Inline Elements

An **Inline Element** stays on the **same line** as other elements.

It only takes up as much width as its content needs.

### Common Inline Elements

- `<span>`
- `<a>`
- `<strong>`
- `<em>`
- `<b>`

---

# 📝 Example

### HTML

```html
<span>HTML</span>
<span>CSS</span>
<span>JavaScript</span>
```

### CSS

```css
span {
    display: inline;
    border: 2px solid blue;
}
```

### 🎨 Output Preview

```text
┌──────┐ ┌─────┐ ┌────────────┐
│ HTML │ │ CSS │ │ JavaScript │
└──────┘ └─────┘ └────────────┘
```

> 💡 All elements stay on the **same line**.

---

# ✨ Features of Inline Elements

- ✅ Does **not** start on a new line.
- ✅ Takes only the required width.
- ❌ `width` and `height` usually don't work.
- ⚠️ Horizontal margin and padding work, but vertical sizing is limited.

---

# 📦 Inline-block Elements

An **Inline-block Element** combines the features of both **Inline** and **Block** elements.

It stays on the same line **and** supports `width` and `height`.

### CSS

```css
.card {
    display: inline-block;
    width: 120px;
    height: 60px;
}
```

### 🎨 Output Preview

```text
┌─────────┐ ┌─────────┐ ┌─────────┐
│  Box 1  │ │  Box 2  │ │  Box 3  │
└─────────┘ └─────────┘ └─────────┘
```

> 💡 Great for creating cards, buttons, and navigation items.

---

# 👻 Visibility

The `visibility` property controls whether an element is visible or hidden.

### Example

```css
visibility: hidden;
```

When an element is hidden:

- ❌ It is **not visible**.
- ✅ Its space is **still reserved** on the page.

### 🎨 Output Preview

```text
Box 1   [ Empty Space ]   Box 3
```

---

# 🚫 `display: none`

```css
display: none;
```

When an element uses `display: none`:

- ❌ It is removed from the page.
- ❌ It does **not** take up any space.

### 🎨 Output Preview

```text
Box 1   Box 3
```

(Box 2 is completely removed.)

---

# ⭐ Visibility vs Display None

```text
visibility: hidden

┌─────┐     ┌─────┐
│Box1 │     │Box3 │
└─────┘     └─────┘
     ↑
 Space Still Exists

────────────────────────────

display: none

┌─────┐ ┌─────┐
│Box1 │ │Box3 │
└─────┘ └─────┘
     ↑
 Element Removed
```

---

# ✅ Key Points

- Inline elements stay on the same line.
- Inline-block elements stay on the same line and support width & height.
- `visibility: hidden` hides an element but keeps its space.
- `display: none` removes the element completely from the layout.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 💡 Best Practices

When choosing a display type:

- ✅ Use **Block** elements for page sections and layouts.
- ✅ Use **Inline** elements for small pieces of text.
- ✅ Use **Inline-block** when elements should stay on the same line while supporting `width` and `height`.
- ✅ Use `display: none` when an element should be completely removed from the layout.
- ✅ Use `visibility: hidden` when you want to hide an element but preserve its space.

---

# 📚 Quick Revision

## Display Types

| Display | Starts New Line | Width & Height | Takes Full Width |
|----------|:---------------:|:--------------:|:----------------:|
| `block` | ✅ Yes | ✅ Yes | ✅ Yes |
| `inline` | ❌ No | ❌ No | ❌ No |
| `inline-block` | ❌ No | ✅ Yes | ❌ No |

---

## Visibility Comparison

| Property | Visible? | Space Reserved? |
|----------|----------|-----------------|
| `visibility: hidden` | ❌ No | ✅ Yes |
| `display: none` | ❌ No | ❌ No |

---

# 📌 CSS Cheat Sheet

| Syntax | Purpose |
|---------|----------|
| `display: block;` | Display as a block element |
| `display: inline;` | Display as an inline element |
| `display: inline-block;` | Display as an inline-block element |
| `display: none;` | Remove the element from the layout |
| `visibility: hidden;` | Hide the element but keep its space |

---

# 🌳 CSS Display Roadmap

```text
display
│
├── block
│   ├── New line
│   ├── Full width
│   └── Width & Height ✔
│
├── inline
│   ├── Same line
│   ├── Content width
│   └── Width & Height ✘
│
├── inline-block
│   ├── Same line
│   ├── Content width
│   └── Width & Height ✔
│
└── none
    └── Element removed
```

---

# 🧠 Memory Trick

```text
Block
↓

📦
📦
📦

------------------------

Inline

📦 📦 📦

------------------------

Inline-block

🟦 🟦 🟦
(Width & Height work)

------------------------

display: none

❌ Removed

------------------------

visibility: hidden

⬜ Hidden
(Space remains)
```

---

# 🎯 Key Takeaways

- ✅ The `display` property controls how HTML elements appear on a webpage.
- ✅ **Block** elements start on a new line and take the full available width.
- ✅ **Inline** elements stay on the same line and only use the space they need.
- ✅ **Inline-block** combines the benefits of both block and inline elements.
- ✅ `display: none` completely removes an element from the layout.
- ✅ `visibility: hidden` hides an element while keeping its space reserved.

---

[⬆️ Back to Table of Contents](#-table-of-contents)
