# 📚 Programming Hero - Smart Notes

## Class 5-6

# 💼 What I Do Section Introduction & HTML Structure

> **Class Duration:** _(Project Class)_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [🌟 What is the "What I Do" Section](#what-is-the-"what-i-do"-section)
- [🃏 Building Skill Cards & Content Structure](#-building-skill-cards--content-structure)
- [🎨 Styling the Skills Section & Card Layout](#-styling-the-skills-section--card-layout)
- [🚀 Skill Section Best Practices & Professional Card Design](#-skill-section-best-practices--professional-card-design)
- [🎯 Mini Challenge](#-mini-challenge)
- [📚 Class Summary](#-class-summary)

---

# 📖 What You'll Learn

In this class, you'll learn:

- What is the "What I Do" Section?
- Why Every Portfolio Needs It
- Purpose of the Skills Section
- Semantic HTML Structure
- Skills Container
- Preparing the HTML Before CSS

---

# 🌟 What is the "What I Do" Section?

The **What I Do** section introduces your professional skills and expertise.

It answers an important question:

> **"What can you do?"**

While the Hero and About sections introduce **who you are**, this section focuses on **what you are capable of building or working with**.

---

# 🎯 Why is This Section Important?

Visitors often want to know:

- 💻 What technologies you know
- 🛠️ What kind of work you do
- 🚀 What value you can provide
- 📚 What skills you've learned

A clear skills section helps recruiters and clients quickly understand your abilities.

---

# 🌍 Where Does It Appear?

A typical portfolio website follows this order:

```text
Header

↓

Hero Section

↓

About Section

↓

What I Do

↓

Resume

↓

Contact

↓

Footer
```

The **What I Do** section usually comes right after the About section.

---

# 🧩 Main Components

A professional What I Do section contains:

```text
What I Do

│

├── Section Title

├── Description

└── Skills Container
```

These three parts provide both context and technical information.

---

# 🌳 Section Anatomy

```text
What I Do

│

├── Heading

├── Description

└── Skill Cards
```

The heading introduces the section, the description explains it, and the skill cards showcase your expertise.

---

# 🏗️ Semantic HTML Structure

Like the About section, this section should use the semantic `<section>` element.

Example:

```html
<main>

    <section class="skills">

    </section>

</main>
```

Using semantic HTML makes the code:

- Easier to read
- More accessible
- Better for SEO
- Easier to maintain

---

# 🌳 HTML Hierarchy

```text
main

│

└── section

      ├── Heading

      ├── Description

      └── Skills Container
```

Each part has a clear responsibility.

---

# 📦 Skills Container

Instead of placing skill cards directly inside the section, they are grouped inside a dedicated container.

```text
Skills Container

│

├── Skill Card

├── Skill Card

├── Skill Card

└── Skill Card
```

This makes future styling with Flexbox or Grid much easier.

---

# 📝 Section Heading

The heading tells visitors what this section is about.

Example:

```text
What I Do
```

A clear title improves navigation and readability.

---

# 📄 Section Description

The description briefly explains your experience or technical focus.

Example:

```text
I have experience building responsive and modern
websites using HTML, CSS, and JavaScript.
```

A good description should:

- Be short
- Be informative
- Highlight your technical interests

---

# 🧠 Think Before You Code

Before writing HTML, ask yourself:

- Which skills should I showcase?
- How many skill cards do I need?
- What information belongs inside each card?
- How should everything be organized?

Planning first makes the code cleaner and easier to expand.

---

# 🌳 Development Workflow

```text
Understand Design

↓

Identify Components

↓

Write HTML

↓

Group Skill Cards

↓

Apply CSS
```

Always build the structure before styling.

---

# 💡 Developer Tips

✅ Use the `<section>` element.

✅ Write a meaningful heading.

✅ Keep the description concise.

✅ Place all skill cards inside one container.

✅ Think in reusable components.

---

# ⚠️ Common Beginner Mistakes

### ❌ Writing Skills in a Paragraph

Instead of:

```text
HTML, CSS, JavaScript, React...
```

Use separate skill cards.

---

### ❌ Mixing the Description with the Cards

Keep the description separate from the skill container.

---

### ❌ Skipping Semantic HTML

Prefer:

```html
<section>

</section>
```

instead of using only `<div>` elements.

---

### ❌ Styling Before Structuring

Complete the HTML first.

A solid structure makes CSS much easier.

---

# 🎯 Mini Practice

Draw the structure of the section.

```text
What I Do

│

├── Heading

├── Description

└── Skills Container

      ├── Skill Card

      ├── Skill Card

      ├── Skill Card

      └── Skill Card
```

Then create the HTML structure without looking at the video.

---

# ✅ Key Takeaways

- The **What I Do** section showcases your technical skills.
- It usually appears after the About section.
- Use a semantic `<section>` element.
- Group all skill cards inside one parent container.
- Keep the heading and description short and meaningful.
- Build a clean HTML structure before writing CSS.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 📚 Programming Hero - Smart Notes

## Class 5-6

# 🃏 Building Skill Cards & Content Structure

> The **Skill Card** is the core component of the **What I Do** section. Each card highlights one technology or skill in a clean and easy-to-read format.

---

# 📖 What is a Skill Card?

A **Skill Card** is a small UI component that represents one specific skill.

Instead of writing all skills in one paragraph, each skill is presented separately.

This improves:

- 📖 Readability
- 🎨 Visual appearance
- 👀 User experience
- ♻️ Code reusability

---

# 🎯 Purpose of Skill Cards

Each Skill Card helps visitors quickly understand:

- What technology you know
- What it is used for
- Your area of expertise

Visitors can scan the cards within a few seconds.

---

# 🌳 Skill Card Anatomy

Every Skill Card usually contains:

```text
Skill Card

│

├── Icon

├── Skill Title

└── Description
```

Each element has a specific purpose.

---

# 🖼️ Skill Icon

The icon gives a quick visual clue about the technology.

Examples:

```text
🟧 HTML

🔵 CSS

🟨 JavaScript

⚛ React
```

Icons make the section more attractive and easier to scan.

---

# 🏷️ Skill Title

The title contains the name of the technology.

Example:

```text
JavaScript
```

The title should be:

- Short
- Clear
- Easy to recognize

Visitors should immediately know which skill the card represents.

---

# 📄 Skill Description

The description briefly explains the technology or your experience.

Example:

```text
JavaScript is a programming language
used to build interactive web applications.
```

A good description should:

- Be short
- Explain the main purpose
- Avoid unnecessary details

---

# 🌳 Complete Skill Card

```text
🟨

JavaScript

Programming language for building
interactive web applications.
```

This simple structure is used in many modern portfolio websites.

---

# 📑 HTML Structure

A Skill Card usually looks like this:

```html
<div class="skill">

    <img>

    <h4>

    <p>

</div>
```

Each card contains:

- An icon
- A heading
- A paragraph

This makes the component easy to reuse.

---

# 🌳 HTML Hierarchy

```text
Skills Container

│

├── Skill Card

│      ├── Icon

│      ├── Title

│      └── Description

│

├── Skill Card

├── Skill Card

└── Skill Card
```

Notice how every card follows the exact same structure.

---

# ♻️ Reusable Component

Instead of creating different HTML for every skill:

❌

```text
HTML Card

CSS Card

JS Card

React Card
```

Use one reusable structure.

```text
Skill Card

↓

HTML

↓

CSS

↓

JavaScript

↓

React
```

Only the content changes—the HTML stays the same.

---

# 📋 Information Hierarchy

Visitors usually scan a card in this order:

```text
Icon

↓

Title

↓

Description
```

That's why the icon should be placed at the top.

---

# 🌍 Example Skill Cards

```text
🟧 HTML

Structure of web pages.
```

---

```text
🔵 CSS

Styles and layouts for websites.
```

---

```text
🟨 JavaScript

Adds interactivity to web pages.
```

---

```text
⚛ React

Builds reusable user interfaces.
```

All cards follow the same layout.

---

# 🧠 Why Use Cards?

Imagine writing everything like this:

```text
HTML, CSS, JavaScript and React are my skills...
```

Now compare it with:

```text
🟧 HTML

🔵 CSS

🟨 JavaScript

⚛ React
```

Cards are much easier to scan and understand.

---

# 💡 Developer Tips

✅ Keep every card consistent.

✅ Use icons that match the technology.

✅ Write short descriptions.

✅ Use the same HTML structure for every card.

✅ Think of each card as a reusable component.

---

# ⚠️ Common Beginner Mistakes

### ❌ Different Card Structures

Every card should have the same layout.

---

### ❌ Long Descriptions

Skill cards should provide a quick overview—not a full tutorial.

---

### ❌ Missing Icons

Icons improve visual recognition.

Use them whenever appropriate.

---

### ❌ Random Heading Sizes

Keep all skill titles consistent.

---

### ❌ Duplicate HTML

Avoid writing completely different HTML for each technology.

Reuse the same component.

---

# 🎯 Mini Practice

Create four Skill Cards.

Each card should contain:

```text
Icon

↓

Title

↓

Description
```

Then place all four cards inside one **Skills Container**.

---

# 🌟 Beyond the Course

As you continue learning, you can enhance your Skill Cards with:

- 🎨 Hover Effects
- 🌈 Colored Icons
- 📊 Skill Levels
- 🏷️ Category Labels
- ✨ Animations
- 🔗 Links to Projects

These improvements make your portfolio more engaging while keeping the same reusable structure.

---

# ✅ Key Takeaways

- A Skill Card represents one technology or skill.
- Every card consists of an **Icon**, **Title**, and **Description**.
- All cards should follow the same HTML structure.
- Reusable components reduce duplicate code.
- Short descriptions improve readability.
- Consistent card design creates a more professional portfolio.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 📚 Programming Hero - Smart Notes

## Class 5-6

# 🎨 Styling the Skills Section & Card Layout

> A good Skill Card isn't just about its content—it also needs a clean layout, proper spacing, and consistent styling. In this part, we'll transform simple HTML into a modern-looking Skills Section.

---

# 📖 What You'll Learn

In this part, you'll learn:

- Flexbox Layout
- Card Width
- Gap
- Padding
- Background Color
- Border Radius
- Box Shadow
- Reusable CSS Classes

---

# 🎯 Design Goal

Create a clean and professional Skills Section.

Example:

```text
┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────┐

   HTML          CSS        JavaScript       React

└────────────┘ └────────────┘ └────────────┘ └────────────┘
```

Every card should have equal spacing and consistent styling.

---

# 📦 Skills Container

The Skills Container holds all the Skill Cards.

Example:

```text
Skills Container

│

├── Card

├── Card

├── Card

└── Card
```

Instead of styling each card individually, we style the parent container first.

---

# 🌿 Using Flexbox

The Skills Container usually becomes a Flex Container.

Example:

```css
.skills-container{
    display: flex;
}
```

Result:

```text
Card   Card   Card   Card
```

All cards appear in one row.

---

# 🌉 Adding Space Between Cards

Without spacing:

```text
CardCardCardCard
```

Using `gap`:

```css
.skills-container{
    display: flex;
    gap: 24px;
}
```

Result:

```text
Card      Card      Card      Card
```

`gap` creates equal spacing between every card.

---

# 📏 Card Width

Each card should have enough space for:

- Icon
- Title
- Description

Instead of stretching too wide, give the cards a balanced width.

Visual:

```text
┌──────────────┐

Icon

Title

Description

└──────────────┘
```

Balanced cards are easier to read.

---

# 🌿 Padding

Padding creates space **inside** each card.

Example:

```css
.skill{
    padding: 30px;
}
```

Without padding:

```text
┌────────────┐
│IconTitle...│
└────────────┘
```

With padding:

```text
┌──────────────┐

   Icon

   Title

   Description

└──────────────┘
```

The content gets room to breathe.

---

# 🎨 Background Color

Cards usually have a white background.

Example:

```css
.skill{
    background-color: white;
}
```

This helps the cards stand out from the section background.

---

# 🔵 Border Radius

Rounded corners create a softer, modern appearance.

Example:

```css
.skill{
    border-radius: 8px;
}
```

Visual:

Without:

```text
┌────────────┐
│            │
└────────────┘
```

With:

```text
╭────────────╮
│            │
╰────────────╯
```

---

# 🌑 Box Shadow

A subtle shadow gives depth to the card.

Example:

```css
.skill{
    box-shadow: 0px 6px 20px rgba(0,0,0,0.08);
}
```

Benefits:

- Separates cards from the background
- Creates a modern UI
- Makes the design feel more interactive

Use shadows subtly—too much shadow can make the design look heavy.

---

# 🌳 Card Layout

```text
┌────────────────────┐

      Icon

      Title

   Description

└────────────────────┘
```

Every card should follow the same layout for visual consistency.

---

# ♻️ Reusable CSS Classes

Avoid creating separate CSS for each technology.

❌

```css
.html{}

.css{}

.javascript{}
```

Instead:

```css
.skill{}
```

Every card shares the same style.

Only the content changes.

---

# 🌍 Layout Flow

```text
Skills Container

↓

display:flex

↓

gap

↓

Skill Cards

↓

padding

↓

shadow

↓

Professional Layout
```

This step-by-step approach keeps your CSS organized.

---

# 💡 Developer Tips

✅ Use Flexbox for horizontal card layouts.

✅ Use `gap` instead of margins between cards.

✅ Keep all cards the same size.

✅ Apply subtle shadows.

✅ Create reusable CSS classes.

---

# ⚠️ Common Beginner Mistakes

### ❌ Unequal Card Sizes

Different card widths make the layout look messy.

Keep cards visually consistent.

---

### ❌ Too Much Shadow

Heavy shadows can distract users.

Use light, subtle shadows.

---

### ❌ No Padding

Content touching the edges reduces readability.

Always add internal spacing.

---

### ❌ Using Margins Everywhere

Instead of:

```css
margin-right: 30px;
```

Prefer:

```css
gap: 30px;
```

This keeps spacing cleaner and easier to manage.

---

### ❌ Styling Every Card Separately

Use one reusable class for all Skill Cards.

---

# 🎯 Mini Practice

Style four Skill Cards with:

- Background Color
- Padding
- Border Radius
- Box Shadow
- Flexbox
- Gap

Then compare your design with the original project and adjust the spacing until the layout feels balanced.

---

# 🌟 Beyond the Course

As you continue learning CSS, you can improve the Skills Section with:

- ✨ Hover Animations
- 🎭 Card Transitions
- 🌈 Gradient Backgrounds
- 📱 Responsive Flexbox
- 🧩 CSS Grid Layout
- 🎨 Theme Switching (Light/Dark Mode)

These techniques will help you build modern, interactive portfolio websites.

---

# ✅ Key Takeaways

- Use **Flexbox** to arrange Skill Cards in a row.
- Use **gap** for equal spacing between cards.
- Add **padding** to create internal spacing.
- Use **border-radius** for modern rounded corners.
- Apply **box-shadow** subtly to create depth.
- Build reusable CSS classes for cleaner and more maintainable code.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 📚 Programming Hero - Smart Notes

## Class 5-6

# 🚀 Skill Section Best Practices & Professional Card Design

> The **What I Do** section is one of the first places recruiters and clients look to understand your technical expertise. A well-designed Skills Section can make your portfolio look significantly more professional.

---

# 🎯 Goal of the Skills Section

A great Skills Section should answer one simple question:

```text
What technologies do you work with?
```

Visitors should understand your core skills within a few seconds.

---

# 🌳 Complete Skills Section

```text
What I Do

│

├── Section Title

├── Short Description

└── Skills Container

      ├── HTML

      ├── CSS

      ├── JavaScript

      └── React
```

A clear structure makes the section easy to scan.

---

# 👀 Visitor Reading Pattern

Most visitors naturally follow this order:

```text
Section Title

↓

Description

↓

Icon

↓

Skill Name

↓

Description
```

This is why the icon should always appear at the top of the card.

---

# 🎨 Characteristics of a Good Skill Card

Every Skill Card should be:

- Clean
- Simple
- Consistent
- Easy to read
- Visually balanced

A card should communicate one idea only.

---

# 📝 Writing Better Skill Descriptions

Instead of writing long paragraphs:

❌

```text
JavaScript is one of the most popular programming
languages in the world and it is used in many...
```

Write concise descriptions:

✅

```text
Builds interactive and dynamic web applications.
```

Short descriptions improve readability.

---

# 🖼️ Choosing the Right Icons

Good icons should be:

- Easy to recognize
- High quality
- Consistent in style
- Related to the technology

Examples:

```text
🟧 HTML

🔵 CSS

🟨 JavaScript

⚛ React
```

Avoid mixing different icon styles in the same section.

---

# 📏 Maintain Visual Consistency

All cards should have the same:

- Width
- Padding
- Border Radius
- Font Sizes
- Shadow
- Alignment

Example:

```text
┌──────────┐
│          │
└──────────┘

┌──────────┐
│          │
└──────────┘
```

Consistency creates a professional appearance.

---

# 🌟 Personal Branding Through Skills

The Skills Section reflects your technical identity.

Only include technologies that you:

- Have learned
- Can explain
- Have practiced

Avoid adding technologies just because they are popular.

Your portfolio should represent your actual abilities.

---

# 📋 Beginner vs Professional Skills Section

### Beginner

```text
HTML

CSS

JavaScript

React
```

---

### Professional

```text
🟧 HTML

Semantic and accessible webpage structure.

────────────────────────

🔵 CSS

Responsive layouts and modern styling.

────────────────────────

🟨 JavaScript

Interactive web applications.

────────────────────────

⚛ React

Reusable component-based UI development.
```

The second version provides much more value to visitors.

---

# 💡 UI/UX Tips

A good Skills Section should:

✅ Have enough spacing

✅ Use readable typography

✅ Follow a consistent card design

✅ Be easy to scan

✅ Avoid unnecessary decorations

Good UI always prioritizes clarity.

---

# ⚠️ Common Portfolio Mistakes

### ❌ Adding Too Many Skills

Listing every technology you've ever seen can overwhelm visitors.

Focus on your strongest and most relevant skills.

---

### ❌ Using Low-Quality Icons

Blurry or inconsistent icons make the portfolio look less polished.

---

### ❌ Long Card Descriptions

Skill Cards are summaries—not documentation.

Keep descriptions brief.

---

### ❌ Inconsistent Card Heights

Cards with different heights create an uneven layout.

Aim for a uniform appearance.

---

### ❌ Copying Descriptions from the Internet

Write descriptions in your own words whenever possible.

This makes your portfolio feel more authentic.

---

# 🎯 Mini Challenge

Improve your Skills Section by completing these tasks:

- ✍ Rewrite every skill description in one sentence.
- 🎨 Replace low-quality icons with cleaner ones.
- 📏 Make every card the same size.
- 🌿 Check that spacing is equal between all cards.
- 📱 Test the layout on different screen sizes.

---

# 🌱 Beyond This Class

As you continue learning, you can upgrade this section with:

- 📊 Skill Progress Bars
- 🏆 Experience Levels
- ✨ Hover Animations
- 🎭 Flip Cards
- 🌈 Gradient Effects
- 📱 Responsive Grid Layout
- 🔗 Project Links for Each Skill

These enhancements can make your portfolio more interactive while preserving a clean structure.

---

# 📚 Class Summary

In this class, you learned:

- ✅ What the "What I Do" section is
- ✅ How to structure it with semantic HTML
- ✅ How to build reusable Skill Cards
- ✅ How to style cards using Flexbox, padding, shadows, and spacing
- ✅ Best practices for writing skill descriptions
- ✅ How to create a clean and professional Skills Section

---

# 🏁 Final Takeaways

- The **What I Do** section highlights your technical expertise.
- Every Skill Card should contain an **Icon**, **Title**, and **Short Description**.
- Keep the design consistent across all cards.
- Use Flexbox and reusable CSS classes for a clean layout.
- Focus on technologies you genuinely know and can confidently discuss.
- A simple, organized Skills Section creates a stronger impression than a crowded one.

> 💡 **Golden Rule:**  
> **Don't try to showcase every technology—showcase the technologies you understand well and present them clearly. Quality always creates a stronger impression than quantity.**

---

[⬆️ Back to Table of Contents](#-table-of-contents)
