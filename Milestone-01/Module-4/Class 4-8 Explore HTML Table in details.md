# 📚 Programming Hero - Smart Notes

## Class 4-8

# 📊 Explore HTML Table in Details

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [📊 What is an HTML Table?](#-what-is-an-html-table)
- [🏗️ Basic Table Structure](#️-basic-table-structure)
- [🧩 Understanding Each Tag](#-understanding-each-tag)
- [🏗️ Advanced Table Structure](#️-advanced-table-structure)
- [📑 `<caption>`](#-caption)
- [↔️ `colspan`](#️-colspan)
- [↕️ `rowspan`](#️-rowspan)
- [🎨 Basic Table Styling](#-basic-table-styling)
- [🌈 Zebra Stripe Table](#-zebra-stripe-table)
- [🌍 Real-World Examples](#-real-world-examples)
- [🌳 HTML Table Roadmap](#-html-table-roadmap)
- [🎯 Mini Practice](#-mini-practice)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- What is an HTML Table?
- Table Structure
- `<table>`
- `<tr>`
- `<th>`
- `<td>`

---

# 📊 What is an HTML Table?

An **HTML Table** is used to display data in a structured format using **rows** and **columns**.

Tables are useful when you want to organize related information in a grid.

> 💡 HTML tables are commonly used for reports, student lists, invoices, schedules, dashboards, attendance sheets, and more.

---

# 🏗️ Basic Table Structure

A simple HTML table consists of four main elements:

- `<table>` → Creates the table.
- `<tr>` → Creates a table row.
- `<th>` → Creates a header cell.
- `<td>` → Creates a data cell.

---

# 📝 Example

```html
<table>
    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>

    <tr>
        <td>Afia</td>
        <td>20</td>
    </tr>

    <tr>
        <td>Rahim</td>
        <td>22</td>
    </tr>
</table>
```

---

# 🌳 HTML Structure

```text
table
│
├── tr
│   ├── th
│   │   └── Name
│   └── th
│       └── Age
│
├── tr
│   ├── td
│   │   └── Afia
│   └── td
│       └── 20
│
└── tr
    ├── td
    │   └── Rahim
    └── td
        └── 22
```

---

# 🖥️ Output Preview

```text
+---------+------+
| Name    | Age  |
+---------+------+
| Afia    | 20   |
+---------+------+
| Rahim   | 22   |
+---------+------+
```

---

# 🧩 Understanding Each Tag

## `<table>`

The `<table>` element is the main container that holds the entire table.

```html
<table>
    ...
</table>
```

---

## `<tr>` (Table Row)

The `<tr>` element creates a new row inside the table.

```html
<tr>
    ...
</tr>
```

Every row is wrapped inside its own `<tr>` tag.

---

## `<th>` (Table Header)

The `<th>` element defines a **header cell**.

```html
<th>Name</th>
```

### Features

- Bold text by default
- Center aligned by default
- Usually placed in the first row

---

## `<td>` (Table Data)

The `<td>` element defines a **data cell**.

```html
<td>Afia</td>
```

It contains the actual information displayed in the table.

---

# ⚖️ `<th>` vs `<td>`

| `<th>` | `<td>` |
|---------|---------|
| Header Cell | Data Cell |
| Usually in the first row | Contains actual data |
| Bold by default | Normal text by default |
| Center aligned by default | Left aligned by default |

---

# 🌳 Table Hierarchy

```text
table
│
├── Row (tr)
│   ├── Header (th)
│   └── Header (th)
│
├── Row (tr)
│   ├── Data (td)
│   └── Data (td)
│
└── Row (tr)
    ├── Data (td)
    └── Data (td)
```

---

# 🧠 Memory Trick

```text
table
   │
   ▼
Rows (tr)
   │
   ▼
Cells
│
├── th → Header
└── td → Data
```

---

# ✅ Key Points

- HTML tables display data using rows and columns.
- `<table>` creates the table.
- `<tr>` creates a row.
- `<th>` creates a header cell.
- `<td>` creates a data cell.
- A table is built by combining multiple rows, each containing header or data cells.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 🏗️ Advanced Table Structure

As tables become larger, HTML provides additional elements to organize them better.

These elements improve both **readability** and **accessibility**.

---

# 📌 `<thead>`

The `<thead>` element groups all **header rows** of a table.

### HTML

```html
<thead>
    <tr>
        <th>Name</th>
        <th>Age</th>
        <th>Country</th>
    </tr>
</thead>
```

### Purpose

- Keeps all table headers together.
- Makes the table structure more organized.
- Improves accessibility for screen readers.

---

# 📌 `<tbody>`

The `<tbody>` element contains the **main data** of the table.

### HTML

```html
<tbody>
    <tr>
        <td>Afia</td>
        <td>20</td>
        <td>Bangladesh</td>
    </tr>

    <tr>
        <td>Rahim</td>
        <td>22</td>
        <td>Bangladesh</td>
    </tr>
</tbody>
```

---

# 📌 `<tfoot>`

The `<tfoot>` element contains the **footer** of a table.

It is commonly used to display:

- Total
- Average
- Summary
- Final Result

### HTML

```html
<tfoot>
    <tr>
        <td colspan="3">Total Students: 2</td>
    </tr>
</tfoot>
```

---

# 🌳 Complete Table Structure

```text
table
│
├── thead
│   └── tr
│       ├── th
│       ├── th
│       └── th
│
├── tbody
│   ├── tr
│   ├── tr
│   └── tr
│
└── tfoot
    └── tr
        └── td
```

---

# 📑 `<caption>`

The `<caption>` element adds a title to the table.

### HTML

```html
<table>
    <caption>
        Student List
    </caption>

    ...
</table>
```

### Output

```text
Student List

+---------+------+
| Name    | Age  |
+---------+------+
| Afia    | 20   |
+---------+------+
```

> 💡 `<caption>` should be the first child inside the `<table>` element.

---

# ↔️ `colspan`

The `colspan` attribute allows a cell to span **multiple columns**.

### HTML

```html
<tr>
    <th colspan="2">Student Information</th>
</tr>
```

### Without `colspan`

```text
+------+------+
| Name | Age  |
+------+------+
```

### With `colspan="2"`

```text
+--------------+
| Student Info |
+------+--------+
| Name | Age    |
+------+--------+
```

---

# ↕️ `rowspan`

The `rowspan` attribute allows a cell to span **multiple rows**.

### HTML

```html
<tr>
    <td rowspan="2">Afia</td>
    <td>Math</td>
</tr>

<tr>
    <td>English</td>
</tr>
```

### Output

```text
+-------+----------+
| Afia  | Math     |
|       +----------+
|       | English  |
+-------+----------+
```

> 💡 The "Afia" cell occupies two rows.

---

# 🌳 Advanced Table Flow

```text
table
│
├── caption
│
├── thead
│
├── tbody
│
├── tfoot
│
├── colspan
│
└── rowspan
```

---

# ✅ Key Points

- `<thead>` groups the header rows.
- `<tbody>` contains the main table data.
- `<tfoot>` stores summary or footer information.
- `<caption>` adds a title to the table.
- `colspan` merges multiple columns into one cell.
- `rowspan` merges multiple rows into one cell.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 💡 Best Practices

Follow these best practices when creating HTML tables:

- ✅ Use tables **only for tabular data**, not for page layouts.
- ✅ Organize large tables using `<thead>`, `<tbody>`, and `<tfoot>`.
- ✅ Add a `<caption>` to describe the table.
- ✅ Use `<th>` for headings and `<td>` for data.
- ✅ Use `colspan` and `rowspan` only when they improve readability.
- ✅ Style tables with CSS instead of using old HTML attributes like `border`.

---

# 🎨 Basic Table Styling

A table becomes much easier to read with a little CSS.

### CSS

```css
table {
    border-collapse: collapse;
    width: 100%;
}

th,
td {
    border: 1px solid gray;
    padding: 10px;
    text-align: left;
}
```

---

# 📌 `border-collapse`

The `border-collapse` property controls how table borders are displayed.

### Without `border-collapse`

```text
+----++----+
| A  || B  |
+----++----+
```

### With `border-collapse: collapse`

```text
+----+----+
| A  | B  |
+----+----+
```

```css
table {
    border-collapse: collapse;
}
```

---

# 📏 `padding`

The `padding` property adds space **inside** table cells.

```css
th,
td {
    padding: 12px;
}
```

### Without Padding

```text
|Name|Age|
```

### With Padding

```text
|  Name  |  Age  |
```

---

# 📝 `text-align`

Controls the alignment of text inside cells.

```css
th,
td {
    text-align: center;
}
```

Available values:

- `left`
- `center`
- `right`

---

# 🌈 Zebra Stripe Table

To improve readability, alternate row colors can be applied.

### CSS

```css
tr:nth-child(even) {
    background-color: #f2f2f2;
}
```

### Visual

```text
Row 1  ⬜

Row 2  🟦

Row 3  ⬜

Row 4  🟦
```

> 💡 This pattern is called **Zebra Striping** and is commonly used in dashboards and reports.

---

# 🌍 Real-World Examples

## 🎓 Student Result Table

```text
+--------+-------+-------+
| Name   | Math  | English |
+--------+-------+--------+
| Afia   | 90    | 95      |
| Rahim  | 85    | 88      |
+--------+-------+--------+
```

---

## 🧾 Invoice Table

```text
+-----------+-----+-------+
| Product   | Qty | Price |
+-----------+-----+-------+
| Laptop    |  1  | $900  |
| Mouse     |  2  | $40   |
+-----------+-----+-------+
```

---

## 📅 Attendance Sheet

```text
+--------+---------+
| Name   | Present |
+--------+---------+
| Afia   | ✔       |
| Rahim  | ✘       |
+--------+---------+
```

---

## 📊 Dashboard Report

```text
+---------+--------+
| Month   | Sales  |
+---------+--------+
| January | 5000   |
| February| 6200   |
+---------+--------+
```

---

# 🌳 HTML Table Roadmap

```text
HTML Table
│
├── table
│
├── tr
│
├── th
│
├── td
│
├── thead
│
├── tbody
│
├── tfoot
│
├── caption
│
├── colspan
│
├── rowspan
│
└── CSS Styling
```

---

# 🧠 Memory Trick

```text
table

↓

Rows (tr)

↓

Header (th)

↓

Data (td)

↓

thead
tbody
tfoot

↓

caption

↓

colspan
rowspan

↓

Beautiful Table ✅
```

---

# 🎯 Mini Practice

### ✅ Practice 1

Create a **Student Information Table** with:

- Name
- Roll
- Class
- GPA

---

### ✅ Practice 2

Add:

- `<caption>`
- `<thead>`
- `<tbody>`
- `<tfoot>`

to the table.

---

### ✅ Practice 3

Style the table using:

- `border-collapse`
- `padding`
- `text-align`
- Zebra Striping (`tr:nth-child(even)`)

---

# 🎯 Key Takeaways

- ✅ HTML tables organize data into rows and columns.
- ✅ Use semantic elements like `<thead>`, `<tbody>`, and `<tfoot>` for better structure.
- ✅ `<caption>` provides a meaningful title for the table.
- ✅ `colspan` merges columns, while `rowspan` merges rows.
- ✅ CSS properties such as `border-collapse`, `padding`, and `text-align` improve readability.
- ✅ Zebra Striping makes large tables easier to scan.

---

[⬆️ Back to Table of Contents](#-table-of-contents)
