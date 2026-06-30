# 📚 Programming Hero - Smart Notes

## Module 1 — Frontend Basics: HTML

# 📝 Class 1_7: Semantic HTML Tags — `section`, `nav`, `header`, `main`, `aside` & `article`

> **Class Duration:** 14 Minutes

---

## 📌 At a Glance

As your webpages become larger and more complex, simply writing HTML tags is no longer enough.

Professional developers don't just create webpages—they organize them in a meaningful way.

This is where **Semantic HTML** comes in.

Instead of using generic containers everywhere, Semantic HTML provides elements that clearly describe the purpose of different parts of a webpage.

These tags make your code easier to:

- Read
- Understand
- Maintain
- Navigate
- Improve for accessibility and search engines

> [!NOTE]
> Semantic HTML is not about changing how a webpage looks.
>
> It's about giving **meaning** to your HTML structure.

---

# 📖 Learning Objectives

After completing this lesson, you should be able to:

- Understand what Semantic HTML is.
- Explain why semantic tags are important.
- Identify the purpose of common semantic HTML elements.
- Organize webpages using meaningful HTML structure.
- Understand the difference between generic and semantic containers.
- Write cleaner and more professional HTML code.

---

# 🤖 Practice with AI

The instructor encouraged using AI to better understand Semantic HTML.

Example Prompt:

```text
Explain Semantic HTML to me like I'm a complete beginner.

Explain why developers use semantic tags instead of generic tags.

Use simple language and real-life examples.

Finally, compare semantic HTML with non-semantic HTML.
```

---

## 💡 Better Prompt (Recommended)

```text
Act as an experienced frontend developer.

Teach me Semantic HTML step by step.

For every semantic tag:

- Explain its purpose.
- Explain when it should be used.
- Give a real-life example.
- Show a simple HTML example.
- Mention common beginner mistakes.

Finish with a comparison table and a practice exercise.
```

A detailed prompt usually produces explanations that are easier to understand and remember.

---

# 🌍 Why Does Semantic HTML Matter?

Imagine walking into a library where every book has a blank cover.

There are no labels.

No categories.

No titles.

Finding the right book would be frustrating.

Now imagine the same library with clear labels:

```text
📚 Science

📚 History

📚 Programming

📚 Fiction
```

You can immediately understand where everything belongs.

Semantic HTML works in the same way.

Instead of placing everything inside anonymous containers, semantic tags clearly describe the role of each part of the webpage.

This makes the structure easier for both humans and computers to understand.

---

# 💡 A Simple Way to Think About It

Suppose you're organizing your study desk.

Instead of putting everything into one large box, you organize it like this:

```text
📦 Study Desk

├── 📚 Books

├── ✏️ Stationery

├── 💻 Laptop

└── 📄 Notes
```

Everything has its own place.

Semantic HTML follows the same principle.

Every section of a webpage has a specific purpose, and semantic tags help express that purpose clearly.

> [!TIP]
> Good HTML is not only about making a webpage work.
>
> It's also about making the code meaningful, organized, and easy to understand for anyone who reads it.

---

# 🚀 Key Idea

Before learning individual semantic tags, remember this one sentence:

> **Semantic HTML tells us what a part of the webpage means, not just how it is displayed.**

This simple idea is the foundation of writing clean, accessible, and professional HTML.





# 🌟 What is Semantic HTML?

The word **Semantic** means **"having meaning"** or **"describing the purpose of something."**

So,

**Semantic HTML** means using HTML elements that clearly describe the purpose or meaning of the content they contain.

Instead of using generic containers everywhere, semantic tags tell both developers and browsers **what each part of the webpage is meant for**.

---

# 🤔 Why Do We Need Semantic HTML?

Imagine reading a book where every chapter is simply named:

```text
Chapter 1

Chapter 2

Chapter 3

Chapter 4
```

You have no idea what each chapter is about.

Now imagine the same book like this:

```text
📖 Introduction

📖 HTML Basics

📖 CSS Styling

📖 JavaScript

📖 Projects
```

Now it's much easier to understand and navigate.

Semantic HTML works exactly the same way.

It gives meaningful names to different parts of a webpage.

---

# 📦 Non-Semantic vs Semantic Elements

HTML elements can be divided into two categories.

## 🔹 Non-Semantic Elements

These elements **do not describe their purpose**.

The most common examples are:

```html
<div>

<span>
```

When you see:

```html
<div>

</div>
```

You don't know what it contains.

It could be:

- Navigation
- Footer
- Sidebar
- Article
- Image Gallery
- Anything

The tag itself gives no clue.

---

## 🔹 Semantic Elements

Semantic elements **describe the purpose of the content**.

Examples:

```html
<header>

<nav>

<main>

<section>

<article>

<aside>

<footer>
```

Just by reading the tag names, you can already guess their role.

For example:

```html
<header>
```

You immediately know:

> This is the header of the webpage.

Likewise,

```html
<footer>
```

clearly indicates the footer section.

---

# 📊 Semantic vs Non-Semantic

| Non-Semantic | Semantic |
|--------------|----------|
| `<div>` | `<header>` |
| `<div>` | `<nav>` |
| `<div>` | `<main>` |
| `<div>` | `<section>` |
| `<div>` | `<article>` |
| `<div>` | `<aside>` |
| `<div>` | `<footer>` |

> [!NOTE]
> This **doesn't mean `<div>` is bad**.
>
> `<div>` is still one of the most useful HTML elements.
>
> Semantic elements are simply preferred whenever they accurately describe the content's purpose.

---

# 🌍 Real-Life Analogy

Imagine you're packing your luggage for a trip.

### Without Labels

```text
📦 Box

📦 Box

📦 Box

📦 Box
```

Every box looks the same.

To find your clothes, you have to open each one.

---

### With Labels

```text
📦 Clothes

📦 Shoes

📦 Electronics

📦 Documents
```

Now you instantly know what's inside each box.

Semantic HTML does the same thing.

Instead of anonymous containers, every part of the webpage has a meaningful label.

---

# 🎯 Benefits of Semantic HTML

Using semantic HTML makes your code:

### 👨‍💻 Easier for Developers

Developers can understand the page structure quickly.

---

### 🔧 Easier to Maintain

Finding and updating specific sections becomes much simpler.

---

### ♿ Better for Accessibility

Screen readers can understand the structure more accurately, making websites easier to use for people with disabilities.

---

### 🔍 Better for Search Engines (SEO)

Search engines can better understand the content and organization of your webpage.

> [!TIP]
> Semantic HTML doesn't directly make your website rank higher.
>
> However, it helps search engines understand your content more effectively, which is an important part of good SEO.

---

# 🚀 Key Idea

Think of Semantic HTML like giving **proper names** to different rooms in a house.

Instead of saying:

```text
Room 1

Room 2

Room 3
```

You say:

```text
🏠 Kitchen

🛏️ Bedroom

🛋️ Living Room
```

The rooms haven't changed—

only their **meaning** has become clear.

Semantic HTML follows exactly the same idea.

It makes your webpage more meaningful, more organized, and much easier for both humans and computers to understand.



# 🏗️ The Core Semantic Layout

Most modern websites follow a similar high-level structure.

```text
┌────────────────────────────────────┐
│             Header                 │
├────────────────────────────────────┤
│          Navigation Menu           │
├────────────────────────────────────┤
│                                    │
│            Main Content            │
│                                    │
├────────────────────────────────────┤
│             Footer                 │
└────────────────────────────────────┘
```

Instead of using multiple generic `<div>` elements, Semantic HTML provides meaningful tags for each section.

This makes the page easier to understand for developers, browsers, and assistive technologies.

---

# 🏠 `<header>` — The Introduction of a Webpage

The `<header>` element represents the introductory section of a webpage or a section.

It usually contains:

- Website logo
- Website title
- Navigation menu
- Search box
- Login/Register button

Example:

```html
<header>

    <h1>Programming Hero Notes</h1>

</header>
```

### 🌍 Real-Life Example

Think of entering a school.

The first thing you usually notice is:

- School name
- School logo
- Reception

The `<header>` plays a similar role—it introduces the webpage.

> [!TIP]
> A webpage usually has one main header, but individual sections or articles can also have their own headers.

---

# 🧭 `<nav>` — Navigation Menu

The `<nav>` element contains links that help users move around a website.

Typical navigation items include:

- Home
- About
- Courses
- Blog
- Contact

Example:

```html
<nav>

    <a href="#">Home</a>

    <a href="#">About</a>

    <a href="#">Contact</a>

</nav>
```

### 🌍 Real-Life Example

Imagine visiting a shopping mall.

At the entrance, there's usually a directory board showing where different stores are located.

The `<nav>` element works in the same way.

It helps visitors find different parts of the website.

---

# 📄 `<main>` — The Main Content

The `<main>` element contains the **primary content** of the webpage.

This is the part users come to read, watch, or interact with.

It may include:

- Articles
- Tutorials
- Products
- Images
- Videos
- Forms

Example:

```html
<main>

    <h2>Learn HTML</h2>

    <p>Welcome to today's lesson.</p>

</main>
```

> [!NOTE]
> Every webpage should have only **one** `<main>` element because it represents the central content of that page.

---

# 🦶 `<footer>` — The Ending Section

The `<footer>` element appears at the bottom of a webpage or a section.

It commonly contains:

- Copyright notice
- Contact information
- Social media links
- Privacy Policy
- Terms & Conditions

Example:

```html
<footer>

    <p>© 2026 Programming Hero Notes</p>

</footer>
```

### 🌍 Real-Life Example

Think of the final page of a book.

It often includes:

- Publisher information
- Copyright details
- Contact information

The `<footer>` serves a similar purpose on a webpage.

---

# 🧩 How These Elements Work Together

A simple semantic webpage structure looks like this:

```html
<body>

    <header>

    </header>

    <nav>

    </nav>

    <main>

    </main>

    <footer>

    </footer>

</body>
```

Each element has a clear responsibility.

This makes the HTML document easier to read and maintain.

---

# 📊 Quick Comparison

| Element | Purpose |
|----------|---------|
| `<header>` | Introduces the webpage or section |
| `<nav>` | Contains navigation links |
| `<main>` | Holds the primary page content |
| `<footer>` | Displays ending information and additional links |

---

# 🚀 Key Idea

Think of these four elements as the basic structure of a book.

```text
📖 Book

↓

Cover

↓

Table of Contents

↓

Chapters

↓

Back Cover
```

Now compare it with a webpage.

```text
🌐 Webpage

↓

Header

↓

Navigation

↓

Main Content

↓

Footer
```

Just as every part of a book has a specific purpose, each semantic HTML element also has its own meaningful role.

Using these tags makes your HTML cleaner, more organized, and much easier to understand.




# 📚 Understanding `<section>` and `<article>`

Although `<section>` and `<article>` may look similar, they are designed for different purposes.

The easiest way to remember them is:

> **A Section groups related content.**
>
> **An Article is a complete, self-contained piece of content.**

Let's understand them one by one.

---

# 📂 `<section>` — Grouping Related Content

The `<section>` element is used to group related content together under a common topic.

Think of it as dividing a webpage into meaningful sections.

Example:

```text
Programming Hero

│

├── HTML

├── CSS

├── JavaScript

└── React
```

Each topic represents a different section of the webpage.

---

## Example

```html
<section>

    <h2>HTML Basics</h2>

    <p>Learn the fundamentals of HTML.</p>

</section>
```

Here,

the entire **HTML Basics** topic is one section.

---

## 🌍 Real-Life Analogy

Imagine reading a textbook.

```text
📖 Web Development Book

│

├── Chapter 1 → HTML

├── Chapter 2 → CSS

├── Chapter 3 → JavaScript
```

Each chapter discusses a different topic.

Similarly,

each `<section>` groups content related to one subject.

---

# 📰 `<article>` — Independent Content

The `<article>` element represents content that can stand on its own.

An article should still make sense even if it is copied and placed somewhere else.

Examples include:

- Blog posts
- News articles
- Forum posts
- Product reviews
- User comments

---

## Example

```html
<article>

    <h2>How to Learn HTML</h2>

    <p>HTML is the foundation of web development...</p>

</article>
```

Even if this article is removed from the webpage and published somewhere else, it still makes sense.

That's why it's called a **self-contained** piece of content.

---

# 🌍 Real-Life Analogy

Think of a newspaper.

```text
📰 Newspaper

│

├── Sports News

├── Technology News

├── Business News
```

Each news story can be read independently.

You don't need the entire newspaper to understand one article.

The `<article>` element works exactly the same way.

---

# 🔍 Section vs Article

This is one of the most common interview questions for beginners.

| `<section>` | `<article>` |
|--------------|-------------|
| Groups related content | Represents independent content |
| Usually focuses on one topic | Can stand alone by itself |
| Often contains multiple elements | Often contains a complete story or post |
| Similar to a chapter | Similar to a complete article |

---

# 🧩 Can an Article Be Inside a Section?

Yes!

This is actually very common.

Example:

```text
Programming Blog

│

└── HTML Tutorials (Section)

      │

      ├── Article 1

      ├── Article 2

      └── Article 3
```

Here,

the **HTML Tutorials** section groups multiple related articles together.

---

## HTML Example

```html
<section>

    <h2>Latest Articles</h2>

    <article>

        <h3>Introduction to HTML</h3>

    </article>

    <article>

        <h3>Understanding Semantic HTML</h3>

    </article>

</section>
```

This is a very common structure in modern websites.

---

# 💡 When Should You Use Which?

Ask yourself this simple question.

### 👉 Is this content part of a larger topic?

Use:

```html
<section>
```

---

### 👉 Can this content be shared or published independently?

Use:

```html
<article>
```

This simple rule works in most situations.

---

# 🎯 Key Idea

Remember this relationship:

```text
📖 Book

↓

Chapter

↓

Story
```

Now compare it to HTML.

```text
🌐 Webpage

↓

Section

↓

Article
```

A **section** organizes related content.

An **article** represents one complete piece of content.

Understanding this difference will help you write cleaner, more meaningful HTML.




# 📌 Understanding the `<aside>` Element

The `<aside>` element is used for content that is **related to the main content**, but is **not part of the primary topic**.

In other words,

the webpage can still be understood even if the aside content is removed.

Think of it as **supporting information**, not the main content.

---

# 🎯 What Can Be Inside an Aside?

Common examples include:

- 📢 Advertisements
- 📝 Author Information
- 🔗 Related Articles
- 📚 Recommended Resources
- 📈 Popular Posts
- 🏷️ Categories
- 📌 Quick Tips
- 📅 Upcoming Events

These elements support the reader but are not the primary focus of the page.

---

# 🌍 Real-Life Analogy

Imagine you're reading a textbook.

The main lesson is printed in the center of the page.

Sometimes you'll also notice a small side box like this:

```text
────────────────────────────

💡 Did You Know?

HTML was first introduced in 1993.

────────────────────────────
```

This information is interesting and helpful,

but it's not required to understand the main lesson.

That side box is similar to an **`<aside>`**.

---

# 🖥️ Where Does `<aside>` Usually Appear?

A common webpage layout looks like this:

```text
┌────────────────────────────────────────────┐
│                  Header                    │
├────────────────────────────────────────────┤
│                  Navigation                │
├───────────────────────┬────────────────────┤
│                       │                    │
│      Main Content     │       Aside        │
│                       │                    │
├───────────────────────┴────────────────────┤
│                  Footer                    │
└────────────────────────────────────────────┘
```

The **main content** appears on one side,

while the **aside** provides additional information.

---

# 💻 HTML Example

```html
<main>

    <article>

        <h2>Learning Semantic HTML</h2>

        <p>Semantic HTML makes webpages more meaningful.</p>

    </article>

    <aside>

        <h3>Related Resources</h3>

        <ul>

            <li>HTML Basics</li>

            <li>Accessibility Guide</li>

        </ul>

    </aside>

</main>
```

Here,

the article contains the primary lesson,

while the aside provides extra learning resources.

---

# 🌐 Real Website Examples

You'll find `<aside>` on many websites.

Examples:

### 📰 News Websites

```text
Main News

──────────────

Related News

Trending Topics

Advertisements
```

---

### 🛍️ E-commerce Websites

```text
Product Details

──────────────

Similar Products

Special Offers

Recently Viewed
```

---

### 📚 Blog Websites

```text
Blog Article

──────────────

Author Profile

Categories

Popular Posts

Newsletter
```

In all of these cases,

the aside enhances the page without replacing the main content.

---

# 🧩 Complete Semantic Page Structure

Now let's combine everything you've learned so far.

```text
HTML Document

│

└── Body

     │

     ├── Header

     │

     ├── Navigation

     │

     ├── Main

     │      │

     │      ├── Section

     │      │      │

     │      │      ├── Article

     │      │      └── Article

     │      │

     │      └── Aside

     │

     └── Footer
```

This is a common structure used in modern websites.

Not every website will include every element,

but this layout is a great foundation for beginners.

---

# 📊 Semantic HTML Overview

| Element | Primary Purpose |
|----------|-----------------|
| `<header>` | Introduces the page or section |
| `<nav>` | Contains navigation links |
| `<main>` | Holds the primary content |
| `<section>` | Groups related content |
| `<article>` | Represents self-contained content |
| `<aside>` | Displays related or supporting content |
| `<footer>` | Contains ending information |

---

# 🚀 Key Idea

Think of a classroom.

```text
👨‍🏫 Teacher's Lesson

↓

Main Topic

↓

💡 Extra Tips

📖 Reference Books

📝 Homework Reminder
```

The lesson is the most important part.

The extra tips and references help students learn more,

but the lesson still makes sense without them.

That's exactly how the `<aside>` element works.

It provides valuable supporting information without becoming the main focus of the webpage.




# 💻 Building a Complete Semantic HTML Page

Now that you've learned the purpose of each semantic element, it's time to see how they work together in a real webpage.

A typical semantic HTML document looks like this:

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Semantic HTML Example</title>
</head>

<body>

    <header>
        <h1>Programming Hero Notes</h1>
    </header>

    <nav>
        <a href="#">Home</a>
        <a href="#">Modules</a>
        <a href="#">Projects</a>
        <a href="#">Contact</a>
    </nav>

    <main>

        <section>

            <h2>Latest Tutorials</h2>

            <article>
                <h3>Introduction to HTML</h3>
                <p>HTML is the foundation of every webpage.</p>
            </article>

            <article>
                <h3>Semantic HTML</h3>
                <p>Semantic tags make HTML more meaningful.</p>
            </article>

        </section>

        <aside>

            <h3>Related Resources</h3>

            <ul>
                <li>HTML Basics</li>
                <li>CSS Roadmap</li>
                <li>Practice Tasks</li>
            </ul>

        </aside>

    </main>

    <footer>
        <p>© 2026 Programming Hero Smart Notes</p>
    </footer>

</body>

</html>
```

---

# 🌳 Visualizing the Structure

Instead of looking at the code line by line, imagine it as a tree.

```text
HTML

│

├── Head

│     ├── Meta

│     ├── Meta

│     └── Title

│

└── Body

      ├── Header

      ├── Navigation

      ├── Main

      │      │

      │      ├── Section

      │      │      ├── Article

      │      │      └── Article

      │      │

      │      └── Aside

      │

      └── Footer
```

This tree view makes it much easier to understand how HTML elements are nested inside one another.

---

# 🧩 How the Elements Work Together

Think of each semantic element as a member of a team.

| Element | Responsibility |
|----------|----------------|
| `<header>` | Introduces the website |
| `<nav>` | Helps users navigate |
| `<main>` | Contains the primary content |
| `<section>` | Groups related information |
| `<article>` | Holds an independent piece of content |
| `<aside>` | Provides supporting information |
| `<footer>` | Ends the webpage with additional details |

Each element has a specific role.

Together, they create a well-organized webpage.

---

# 🌍 Real-Life Analogy

Imagine a university campus.

```text
🎓 University

│

├── Main Gate (Header)

├── Campus Map (Navigation)

├── Academic Building (Main)

│      ├── Department (Section)

│      │      ├── Classroom 1 (Article)

│      │      └── Classroom 2 (Article)

│      │

│      └── Notice Board (Aside)

└── Exit & Information Desk (Footer)
```

Every building has its own purpose.

The campus feels organized because everything is placed where it belongs.

Semantic HTML follows the same principle.

---

# ✅ Best Practices

When writing Semantic HTML:

- Use semantic elements whenever they accurately describe the content.
- Keep your HTML structure simple and logical.
- Avoid replacing every semantic tag with `<div>`.
- Write meaningful headings inside sections and articles.
- Keep related content grouped together.

Clean HTML is easier to read, debug, and maintain.

---

# ⚠️ Common Beginner Mistakes

### ❌ Using Only `<div>` Elements

```html
<div>
    <div>
        <div>
            <div>
```

Although this works, it's difficult to understand the page structure.

---

### ✅ Using Semantic Elements

```html
<header>

<nav>

<main>

<section>

<article>

<aside>

<footer>
```

The purpose of each section becomes immediately clear.

---

### ❌ Creating Too Many Sections

Don't create a new `<section>` for every small paragraph.

A section should group content around a meaningful topic.

---

### ❌ Using `<article>` for Everything

Remember:

An article should make sense on its own.

If the content cannot stand independently, another element may be more appropriate.

---

# 💡 Pro Developer Tip

Ask yourself this question while writing HTML:

> **"If another developer opens my code for the first time, can they understand the page structure without asking me?"**

If the answer is **yes**, you're probably using Semantic HTML correctly.

Professional developers write code not only for browsers—but also for other humans.

---

# 🚀 Key Idea

Semantic HTML is about communication.

It communicates the purpose of your content to:

- 👨‍💻 Developers
- 🌐 Browsers
- ♿ Screen Readers
- 🔍 Search Engines

The clearer your structure is, the easier your webpage is to understand, maintain, and improve.



# 📝 Quick Revision

Let's quickly review everything you've learned in this lesson.

---

## 🌟 What is Semantic HTML?

Semantic HTML uses elements that **describe the purpose or meaning of the content** they contain.

Instead of writing generic containers everywhere, semantic tags make the structure of a webpage clear and meaningful.

---

## 📊 Semantic Elements Overview

| Element | Purpose | Real-Life Example |
|----------|---------|-------------------|
| `<header>` | Introduces the webpage or a section | Book Cover |
| `<nav>` | Contains navigation links | Table of Contents / Road Map |
| `<main>` | Holds the primary content | Main Chapters |
| `<section>` | Groups related content | Chapter |
| `<article>` | Represents self-contained content | Newspaper Article |
| `<aside>` | Displays supporting information | Side Note / Reference Box |
| `<footer>` | Contains ending information | Back Cover |

---

# 🧩 The Relationship Between Semantic Elements

A typical webpage structure looks like this:

```text
Body

│

├── Header

├── Navigation

├── Main

│      │

│      ├── Section

│      │      ├── Article

│      │      └── Article

│      │

│      └── Aside

└── Footer
```

Not every website uses every element,

but this is one of the most common semantic layouts.

---

# ⚖️ Non-Semantic vs Semantic

| Non-Semantic | Semantic |
|--------------|----------|
| `<div>` | `<header>` |
| `<div>` | `<nav>` |
| `<div>` | `<main>` |
| `<div>` | `<section>` |
| `<div>` | `<article>` |
| `<div>` | `<aside>` |
| `<div>` | `<footer>` |

> [!IMPORTANT]
> **`<div>` is not wrong.**
>
> Use semantic elements whenever they accurately describe the content.
>
> Use `<div>` when no semantic element fits your layout or styling needs.

---

# ⚠️ Common Beginner Mistakes

### ❌ Using `<article>` for Every Content Block

Remember:

An article should be able to stand on its own.

---

### ❌ Creating Too Many `<section>` Elements

Every paragraph does **not** need its own section.

A section should group related content around a meaningful topic.

---

### ❌ Forgetting the Purpose of `<aside>`

`<aside>` is for **supporting content**, not the main lesson.

---

### ❌ Ignoring Semantic Tags

Using only `<div>` everywhere makes the HTML harder to understand.

Choose meaningful elements whenever possible.

---

# ✅ Best Practices

Professional developers usually follow these habits:

- Use semantic tags whenever they match the content.
- Keep the HTML hierarchy clean and logical.
- Write meaningful headings inside sections.
- Group related content together.
- Avoid unnecessary nesting.
- Write HTML for both humans and browsers.

---

# 💡 Memory Trick

Imagine building a newspaper website.

```text
📰 Newspaper Website

↓

🏷️ Header

↓

🧭 Navigation

↓

📰 Main News

↓

📂 Sections

↓

📝 Articles

↓

💡 Related Posts

↓

📞 Footer
```

If you can imagine this flow,

you'll remember most semantic HTML elements naturally.

---

# 🎯 Key Takeaways

After completing this lesson, you should understand that:

- Semantic HTML gives meaning to your webpage structure.
- Semantic elements improve readability and organization.
- They also support accessibility and help search engines better understand your content.
- `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, and `<footer>` each have a specific responsibility.
- A well-structured webpage is easier to build, maintain, and collaborate on.

---

# 🌱 Looking Ahead

You've now learned how to create a meaningful HTML page structure.

In the upcoming lessons, you'll continue exploring more HTML elements and gradually build complete webpages using these semantic foundations.

Everything you learn in CSS, Flexbox, Grid, Responsive Design, and JavaScript will build upon this structure.

---

# 📄 Document Information

| Field | Value |
|-------|-------|
| **Module** | 1 — Frontend Basics: HTML |
| **Class** | 1_7 |
| **Document Version** | v1.0 |
| **Status** | ✅ Completed |
| **Last Updated** | 30 June 2026 |
