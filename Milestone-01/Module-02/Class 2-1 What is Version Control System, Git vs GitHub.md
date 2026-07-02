# 📚 Programming Hero - Smart Notes

## Class 2-1

# 🚀 What is Version Control System, Git vs GitHub

> **Class Duration:** 12 Minutes

---

# 📑 Table of Contents

* [📖 What You'll Learn](#-what-youll-learn)
* [🤔 Why Do We Need Git?](#-why-do-we-need-git)
* [🗂️ Types of Version Control System (VCS)](#️-types-of-version-control-system-vcs)
* [💻 What is Git?](#-what-is-git)
* [⚙️ How Git Works](#️-how-git-works)
* [☁️ What is GitHub?](#️-what-is-github)
* [🎤 Interview Questions](#-interview-questions)
* [📚 Key Terms](#-key-terms)
* [📝 Quick Revision](#-quick-revision)
* [🎯 Key Takeaways](#-key-takeaways)
* [📖 Summary](#-summary)


---



# 📚 Programming Hero - Smart Notes

## Class 2-1

# 🚀 What is Version Control System, Git vs GitHub

> **Class Duration:** 12 Minutes

---

# 📖 What You'll Learn

In this class, you'll learn:

* Why Git was created
* Problems developers faced before Git
* What a Version Control System (VCS) is
* Why Version Control is important
* Why developers use Git
* The core benefits of Version Control

---

# 🤔 Why Do We Need Git?

Imagine you've been working on a project for several weeks.

Your computer suddenly crashes.

Or your hard drive gets damaged.

Or you accidentally delete your project folder.

Without any backup, you may lose:

* 💻 Source code
* 📄 Important documents
* 📝 Drafts and notes
* 📂 Project files
* 📸 Images and assets

Everything you've worked on could disappear in just a few seconds.

This was one of the biggest challenges developers faced before Version Control Systems became popular.

---

# 🌍 Real-Life Example

Imagine you're writing a university assignment.

You save the file as:

```text
Assignment.docx
```

The next day, you make some changes.

To avoid losing the previous version, you save another copy.

```text
Assignment Final.docx
```

Later, you edit it again.

```text
Assignment Final Final.docx
```

Then again...

```text
Assignment Final Latest.docx
```

After a few days, your folder looks like this:

```text
Assignment.docx

Assignment Final.docx

Assignment Final Final.docx

Assignment Final Latest.docx

Assignment Final Latest Updated.docx
```

Now imagine trying to remember:

* Which one is the newest?
* Which version should you submit?
* Which file contains yesterday's changes?

It quickly becomes confusing.

Git solves this problem by automatically keeping track of every version of your project.

You no longer need to create dozens of duplicate files.

---

# 💡 Why Was Git Created?

Git was created to make project management easier and safer.

Instead of manually creating multiple copies of files, Git automatically tracks every important change.

With Git, developers can:

* Save project history
* Compare different versions
* Restore previous versions
* Collaborate with other developers
* Keep projects backed up safely

Git acts like a **time machine** for your project.

You can always go back to an earlier version whenever needed.

---

# 🌐 Popular Git Platforms

Git itself is a Version Control System.

To store and share Git repositories online, developers use platforms such as:

* GitHub
* GitLab
* Bitbucket

These platforms allow developers to:

* Store projects online
* Collaborate with teams
* Share code with others
* Back up repositories in the cloud

> **Note:** Git and GitHub are **not the same thing**. We'll explore their differences later in this class.

---

# 🎯 Why is Version Control System Needed?

A Version Control System helps developers manage projects efficiently.

The four main reasons are:

## 1️⃣ Collaboration

Multiple developers can work on the same project without overwriting each other's work.

---

## 2️⃣ Version History

Every important change is recorded.

You can easily see:

* Who made the change
* When it was made
* What was changed

---

## 3️⃣ Restore Previous Versions

Made a mistake?

No problem.

Git allows you to return to an earlier version of your project whenever necessary.

---

## 4️⃣ Backup

Even if your computer is damaged or files are accidentally deleted, your project can remain safe when stored in an online repository like GitHub.

---

# 📌 Quick Summary

| Without Git                | With Git                              |
| -------------------------- | ------------------------------------- |
| High risk of losing files  | Project history is safely preserved   |
| Difficult to track changes | Every change is recorded              |
| Collaboration is difficult | Multiple developers can work together |
| Manual backups             | Easy backup using online repositories |
| Confusing file versions    | Organized version history             |

---

# 💡 Pro Tip

Think of **Git as the save history of your project**, not just a backup tool.

Instead of saving dozens of files like:

```text
Project Final

Project Final Final

Project Final Latest

Project Final Latest Updated
```

Git keeps every version organized automatically, making project management much easier.

---

# ⚠️ Common Mistake

Many beginners think:

> **"Git is only for uploading code to GitHub."**

❌ That's not true.

Git's primary purpose is **Version Control**.

Uploading code to GitHub is just one of its many uses.

---




# 🗂️ Types of Version Control System (VCS)

A **Version Control System (VCS)** can be categorized into **three main types**:

1. Local Version Control System (LVCS)
2. Centralized Version Control System (CVCS)
3. Distributed Version Control System (DVCS)

---

# 📊 Visual Overview

> **Image:** `Images/vcs-types.png`

```text
                 Version Control System
                         │
      ┌──────────────────┼──────────────────┐
      │                  │                  │
      ▼                  ▼                  ▼
   Local VCS      Centralized VCS    Distributed VCS
```

---

# 1️⃣ Local Version Control System (LVCS)

A **Local Version Control System** stores all project versions on a **single computer**.

Everything remains inside your local machine.

## 📌 How It Works

```text
        Your Computer
   ┌─────────────────────┐
   │   Project Files      │
   │        ↓             │
   │ Local Version Store  │
   └─────────────────────┘
```

Only one developer usually works on the project.

---

## ✅ Advantages

* Very simple
* Fast
* No internet required

---

## ❌ Disadvantages

* No collaboration
* Easy to lose everything if the computer crashes
* No online backup

---

# 🌍 Real-Life Example

Imagine writing your assignment only on your laptop.

If your laptop suddenly stops working,

👉 all your work could be lost.

---

# 2️⃣ Centralized Version Control System (CVCS)

A **Centralized Version Control System** uses **one central server**.

Every developer connects to that server to access the project.

---

## 📊 How It Works

```text
           Central Server
                │
     ┌──────────┼──────────┐
     │          │          │
 Developer A Developer B Developer C
```

Everyone works using the same central repository.

---

## ✅ Advantages

* Easy collaboration
* One shared project
* Better management

---

## ❌ Disadvantages

If the **central server fails**, everyone is affected.

Without the server, developers may not be able to continue working normally.

---

# 🌍 Real-Life Example

Think of **Google Drive**.

Everyone edits the same file stored in one place.

If the server becomes unavailable,

everyone experiences the problem.

---

# 3️⃣ Distributed Version Control System (DVCS)

A **Distributed Version Control System** gives **every developer a complete copy** of the repository.

This is the system used by **Git**.

---

## 📊 How It Works

```text
        GitHub Repository
               │
      ┌────────┼────────┐
      │        │        │
      ▼        ▼        ▼
 Dev A     Dev B     Dev C

Each developer has a complete
copy of the repository.
```

---

## ✅ Advantages

* Full project history on every computer
* Better collaboration
* Faster operations
* Easy backup
* Can work offline

---

## ❌ Disadvantages

* Takes more storage space
* Slightly more complex for beginners

---

# 🌍 Real-Life Example

Imagine every member of a team has a complete copy of the project.

Even if one computer is damaged,

the project is still safe because everyone has another complete copy.

---

# ⭐ Which Type Does Git Use?

Git is a:

> **Distributed Version Control System (DVCS)**

Every developer has:

* Complete project files
* Complete version history
* Ability to work offline
* Ability to synchronize changes later

This makes Git one of the most powerful Version Control Systems available today.

---

# 📋 Comparison Table

| Feature                 | Local VCS  | Centralized VCS | Distributed VCS (Git) |
| ----------------------- | ---------- | --------------- | --------------------- |
| Stores versions locally | ✅          | ❌               | ✅                     |
| Central server          | ❌          | ✅               | ✅ (for sharing)       |
| Offline work            | ✅          | ❌               | ✅                     |
| Collaboration           | ❌          | ✅               | ✅                     |
| Backup                  | ❌          | Limited         | ✅                     |
| Full project history    | Local only | Server only     | Every developer       |

---

# 💡 Pro Tip

Don't memorize the three types of Version Control Systems.

Instead, understand **how they work**.

Once you understand their workflow, you'll easily remember why **Git uses the Distributed Version Control System (DVCS)**.

---

# ⚠️ Common Mistake

Many beginners think:

> **"GitHub is Git."**

❌ That's incorrect.

Git is the **Distributed Version Control System (DVCS)**.

GitHub is an **online platform** that hosts Git repositories.

We'll explore this difference in detail in the next parts.

---

# 🎤 Interview Question

**Q:** Which type of Version Control System does Git use?

**Answer:**

> Git uses a **Distributed Version Control System (DVCS)**, where every developer has a complete copy of the repository and its entire version history.

---

# 📝 Quick Revision

* Version Control Systems are of **three types**.
* **Local VCS** stores versions only on one computer.
* **Centralized VCS** uses one central server.
* **Distributed VCS** gives every developer a complete copy of the repository.
* **Git** is a **Distributed Version Control System (DVCS)**.



# 💻 What is Git?

Git is the most widely used **Distributed Version Control System (DVCS)** in software development.

It helps developers track changes, manage different versions of a project, and collaborate efficiently with other developers.

Instead of creating multiple copies of the same project, Git keeps a complete history of all changes in an organized way.

---

# 📖 Official Definition

> **Git is a distributed version control system widely used in software development.**

In simple words,

Git is a tool that helps developers:

* Track changes in source code
* Save project history
* Restore previous versions
* Collaborate with multiple developers
* Manage software projects efficiently

---

# ⭐ Key Features of Git

Git provides many powerful features that make software development easier.

## ✅ 1. Version Tracking

Git records every important change made to a project.

This allows developers to review the complete history whenever needed.

---

## ✅ 2. Collaboration

Multiple developers can work on the same project at the same time.

Git helps merge everyone's work without manually combining files.

---

## ✅ 3. Backup & Recovery

Since projects can be stored on platforms like GitHub, your work remains safe even if your computer is damaged.

---

## ✅ 4. Branching

Developers can create separate branches to test new features without affecting the main project.

*(We'll learn Branches in upcoming classes.)*

---

## ✅ 5. Restore Previous Versions

If something goes wrong, Git allows you to return to an earlier version of your project.

This makes experimentation much safer.

---

# 🌍 Real-Life Example

Imagine you're writing a book.

Every day you make some improvements.

Without Git, you might save files like:

```text
Book_v1.docx
Book_v2.docx
Book_Final.docx
Book_Final_Final.docx
```

With Git,

you keep only **one project**, while Git automatically remembers every version behind the scenes.

---

# 🚀 Advantages of Using Git

Using Git offers several important benefits.

* 📌 Tracks every project change
* 📌 Makes collaboration easier
* 📌 Keeps complete project history
* 📌 Allows easy rollback to previous versions
* 📌 Works offline
* 📌 Integrates with platforms like GitHub
* 📌 Widely used in professional software development

---

# 🌐 Git Related Platforms

Git is often used together with online hosting platforms.

Some of the most popular platforms are:

## 🐙 GitHub

The world's most popular platform for hosting Git repositories.

Commonly used for:

* Open Source Projects
* Portfolio
* Team Collaboration
* Code Sharing

---

## 🦊 GitLab

GitLab is another Git hosting platform.

Besides source code hosting, it also provides built-in DevOps and CI/CD features.

---

## 🪣 Bitbucket

Bitbucket is a Git repository hosting service developed by Atlassian.

It integrates well with tools like Jira and is commonly used in enterprise environments.

---

# 📋 Platform Comparison

| Platform  | Best Known For                      |
| --------- | ----------------------------------- |
| GitHub    | Open Source & Community             |
| GitLab    | DevOps & CI/CD                      |
| Bitbucket | Enterprise Teams & Jira Integration |

---

# 💡 Important Note

Git itself is **not** an online platform.

Git is the **tool** that manages your project's version history.

GitHub, GitLab, and Bitbucket are **hosting platforms** where Git repositories can be stored and shared.

Think of it like this:

* **Git = The tool**
* **GitHub = A place to store and share Git projects**

---

# 💡 Pro Tip

When someone asks,

> **"Do you know Git?"**

they usually mean:

* Can you use Git commands?
* Can you manage project versions?
* Can you collaborate using Git?

They are **not** asking whether you simply know how to upload a project to GitHub.

---

# ⚠️ Common Mistake

Many beginners believe:

> **GitHub stores project history.**

Actually,

Git stores the project's history.

GitHub simply hosts Git repositories online.

---

# 🎤 Interview Question

### Q: What is Git?

**Answer:**

Git is a **Distributed Version Control System (DVCS)** that helps developers track changes, manage project versions, and collaborate efficiently on software development projects.

---

### Q: Name some popular Git hosting platforms.

**Answer:**

* GitHub
* GitLab
* Bitbucket

---

# 📝 Quick Revision

* Git is a **Distributed Version Control System**.
* Git tracks every change made to a project.
* Git supports collaboration and version management.
* Git works offline.
* GitHub, GitLab, and Bitbucket are Git hosting platforms.
* Git and GitHub are **not the same thing**.

---

# 🎯 Key Takeaways

✅ Git helps developers manage project versions efficiently.

✅ Git automatically tracks every important change.

✅ Git allows teams to collaborate on the same project.

✅ GitHub, GitLab, and Bitbucket are platforms used to host Git repositories.

✅ Understanding **Git first** makes learning GitHub much easier.




---

# ⚙️ Part 4 — How Git Works

Git is designed to **track changes efficiently**.

Instead of saving the entire project every time you make a change, Git records the **state (snapshot)** of your project at different points in time.

Each snapshot represents how your project looked at the moment you created a commit.

This makes Git fast, reliable, and efficient.

---

# 📸 Git Stores Snapshots, Not File Copies

Many beginners think Git saves a new copy of every file whenever changes are made.

❌ That's not how Git works.

Instead, Git stores a **snapshot** of your project.

Think of it as taking a photograph.

Every time you create a commit:

* Git captures the current state of your project.
* It stores that snapshot.
* It keeps a reference to it.
* Later, you can return to any previous snapshot whenever needed.

---

# 🌍 Real-Life Example

Imagine you're creating a presentation.

After finishing Chapter 1, you save your progress.

After adding Chapter 2, you save again.

After completing the presentation, you save once more.

Instead of keeping files like:

```text
Presentation_v1.pptx

Presentation_v2.pptx

Presentation_Final.pptx

Presentation_Final_Final.pptx
```

Git keeps everything inside a single project while remembering each important version as a snapshot.

You only work on **one project**, while Git manages the history behind the scenes.

---

# 🔄 How Git Works

Whenever you modify your project, Git follows a simple workflow before permanently saving your changes.

The process looks like this:

```text
Working Directory
        │
        ▼
 Staging Area
        │
        ▼
 Git Repository
```

> 📍 **Diagram:** `Images/how-git-works.png`

This is the basic Git workflow you'll use throughout your development journey.

---

# 📂 The Three Areas of Git

A Git project is divided into **three main sections**.

Understanding these three areas is one of the most important Git concepts.

---

## 1️⃣ Working Directory

The **Working Directory** is where you actively work on your project.

It contains all your project files.

Examples:

* Creating new files
* Editing existing files
* Deleting files
* Renaming files

Everything starts here.

Think of it as your workspace.

---

## 🌍 Real-Life Example

Imagine you're writing notes in Microsoft Word.

As long as you're typing,

you're working inside the **Working Directory**.

Nothing has been officially saved into Git yet.

---

## 2️⃣ Staging Area

The **Staging Area** is a temporary place where Git prepares files before creating a commit.

It allows you to choose **which changes should be included** in the next commit.

Not every edited file has to be committed immediately.

You decide what goes into the next snapshot.

Think of it as a **waiting room** before the final save.

---

## 🌍 Real-Life Example

Imagine packing your travel bag.

You don't immediately leave your house after picking up an item.

Instead,

you first place everything into your bag.

Only when everything is ready do you begin your journey.

The Staging Area works in a similar way.

---

## 3️⃣ Git Repository

The **Git Repository** is where Git permanently stores your project's history.

Once you create a commit,

Git saves a snapshot of your project inside the repository.

This repository contains:

* Complete project history
* Previous versions
* Commit information
* Metadata about the project

This is the "database" of your Git project.

---

## 🌍 Real-Life Example

Think of it as a digital library.

Every time you publish a new edition of a book,

the library keeps that edition safely.

You can always revisit older editions whenever necessary.

Git Repository works exactly like that.

---

# 📊 Complete Git Workflow

```text
          Edit Files
               │
               ▼
      Working Directory
               │
        git add
               │
               ▼
        Staging Area
               │
      git commit
               │
               ▼
       Git Repository
```

> 📍 **Diagram:** `Images/how-git-works.png`

This workflow is repeated every time you work with Git.

---

# 💡 Pro Tip

Remember this simple sentence:

> **Edit → Stage → Commit**

Almost every Git workflow follows these three steps.

If you understand this flow, learning future Git commands becomes much easier.

---

# ⚠️ Common Mistake

Many beginners think:

> **Saving a file means Git has saved it.**

❌ Not true.

Saving a file only updates it in your **Working Directory**.

Git doesn't track the change until you:

1. Stage the file.
2. Create a commit.

---

# 🎤 Interview Question

### Q: What are the three areas of a Git project?

**Answer:**

A Git project consists of three main areas:

* Working Directory
* Staging Area
* Git Repository

These three areas form the basic Git workflow.

---

# 📝 Quick Revision

* Git stores **snapshots**, not duplicate copies of files.
* Every commit creates a new snapshot of the project.
* Git workflow has three main stages:

  * Working Directory
  * Staging Area
  * Git Repository
* Files move from the Working Directory → Staging Area → Git Repository.

---

# 🎯 Key Takeaways

✅ Git tracks projects by creating snapshots.

✅ A commit represents a saved snapshot of your project.

✅ Every Git project has three main areas.

✅ Understanding the Git workflow is essential before learning Git commands.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

---




# ☁️ What is GitHub?

GitHub is a **cloud-based platform** that hosts Git repositories online.

It allows developers to store, manage, and share their Git projects over the internet.

While **Git** manages the version history locally, **GitHub** provides a place to publish and collaborate on those Git repositories.

In simple words:

> **GitHub is a platform built around Git.**

---

# 🌍 Real-Life Example

Imagine you're writing a book.

* **Git** is like your notebook that records every edit and revision.
* **GitHub** is like an online library where you publish and share your book with others.

The notebook and the library work together, but they are **not the same thing**.

---

# 📊 GitHub Workflow

A basic GitHub workflow looks like this:

```text
Developer
     │
     ▼
Local Git Repository
     │
 git push
     │
     ▼
GitHub Repository
```

> 📍 **Diagram:** `Images/github-workflow.png`

### Workflow Explanation

1. You write or edit code on your computer.
2. Git tracks your changes locally.
3. You create a commit.
4. You push the commit to GitHub.
5. GitHub stores your repository online.

This allows you to access your project from anywhere and collaborate with others.

---

# 🌟 Why Do Developers Use GitHub?

GitHub offers many useful features beyond simply storing code.

### ✅ Backup

Your project remains safe online even if your computer is damaged.

---

### ✅ Collaboration

Multiple developers can work together on the same repository.

---

### ✅ Portfolio

Developers showcase their projects on GitHub.

Many recruiters and companies check GitHub profiles during hiring.

---

### ✅ Open Source

GitHub makes it easy to contribute to open-source projects around the world.

---

### ✅ Project Sharing

You can easily share your repository with teammates, mentors, or friends.

---

# ⚖️ Git vs GitHub

Although their names sound similar, Git and GitHub are completely different.

| Git                              | GitHub                                |
| -------------------------------- | ------------------------------------- |
| Version Control System           | Cloud-based Hosting Platform          |
| Installed on your computer       | Accessed through the web              |
| Tracks project history           | Stores Git repositories online        |
| Works offline                    | Requires internet for synchronization |
| Developed for version management | Built for collaboration and hosting   |

> 📍 **Diagram:** `Images/git-vs-github.png`

---

# 💡 Easy Way to Remember

Think of it like this:

| Real Life      | Software Development |
| -------------- | -------------------- |
| Microsoft Word | Git                  |
| Google Drive   | GitHub               |

You write your document in Microsoft Word.

You upload and share it using Google Drive.

Similarly,

You manage your project using Git.

You host and share it using GitHub.

---

# 🚀 Git + GitHub Together

Git and GitHub complement each other.

```text
Write Code
     │
     ▼
Git tracks every change
     │
     ▼
Commit changes
     │
     ▼
Push to GitHub
     │
     ▼
Project stored safely online
```

This is the workflow followed by millions of developers every day.

---

# 💡 Pro Tip

A common interview question is:

> **"Can Git work without GitHub?"**

✅ Yes.

Git works completely independently.

You can use Git without ever creating a GitHub account.

GitHub simply adds online storage and collaboration features.

---

# ⚠️ Common Mistake

Many beginners say:

> **"I pushed my project to Git."**

❌ Incorrect.

Projects are pushed to **GitHub** (or another Git hosting platform).

Git only manages the repository on your local machine.

---

# 🎤 Interview Questions

### Q: What is GitHub?

**Answer:**

GitHub is a cloud-based platform that hosts Git repositories online. It allows developers to store, share, collaborate on, and manage Git projects.

---

### Q: What is the difference between Git and GitHub?

**Answer:**

Git is a **Distributed Version Control System (DVCS)** used to track and manage changes in a project.

GitHub is a **cloud-based hosting platform** that stores Git repositories online and enables collaboration.

---

# 📝 Quick Revision

* GitHub is a cloud-based Git hosting platform.
* Git manages version history.
* GitHub stores Git repositories online.
* Git works without GitHub.
* GitHub makes collaboration and project sharing easier.

---

# 🎯 Key Takeaways

✅ Git and GitHub are different tools with different purposes.

✅ Git tracks project history locally.

✅ GitHub hosts Git repositories online.

✅ GitHub enables collaboration, backup, portfolio building, and open-source contributions.

✅ Most professional developers use **Git + GitHub** together.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

---




# 🎤 Interview Questions

Here are some common interview questions based on this class.

### 1. What is Git?

**Answer:**

Git is a **Distributed Version Control System (DVCS)** that helps developers track changes, manage project versions, and collaborate efficiently.

---

### 2. What is Version Control System?

**Answer:**

A Version Control System (VCS) is a tool that records changes made to files over time, allowing developers to track history, restore previous versions, and collaborate on projects.

---

### 3. Why do developers use Git?

**Answer:**

Developers use Git to:

* Track changes
* Collaborate with team members
* Restore previous versions
* Maintain project history
* Keep projects organized

---

### 4. What are the three types of Version Control Systems?

**Answer:**

* Local Version Control System (LVCS)
* Centralized Version Control System (CVCS)
* Distributed Version Control System (DVCS)

---

### 5. Which type of Version Control System is Git?

**Answer:**

Git is a **Distributed Version Control System (DVCS).**

---

### 6. What are the three areas of a Git project?

**Answer:**

* Working Directory
* Staging Area
* Git Repository

---

### 7. What is GitHub?

**Answer:**

GitHub is a cloud-based platform that hosts Git repositories online and enables collaboration, backup, and project sharing.

---

### 8. What is the difference between Git and GitHub?

**Answer:**

Git is a Version Control System.

GitHub is a cloud platform for hosting Git repositories.

---

# 📚 Key Terms

| Term              | Meaning                                |
| ----------------- | -------------------------------------- |
| Version Control   | Tracks and manages file changes        |
| Repository (Repo) | A project managed by Git               |
| Snapshot          | A saved state of a project             |
| Commit            | A saved snapshot in Git                |
| Working Directory | Where you edit project files           |
| Staging Area      | Temporary area before committing       |
| Git Repository    | Stores project history                 |
| Git               | Distributed Version Control System     |
| GitHub            | Online Git repository hosting platform |

---

# 📝 Quick Revision

## Git

* Distributed Version Control System
* Tracks project history
* Works offline
* Creates snapshots
* Supports collaboration

---

## GitHub

* Cloud-based platform
* Hosts Git repositories
* Online backup
* Team collaboration
* Portfolio hosting

---

## Git Workflow

```text
Working Directory
        │
    git add
        │
        ▼
 Staging Area
        │
 git commit
        │
        ▼
 Git Repository
        │
   git push
        │
        ▼
 GitHub
```

---

## Types of Version Control System

```text
Version Control System
        │
 ┌──────┼────────┐
 │      │        │
 ▼      ▼        ▼
Local Centralized Distributed
```

---

# 🎯 Key Takeaways

✅ Git is a **Distributed Version Control System (DVCS).**

✅ Git tracks every important change made to a project.

✅ Git stores project history using **snapshots**, not duplicate file copies.

✅ Every Git project has three main areas:

* Working Directory
* Staging Area
* Git Repository

✅ GitHub is a cloud-based platform used to host Git repositories online.

✅ Git and GitHub are different, but they work together.

✅ Understanding the Git workflow is essential before learning Git commands.

---

# 📖 Summary

In this class, we learned the fundamentals of **Version Control Systems**, why Git was created, and how it helps developers manage projects efficiently.

We explored the three types of Version Control Systems, understood why Git uses the **Distributed Version Control System (DVCS)** model, and learned how Git stores project history using snapshots.

We also discussed the three main areas of a Git project—**Working Directory**, **Staging Area**, and **Git Repository**—and saw how they form the core Git workflow.

Finally, we introduced **GitHub**, understood its role in software development, and compared it with Git to clearly distinguish their purposes.

With these concepts in place, you're now ready to start learning Git commands and using Git in real projects.

---

# 🚀 What's Next?

In the next class, you'll begin working with actual Git commands such as:

* `git init`
* `git status`
* `git add`
* `git commit`

These commands will help you create your first Git repository and start tracking your projects like a professional developer.

---

[⬆️ Back to Table of Contents](#-table-of-contents)


