# 📚 Programming Hero - Smart Notes

## Class 4-5

# 🟦 CSS Grid Fundamentals: Columns, Gap & Basic Layout

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [🚀 What is CSS Grid?](#-what-is-css-grid)
- [🎯 Why Use CSS Grid?](#-why-use-css-grid)
- [⚙️ Enabling CSS Grid](#️-enabling-css-grid)
- [📦 Grid Container & Grid Items](#-grid-container--grid-items)
- [📏 `grid-template-columns`](#-grid-template-columns)
- [🌟 Fraction Unit (`fr`)](#-fraction-unit-fr)
- [📏 Gap](#-gap)
- [💡 Best Practices](#-best-practices)
- [⚖️ Flexbox vs CSS Grid](#️-flexbox-vs-css-grid)
- [📚 CSS Grid Cheat Sheet](#-css-grid-cheat-sheet)
- [🌍 Real-World Examples](#-real-world-examples)
- [🌳 CSS Grid Roadmap](#-css-grid-roadmap)
- [🎯 Mini Practice](#-mini-practice)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- What is CSS Grid?
- Why use CSS Grid?
- Grid Container
- Grid Items
- `display: grid`
- `grid-template-columns`

---

# 🚀 What is CSS Grid?

**CSS Grid** is a modern CSS layout system used to arrange elements into **rows and columns**.

Unlike Flexbox, which mainly works in **one direction (row or column)**, Grid works in **two dimensions (rows and columns together)**.

> 💡 CSS Grid is ideal for building page layouts, galleries, dashboards, and card sections.

---

# 🎯 Why Use CSS Grid?

CSS Grid provides many advantages:

- 📐 Create layouts using both rows and columns.
- 🧩 Organize content in a structured way.
- 📱 Build responsive web layouts.
- ✨ Write cleaner and more maintainable CSS.
- 🚀 Perfect for modern website designs.

---

# ⚙️ Enabling CSS Grid

To use Grid, apply `display: grid` to the **parent element**.

### CSS

```css
.container {
    display: grid;
}
```

Once enabled:

- The **parent** becomes the **Grid Container**.
- All direct children become **Grid Items**.

---

# 📦 Grid Container & Grid Items

```text
Grid Container
│
├── Grid Item
├── Grid Item
├── Grid Item
└── Grid Item
```

### Example

```html
<div class="container">
    <div>Box 1</div>
    <div>Box 2</div>
    <div>Box 3</div>
    <div>Box 4</div>
</div>
```

Here:

- `<div class="container">` → **Grid Container**
- Child `<div>` elements → **Grid Items**

---

# 📏 Creating Columns

The `grid-template-columns` property defines how many columns the Grid will have and how wide each column should be.

### CSS

```css
.container {
    display: grid;
    grid-template-columns: 200px 200px 200px;
}
```

This creates **3 columns**, each **200px** wide.

---

# 🎨 Output Preview

```text
┌────────┬────────┬────────┐
│ Box 1  │ Box 2  │ Box 3  │
├────────┼────────┼────────┤
│ Box 4  │ Box 5  │ Box 6  │
└────────┴────────┴────────┘
```

> 💡 When the first row is full, Grid automatically places the remaining items in the next row.

---

# 🌳 Grid Layout Structure

```text
Grid Container
│
├── Column 1
├── Column 2
└── Column 3

↓

┌──────┬──────┬──────┐
│ Item │ Item │ Item │
├──────┼──────┼──────┤
│ Item │ Item │ Item │
└──────┴──────┴──────┘
```

---

# 🧠 Memory Trick

```text
display: grid

        │
        ▼

Parent
(Grid Container)

        │

Creates

        ▼

Grid Items

        │

Arranged In

        ▼

Rows + Columns
```

---

# ✅ Key Points

- CSS Grid is a **two-dimensional layout system**.
- Apply `display: grid` to create a **Grid Container**.
- Direct child elements become **Grid Items**.
- `grid-template-columns` defines the number and width of columns.
- When one row is full, Grid automatically moves items to the next row.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 📏 `grid-template-columns`

The `grid-template-columns` property defines:

- ✅ How many columns the Grid will have.
- ✅ The width of each column.

---

# 📝 Fixed-Width Columns

You can define columns using fixed units like `px`.

### CSS

```css
.container {
    display: grid;
    grid-template-columns: 200px 200px 200px;
}
```

### 🎨 Output

```text
┌────────┬────────┬────────┐
│ 200px  │ 200px  │ 200px  │
├────────┼────────┼────────┤
│ Item   │ Item   │ Item   │
└────────┴────────┴────────┘
```

> 💡 Every column has the same fixed width.

---

# 🌟 Fraction Unit (`fr`)

The **`fr` (fraction)** unit divides the available space into equal parts.

Instead of specifying widths manually, Grid automatically distributes the remaining space.

### CSS

```css
.container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
}
```

### 🎨 Visual

```text
|────────|────────|────────|
|  1fr   |  1fr   |  1fr   |
|────────|────────|────────|
```

> 💡 Each column gets **one equal share** of the available width.

---

# ⚖️ Different Fraction Values

Columns don't have to be equal.

### CSS

```css
.container {
    display: grid;
    grid-template-columns: 2fr 1fr;
}
```

### 🎨 Visual

```text
|────────────────────|──────────|
|        2fr         |   1fr    |
|────────────────────|──────────|
```

Here:

- First column = **2 parts**
- Second column = **1 part**

The first column is **twice as wide** as the second.

---

# 📏 Gap

The `gap` property creates space **between Grid Items**.

### CSS

```css
.container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 20px;
}
```

### 🎨 Without Gap

```text
┌────┬────┬────┐
│Box1│Box2│Box3│
└────┴────┴────┘
```

---

### 🎨 With Gap

```text
┌────┐    ┌────┐    ┌────┐
│Box1│    │Box2│    │Box3│
└────┘    └────┘    └────┘
```

> 💡 `gap` works for both **rows** and **columns**, making layouts cleaner without using extra margins.

---

# 🌳 Grid Column Roadmap

```text
Grid Columns
│
├── Fixed Width
│   └── 200px
│
├── Fraction Unit
│   ├── 1fr
│   ├── 2fr
│   └── 3fr
│
└── Gap
    └── gap: 20px
```

---

# 🧠 Memory Trick

```text
grid-template-columns

        │

200px
(Fixed Width)

──────────────

1fr
(Equal Share)

──────────────

2fr 1fr
(Bigger + Smaller)

──────────────

gap
(Space Between Boxes)
```

---

# ✅ Key Points

- `grid-template-columns` defines the number and width of columns.
- Fixed units like `px` create fixed-width columns.
- The `fr` unit divides available space proportionally.
- `1fr 1fr 1fr` creates three equal columns.
- `2fr 1fr` gives the first column twice as much space as the second.
- `gap` adds consistent spacing between Grid Items.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 💡 Best Practices

Follow these tips when working with CSS Grid:

- ✅ Use **CSS Grid** for two-dimensional layouts (rows + columns).
- ✅ Use the **`fr` unit** instead of fixed `px` values whenever possible for responsive layouts.
- ✅ Use the `gap` property instead of adding margins between Grid Items.
- ✅ Keep your Grid structure simple and organized.
- ✅ Use meaningful class names for Grid Containers and Grid Items.

---

# ⚖️ Flexbox vs CSS Grid

| Flexbox | CSS Grid |
|----------|----------|
| One-dimensional layout | Two-dimensional layout |
| Works in **Row OR Column** | Works with **Rows AND Columns** |
| Best for components (Navbar, Menu, Buttons) | Best for page layouts, galleries, dashboards |
| Aligns items in one direction | Arranges items into a complete grid |

---

# 📚 CSS Grid Cheat Sheet

| Property | Purpose |
|----------|---------|
| `display: grid` | Enables CSS Grid |
| `grid-template-columns` | Creates columns |
| `1fr` | One equal fraction of available space |
| `2fr 1fr` | First column is twice as wide |
| `gap` | Adds space between Grid Items |

---

# 🌍 Real-World Examples

## 🖼️ Image Gallery

```css
.gallery {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 20px;
}
```

### Visual

```text
🖼️  🖼️  🖼️
🖼️  🖼️  🖼️
```

---

## 🪪 Card Layout

```css
.cards {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 24px;
}
```

### Visual

```text
┌─────┐ ┌─────┐ ┌─────┐
│Card │ │Card │ │Card │
└─────┘ └─────┘ └─────┘
```

---

## 📊 Dashboard Layout

```css
.dashboard {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 20px;
}
```

### Visual

```text
┌──────────────────┬──────────┐
│                  │ Sidebar  │
│   Main Content   │          │
│                  │          │
└──────────────────┴──────────┘
```

---

# 🌳 CSS Grid Roadmap

```text
CSS Grid
│
├── display: grid
│
├── Grid Container
│
├── Grid Items
│
├── Columns
│   ├── 200px
│   ├── 1fr
│   └── 2fr 1fr
│
├── Gap
│
└── Grid Layout
```

---

# 🧠 Memory Trick

```text
CSS Grid

        │

display: grid

        │

Grid Container

        │

Grid Items

        │

Columns

200px
1fr
2fr 1fr

        │

gap

        │

Responsive Layout ✅
```

---

# 🎯 Mini Practice

Try creating the following layouts:

### ✅ Practice 1

Create a **3-column card layout** using:

- `display: grid`
- `grid-template-columns: 1fr 1fr 1fr`
- `gap: 20px`

---

### ✅ Practice 2

Create a **2-column layout** where:

- Main Content → `2fr`
- Sidebar → `1fr`

---

### ✅ Practice 3

Create a simple **photo gallery** with six images arranged in **3 equal columns**.

---

# 🎯 Key Takeaways

- ✅ CSS Grid is designed for **two-dimensional layouts**.
- ✅ `display: grid` turns a parent element into a **Grid Container**.
- ✅ Child elements automatically become **Grid Items**.
- ✅ `grid-template-columns` controls the number and width of columns.
- ✅ The `fr` unit divides available space proportionally.
- ✅ `gap` creates clean spacing between Grid Items.
- ✅ CSS Grid is ideal for building galleries, dashboards, and overall page layouts.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

