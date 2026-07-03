# 📚 Programming Hero - Smart Notes

## Class 3-9

# 🎯 Module 3 Summary & Practice Tasks

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Revise](#-what-youll-revise)
- [🌳 CSS Learning Roadmap](#-css-learning-roadmap)
- [📚 Module 3 Revision](#-module-3-revision)
- [📦 Layout Concepts Revision](#-layout-concepts-revision)
- [🎯 Practice Tasks](#-practice-tasks)
- [🌳 Module 3 Mind Map](#-module-3-mind-map)
- [📌 Module 3 Cheat Sheet](#-module-3-cheat-sheet)
- [📈 Progress Tracker](#-progress-tracker)
- [🎯 Final Key Takeaways](#-final-key-takeaways)

---

# 📖 What You'll Revise

- CSS Types
- CSS Selectors
- CSS Measuring Units
- Font & Text Styling
- Advanced Selectors

---

# 🌳 CSS Learning Roadmap

```text
CSS Basics
│
├── CSS Types
│   ├── Inline
│   ├── Internal
│   └── External
│
├── Selectors
│   ├── Tag
│   ├── Class
│   ├── ID
│   ├── Universal
│   └── Advanced
│
└── Typography
    ├── Units
    │   ├── px
    │   ├── %
    │   ├── em
    │   └── rem
    │
    ├── Font Family
    ├── Font Size
    ├── Font Weight
    └── Text Align
```

> 💡 This roadmap summarizes everything you've learned before moving on to layout-related topics.

---

# 📚 Module 3 Revision

## 🎨 CSS Types

| Type | Description |
|------|-------------|
| Inline CSS | Applied directly inside an HTML element |
| Internal CSS | Written inside the `<style>` tag |
| External CSS | Stored in a separate `.css` file |

---

## 🎯 CSS Selectors

| Selector | Example |
|----------|---------|
| Tag | `h1` |
| Class | `.title` |
| ID | `#header` |
| Universal | `*` |
| Advanced | `div > p`, `:hover` |

---

## 📏 CSS Measuring Units

| Unit | Purpose |
|------|---------|
| `px` | Fixed size |
| `%` | Relative to parent |
| `em` | Relative to parent font size |
| `rem` | Relative to root font size |

---

## 🔤 Font & Text Styling

| Property | Purpose |
|----------|---------|
| `font-family` | Changes the font |
| `font-size` | Changes text size |
| `font-weight` | Changes text thickness |
| `text-align` | Aligns text horizontally |

---

## 🚀 Advanced Selectors

```text
Advanced Selectors
│
├── Child (>)
├── Descendant (space)
├── Grouping (,)
├── :hover
├── :first-child
├── :last-child
├── ::before
└── ::after
```

---

# 🎯 Key Points

- ✅ CSS can be written using **Inline**, **Internal**, or **External** styles.
- ✅ Selectors help target specific HTML elements.
- ✅ `px`, `%`, `em`, and `rem` are the most commonly used CSS units.
- ✅ Typography is controlled using `font-family`, `font-size`, `font-weight`, and `text-align`.
- ✅ Advanced selectors make CSS more powerful and flexible.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 📦 Layout Concepts Revision

After learning the CSS basics, you explored the core concepts used to build webpage layouts.

---

# 📦 CSS Box Model

Every HTML element is treated as a **box**.

The Box Model consists of four layers:

```text
Outside
   │
   ▼
Margin
   │
   ▼
Border
   │
   ▼
Padding
   │
   ▼
Content
```

> 💡 Remember: **Content → Padding → Border → Margin**

---

# 📏 Margin vs Padding

| Margin | Padding |
|---------|----------|
| Space outside the border | Space inside the border |
| Creates distance between elements | Creates space around content |
| Outside the element | Inside the element |

---

# 🖥️ Display Property

The `display` property controls how an element appears on a webpage.

### Display Types

| Display | Starts New Line | Width & Height |
|----------|:---------------:|:--------------:|
| `block` | ✅ Yes | ✅ Yes |
| `inline` | ❌ No | ❌ No |
| `inline-block` | ❌ No | ✅ Yes |

---

# 🎨 Display Visual

```text
Block

📦
📦
📦

------------------------

Inline

📦 📦 📦

------------------------

Inline-block

🟦 🟦 🟦
```

---

# 👻 Visibility vs `display: none`

| Property | Visible? | Space Reserved? |
|----------|----------|-----------------|
| `visibility: hidden` | ❌ No | ✅ Yes |
| `display: none` | ❌ No | ❌ No |

### Visual

```text
visibility: hidden

📦   ⬜   📦
(Space remains)

------------------------

display: none

📦   📦
(Element removed)
```

---

# ✨ CSS Effects

### Box Shadow

Adds depth and shadow to elements.

```css
box-shadow: 5px 5px 10px gray;
```

---

### Background Image

Adds an image behind an element.

```css
background-image: url("bg.jpg");
```

---

# 🌳 CSS Effects Roadmap

```text
CSS Effects
│
├── Box Shadow
│   ├── Horizontal Offset
│   ├── Vertical Offset
│   ├── Blur Radius
│   └── Color
│
└── Background
    ├── Image
    ├── Repeat
    ├── Position
    ├── Size
    └── Attachment
```

---

# 📌 Layout Summary

```text
Layout
│
├── Border
├── Margin
├── Padding
├── Box Model
├── Display
├── Visibility
├── Box Shadow
└── Background Image
```

---

# 🎯 Key Points

- ✅ The **Box Model** is the foundation of CSS layouts.
- ✅ Use **padding** for inner spacing and **margin** for outer spacing.
- ✅ The `display` property controls how elements are arranged.
- ✅ `visibility: hidden` keeps an element's space, while `display: none` removes it completely.
- ✅ Box shadows and background images improve the visual appearance of a webpage.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 🎯 Practice Tasks

Complete the following mini tasks to strengthen your CSS skills.

---

## ✅ Task 1 — Personal Profile Card

Create a profile card that includes:

- Profile image
- Name
- Short bio
- Button
- Rounded corners
- Box shadow

### Practice Topics

- `border-radius`
- `box-shadow`
- `padding`
- `margin`
- `font`

---

## ✅ Task 2 — Hero Section

Create a simple hero section with:

- Background image
- Heading
- Paragraph
- Button

### Practice Topics

- `background-image`
- `background-size`
- `background-position`
- `text-align`

---

## ✅ Task 3 — Styled Article

Design an article section with:

- Heading
- Paragraph
- Highlighted words
- Different font sizes

### Practice Topics

- Selectors
- Typography
- Colors
- Background

---

## ✅ Task 4 — Display Practice

Create three boxes using:

- `display: block`
- `display: inline`
- `display: inline-block`

Observe how each one behaves.

---

# 🌳 Module 3 Mind Map

```text
Module 3
│
├── CSS Basics
│   ├── Inline CSS
│   ├── Internal CSS
│   └── External CSS
│
├── Selectors
│   ├── Tag
│   ├── Class
│   ├── ID
│   ├── Universal
│   └── Advanced
│
├── Typography
│   ├── Units
│   ├── Font
│   └── Text Align
│
├── Box Model
│   ├── Border
│   ├── Margin
│   ├── Padding
│   └── Content
│
├── Display
│   ├── Block
│   ├── Inline
│   ├── Inline-block
│   └── Visibility
│
└── Effects
    ├── Box Shadow
    └── Background Image
```

---

# 📌 Module 3 Cheat Sheet

| Topic | Most Important Property |
|--------|--------------------------|
| CSS Types | `style`, `<style>`, `.css` |
| Selectors | `class`, `id`, `tag` |
| Typography | `font-size`, `font-family` |
| Box Model | `margin`, `padding`, `border` |
| Display | `display` |
| Visibility | `visibility`, `display: none` |
| Effects | `box-shadow`, `background-image` |

---

# 📈 Progress Tracker

```text
☑ CSS Types

☑ CSS Selectors

☑ CSS Units

☑ Font & Typography

☑ Advanced Selectors

☑ Border

☑ Margin

☑ Padding

☑ CSS Box Model

☑ Display

☑ Visibility

☑ Box Shadow

☑ Background Image

🎉 Module 3 Completed!
```

---

# 🎯 Final Key Takeaways

- ✅ You learned how to apply CSS using **Inline**, **Internal**, and **External** styles.
- ✅ You can target elements using different **CSS Selectors**.
- ✅ You understand the **CSS Box Model**, including **Margin**, **Border**, **Padding**, and **Content**.
- ✅ You know how the **Display** property affects element layout.
- ✅ You can enhance UI with **Box Shadow** and **Background Images**.
- ✅ These concepts build the foundation for the next step: **CSS Layout with Flexbox**.

---

[⬆️ Back to Table of Contents](#-table-of-contents)
