# 📚 Programming Hero - Smart Notes

## Class 3-8

# 🌑 CSS Box Shadow & Background Image

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [🌑 What is Box Shadow?](#-what-is-box-shadow)
- [📝 Basic Syntax](#-basic-syntax)
- [🌈 Multiple Shadows](#-multiple-shadows)
- [🖼️ Background Image](#️-background-image)
- [🔁 Background Repeat](#-background-repeat)
- [📍 Background Position](#-background-position)
- [📏 Background Size](#-background-size)
- [📌 Background Attachment](#-background-attachment)
- [✨ Background Shorthand](#-background-shorthand)
- [💡 Best Practices](#-best-practices)
- [📚 Quick Revision](#-quick-revision)
- [📌 CSS Cheat Sheet](#-css-cheat-sheet)
- [🌳 CSS Effects Roadmap](#-css-effects-roadmap)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- What is `box-shadow`?
- Box Shadow Syntax
- Shadow Properties
- Multiple Shadows

---

# 🌑 What is Box Shadow?

The `box-shadow` property adds a **shadow effect** around an HTML element.

It makes elements look more modern and gives a sense of **depth**.

> 💡 Box shadows are commonly used for cards, buttons, images, and containers.

---

# 📝 Basic Syntax

```css
box-shadow: 5px 5px 10px gray;
```

### Breakdown

```text
box-shadow: 5px 5px 10px gray;
             │   │    │     │
             │   │    │     └── Color
             │   │    └──────── Blur Radius
             │   └───────────── Vertical Offset
             └───────────────── Horizontal Offset
```

### Meaning

- **Horizontal Offset** → Moves the shadow left or right.
- **Vertical Offset** → Moves the shadow up or down.
- **Blur Radius** → Controls how soft the shadow looks.
- **Color** → Sets the shadow color.

---

# 📝 Example

### CSS

```css
.card {
    box-shadow: 5px 5px 15px gray;
}
```

### 🎨 Output Preview

```text
Without Shadow

┌──────────────┐
│    Card      │
└──────────────┘

────────────────────────

With Shadow

┌──────────────┐▒▒▒
│    Card      │▒▒▒
└──────────────┘▒▒▒
 ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
```

---

# 🌈 Multiple Shadows

You can apply more than one shadow by separating them with commas.

### Example

```css
box-shadow:
    0 0 5px red,
    0 0 15px blue;
```

> 💡 Multiple shadows are useful for creating glowing or layered effects.

---

# 🌳 Box Shadow Roadmap

```text
box-shadow
│
├── Horizontal Offset
├── Vertical Offset
├── Blur Radius
└── Color
```

---

# 🎯 Memory Trick

```text
Left ↔ Right
      │
      ▼
Horizontal

Up ↕ Down
      │
      ▼
Vertical

Softness
      │
      ▼
Blur

Appearance
      │
      ▼
Color
```

---

# ✅ Key Points

- `box-shadow` adds depth and shadow effects to elements.
- A basic box shadow has four main parts:
  - Horizontal Offset
  - Vertical Offset
  - Blur Radius
  - Color
- Multiple shadows can be applied using commas.
- Box shadows are widely used in modern web design to make UI elements stand out.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 🖼️ Background Image

The `background-image` property is used to set an image as the background of an HTML element.

> 💡 Background images are commonly used in banners, hero sections, cards, and webpages.

---

# 📝 Basic Syntax

```css
background-image: url("image.jpg");
```

### Example

```css
body {
    background-image: url("background.jpg");
}
```

---

# 🔁 Background Repeat

By default, a background image repeats if it's smaller than the element.

### Example

```css
background-repeat: no-repeat;
```

### Common Values

| Value | Purpose |
|--------|---------|
| `repeat` | Repeat horizontally and vertically *(default)* |
| `no-repeat` | Show the image only once |
| `repeat-x` | Repeat horizontally |
| `repeat-y` | Repeat vertically |

---

# 📍 Background Position

The `background-position` property controls where the image appears.

### Example

```css
background-position: center;
```

### Common Values

- `left`
- `center`
- `right`
- `top`
- `bottom`

---

# 📏 Background Size

The `background-size` property controls the size of the background image.

### Example

```css
background-size: cover;
```

### Common Values

| Value | Purpose |
|--------|---------|
| `cover` | Fill the entire element |
| `contain` | Fit the whole image inside the element |
| `100% 100%` | Stretch to match the element's width and height |

---

# 📌 Background Attachment

The `background-attachment` property controls whether the background moves while scrolling.

### Example

```css
background-attachment: fixed;
```

### Common Values

- `scroll` *(default)*
- `fixed`

---

# 🎨 Background Preview

```text
Browser Window

██████████████████████
████ Background ██████
█████  Image █████████
██████████████████████
```

> 💡 `background-size: cover` makes the image cover the entire area.

---

# ✨ Background Shorthand

Instead of writing multiple properties separately, you can use the shorthand property.

```css
background: url("bg.jpg") center / cover no-repeat;
```

This combines:

- Background Image
- Background Position
- Background Size
- Background Repeat

---

# 🌳 Background Property Roadmap

```text
background
│
├── Image
├── Repeat
├── Position
├── Size
└── Attachment
```

---

# ✅ Key Points

- `background-image` sets an image as the background.
- `background-repeat` controls image repetition.
- `background-position` changes the image position.
- `background-size` controls how large the image appears.
- `background-attachment` controls scrolling behavior.
- The `background` shorthand combines multiple background properties into one line.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 💡 Best Practices

Follow these tips when using shadows and background images:

- ✅ Use **subtle box shadows** for a clean, modern look.
- ✅ Avoid very dark or oversized shadows.
- ✅ Use high-quality background images.
- ✅ Prefer `background-size: cover` for hero sections.
- ✅ Use `no-repeat` unless repeating is intentional.
- ✅ Ensure text remains readable over background images.

---

# 📚 Quick Revision

## Box Shadow

| Property | Purpose |
|----------|---------|
| Horizontal Offset | Moves shadow left or right |
| Vertical Offset | Moves shadow up or down |
| Blur Radius | Controls shadow softness |
| Color | Sets the shadow color |

---

## Background Properties

| Property | Purpose |
|----------|---------|
| `background-image` | Sets the background image |
| `background-repeat` | Controls image repetition |
| `background-position` | Changes image position |
| `background-size` | Controls image size |
| `background-attachment` | Controls scroll behavior |

---

# 📌 CSS Cheat Sheet

| Syntax | Purpose |
|---------|----------|
| `box-shadow: 5px 5px 10px gray;` | Add a basic shadow |
| `box-shadow: 0 0 10px blue;` | Create a glow effect |
| `background-image: url("bg.jpg");` | Set a background image |
| `background-repeat: no-repeat;` | Prevent image repetition |
| `background-position: center;` | Center the image |
| `background-size: cover;` | Fill the entire element |
| `background-attachment: fixed;` | Keep the background fixed while scrolling |
| `background: url("bg.jpg") center / cover no-repeat;` | Background shorthand |

---

# 🌳 CSS Effects Roadmap

```text
CSS Effects
│
├── Box Shadow
│   ├── Horizontal
│   ├── Vertical
│   ├── Blur
│   └── Color
│
└── Background
    ├── Image
    ├── Repeat
    ├── Position
    ├── Size
    ├── Attachment
    └── Shorthand
```

---

# 🧠 Memory Trick

```text
Box Shadow

Offset
   │
   ▼
Blur
   │
   ▼
Color

────────────────────────

Background

Image
   │
Repeat
   │
Position
   │
Size
   │
Attachment
```

---

# 🎯 Key Takeaways

- ✅ `box-shadow` adds depth and improves the appearance of UI elements.
- ✅ A box shadow consists of **Horizontal Offset**, **Vertical Offset**, **Blur Radius**, and **Color**.
- ✅ `background-image` adds an image behind an element.
- ✅ Use `background-size: cover` to make the image fill the available space.
- ✅ The `background` shorthand lets you combine multiple background properties into a single declaration.
- ✅ Proper use of shadows and backgrounds makes a website look more modern and visually appealing.

---

[⬆️ Back to Table of Contents](#-table-of-contents)
