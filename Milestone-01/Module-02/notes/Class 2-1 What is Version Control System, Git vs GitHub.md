# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [🤔 Why Do We Need Git?](#-why-do-we-need-git)
- [📌 What is a Version Control System (VCS)?](#-what-is-a-version-control-system-vcs)
- [🌍 Real-Life Example](#-real-life-example)
- [🗂️ Types of Version Control System](#️-types-of-version-control-system)
- [💻 What is Git?](#-what-is-git)
- [⭐ Why Developers Use Git](#-why-developers-use-git)
- [⚙️ How Git Works](#️-how-git-works)
- [📂 Three Areas of Git](#-three-areas-of-git)
- [🔄 Git Workflow](#-git-workflow)
- [☁️ What is GitHub?](#️-what-is-github)
- [💡 Git vs GitHub](#-git-vs-github)
- [📚 Quick Revision](#-quick-revision)
- [🎯 Key Takeaways](#-key-takeaways)


# 📚 Programming Hero - Smart Notes

## Class 2-1

# 🚀 What is Version Control System, Git vs GitHub

> **Class Duration:** 12 Minutes

---

# 📖 What You'll Learn

- Why Git is needed
- What is Version Control System (VCS)
- Types of VCS
- What is Git
- How Git works
- Git vs GitHub

---

# 🤔 Why Do We Need Git?

As a project grows, managing different versions becomes difficult.

Without Version Control, developers may face problems like:

- 💻 Losing files due to system crashes
- 🗑️ Accidentally deleting important code
- 👥 Difficulty collaborating with teammates
- 📂 No way to restore older versions

To solve these problems, developers use a **Version Control System (VCS)**.

---

# 📌 What is a Version Control System (VCS)?

A **Version Control System (VCS)** is a tool that tracks and manages changes made to a project over time.

It helps developers:

- Track changes
- Restore previous versions
- Collaborate with teams
- Keep projects organized
- Maintain backups

---

# 🌍 Real-Life Example

Without Git:

```text
Project.html
Project_Final.html
Project_Final_v2.html
Project_Final_Latest.html
```

With Git:

```text
Project
    │
    ├── Version 1
    ├── Version 2
    ├── Version 3
    └── Latest Version
```

Git automatically manages every version, so you don't need multiple copies of the same project.

---

# 🗂️ Types of Version Control System

There are **three types** of Version Control Systems.

| Type | Description |
|------|-------------|
| **Local VCS** | Stores versions on one computer only. |
| **Centralized VCS** | Uses one central server for the whole team. |
| **Distributed VCS** | Every developer has a complete copy of the repository. |

> ✅ **Git is a Distributed Version Control System (DVCS).**

---

# 💻 What is Git?

**Git** is a **Distributed Version Control System (DVCS)** used to track changes and manage project versions.

It allows developers to:

- Track project history
- Restore previous versions
- Collaborate with others
- Work offline
- Manage projects efficiently

---

# ⭐ Why Developers Use Git

- 🤝 Team Collaboration
- 📜 Version History
- ⏪ Restore Older Versions
- ☁️ Backup Projects
- ⚡ Fast & Lightweight
- 💻 Works Offline

---

# ✅ Key Points

- Git was created to solve version management problems.
- A VCS records every important change in a project.
- There are three types of VCS.
- Git is a **Distributed Version Control System (DVCS).**

---

[⬆️ Back to Table of Contents](#-table-of-contents)


# ⚙️ How Git Works

Git stores your project's history using **snapshots**.

Instead of creating multiple copies of your project, Git saves the state of your project whenever you create a **commit**.

Think of it like taking a photo of your project at different stages.

---

# 📂 Three Areas of Git

Every Git project has **three main areas**.

## 1️⃣ Working Directory

This is where you create, edit, rename, or delete files.

It's your active workspace.

---

## 2️⃣ Staging Area

The Staging Area is a temporary place where you select the changes you want to include in the next commit.

Only staged files are committed.

---

## 3️⃣ Git Repository

The Git Repository stores:

- Project history
- Commits
- Snapshots
- Metadata

Once you commit, your changes are permanently saved here.

---

# 🔄 Git Workflow

```text
Working Directory
        │
    git add
        ▼
 Staging Area
        │
 git commit
        ▼
 Git Repository
```

> 📍 **Image:** `Images/how-git-works.png`

---

# ☁️ What is GitHub?

**GitHub** is a cloud-based platform used to host Git repositories online.

It allows developers to:

- Store projects online
- Collaborate with teams
- Share code
- Back up repositories

Popular Git hosting platforms include:

- GitHub
- GitLab
- Bitbucket

---

# 💡 Git vs GitHub

| Git | GitHub |
|------|---------|
| Version Control System | Git Hosting Platform |
| Installed locally | Cloud-based |
| Tracks project history | Stores Git repositories online |
| Works offline | Requires internet for syncing |

**Easy to Remember:**

- **Git → Manages your project**
- **GitHub → Stores and shares your project online**

---

# ✅ Key Points

- Git stores **snapshots**, not duplicate files.
- Every Git project has **three areas**.
- GitHub is used to host Git repositories online.
- Git and GitHub are different but work together.

---

[⬆️ Back to Table of Contents](#-table-of-contents)


# 📚 Quick Revision

## 📌 Version Control System (VCS)

A tool that helps developers:

- Track changes
- Restore previous versions
- Collaborate with teams
- Keep project history
- Create backups

---

## 📌 Git

- Distributed Version Control System (DVCS)
- Tracks project history
- Stores project snapshots
- Works offline
- Supports collaboration

---

## 📌 GitHub

- Cloud-based Git hosting platform
- Stores Git repositories online
- Makes collaboration easier
- Provides online backup
- Useful for portfolio and open-source projects

---

# 📊 Git Workflow Summary

```text
Edit Files
    │
    ▼
Working Directory
    │
 git add
    ▼
Staging Area
    │
git commit
    ▼
Git Repository
    │
 git push
    ▼
GitHub
```

> 📍 **Image:** `Images/git-workflow-summary.png`

---

# 🎯 Key Takeaways

- ✅ Git is a **Distributed Version Control System (DVCS)**.
- ✅ A VCS helps track, manage, and restore project versions.
- ✅ Git stores project history using **snapshots**.
- ✅ Every Git project has three main areas:
  - Working Directory
  - Staging Area
  - Git Repository
- ✅ GitHub is a cloud platform for hosting Git repositories.
- ✅ Git manages the project, while GitHub stores and shares it online.

---

[⬆️ Back to Table of Contents](#-table-of-contents)
