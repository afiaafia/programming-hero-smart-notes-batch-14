# 📚 Programming Hero - Smart Notes

## Class 2-9

# 🌿 [Advanced] Git Branch, Pull Request & Merge

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [🌿 What is a Git Branch?](#-what-is-a-git-branch)
- [🤔 Why Use Branches?](#-why-use-branches)
- [🌱 Create a New Branch](#-create-a-new-branch)
- [🔀 Switch to Another Branch](#-switch-to-another-branch)
- [📋 View All Branches](#-view-all-branches)
- [🔄 What is a Pull Request (PR)?](#-what-is-a-pull-request-pr)
- [🤝 Why Use Pull Requests?](#-why-use-pull-requests)
- [📝 Pull Request Workflow](#-pull-request-workflow)
- [👀 What Happens After Creating a Pull Request?](#-what-happens-after-creating-a-pull-request)
- [🌐 Where is a Pull Request Created?](#-where-is-a-pull-request-created)
- [🔀 What is Merge?](#-what-is-merge)
- [⚠️ What is a Merge Conflict?](#️-what-is-a-merge-conflict)
- [💡 Best Practices](#-best-practices)
- [📚 Quick Revision](#-quick-revision)
- [📌 Command Cheat Sheet](#-command-cheat-sheet)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- What is a Git Branch?
- Why Branches are Used
- Create a New Branch
- Switch Between Branches
- View Available Branches

---

# 🌿 What is a Git Branch?

A **Git Branch** is an independent line of development.

It allows developers to work on new features or fixes **without affecting the main project**.

> 💡 Think of a branch as a copy of your project where you can safely make changes.

---

# 🤔 Why Use Branches?

Branches help developers:

- Develop new features safely.
- Fix bugs without affecting the main branch.
- Experiment with new ideas.
- Work on multiple tasks at the same time.

---

# 🌱 Create a New Branch

Use the following command:

```bash
git branch feature-name
```

Example:

```bash
git branch login-page
```

This creates a new branch named **login-page**.

---

# 🔀 Switch to Another Branch

You can switch to a branch using:

```bash
git checkout feature-name
```

Example:

```bash
git checkout login-page
```

Or, using the modern command:

```bash
git switch login-page
```

Both commands switch your working directory to the selected branch.

---

# 📋 View All Branches

To see all branches in your repository:

```bash
git branch
```

Example Output:

```text
* main
  login-page
```

> The `*` symbol indicates the **current active branch**.

---

# 🌳 Branch Structure

```text
main
 │
 ├────────────► login-page
 │
 └────────────► navbar-update
```

> 📍 **Image:** `Images/git-branch-diagram.png`

---

# 📌 Command Summary

| Command | Purpose |
|---------|----------|
| `git branch feature-name` | Create a new branch |
| `git checkout feature-name` | Switch to a branch |
| `git switch feature-name` | Switch to a branch (modern command) |
| `git branch` | View all branches |

---

# ✅ Key Points

- A branch allows you to work independently.
- The **main** branch usually contains the stable version of the project.
- Create a separate branch for each new feature or bug fix.
- Use `git branch` to view available branches.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 🔄 What is a Pull Request (PR)?

A **Pull Request (PR)** is a GitHub feature that lets you request to merge the changes from one branch into another (usually `main`).

It allows team members to **review, discuss, and approve** code before it becomes part of the main project.

> 💡 A Pull Request is created on **GitHub**, not in your local Git repository.

---

# 🤝 Why Use Pull Requests?

Pull Requests help teams to:

- Review code before merging.
- Find and fix mistakes.
- Discuss improvements.
- Maintain code quality.
- Collaborate efficiently.

---

# 📝 Pull Request Workflow

```text
Create Branch
      │
      ▼
Make Changes
      │
      ▼
git add .
      │
      ▼
git commit -m "message"
      │
      ▼
git push
      │
      ▼
Create Pull Request
```

> 📍 **Image:** `Images/pull-request-workflow.png`

---

# 👀 What Happens After Creating a Pull Request?

After a Pull Request is created:

1. Team members review the code.
2. Suggestions or changes may be requested.
3. Once approved, the Pull Request is ready to be merged.

> 💡 In personal projects, you can review and merge your own Pull Request.

---

# 🌐 Where is a Pull Request Created?

A Pull Request is created directly on **GitHub**.

Typical steps:

1. Push your branch to GitHub.
2. Open the repository.
3. Click **Compare & Pull Request**.
4. Add a title and description.
5. Click **Create Pull Request**.

> 📍 **Image:** `Images/create-pull-request.png`

---

# 📌 Command Summary

| Command | Purpose |
|---------|----------|
| `git push` | Upload your branch to GitHub |

> 💡 Pull Requests themselves are managed through the **GitHub website**, not with a Git command.

---

# ✅ Key Points

- A Pull Request (PR) is used to request merging changes into another branch.
- PRs help teams review and discuss code before merging.
- Pull Requests are created on GitHub after pushing a branch.
- Code is usually reviewed before it is merged into the `main` branch.

---

[⬆️ Back to Table of Contents](#-table-of-contents)

# 🔀 What is Merge?

A **Merge** combines changes from one branch into another.

After a Pull Request is reviewed and approved, the feature branch is usually **merged into the `main` branch**.

> 💡 Merging keeps the main branch updated with the latest approved changes.

---

# 🌐 Merge Workflow

```text
Create Branch
      │
      ▼
Make Changes
      │
      ▼
Commit & Push
      │
      ▼
Create Pull Request
      │
      ▼
Code Review
      │
      ▼
Merge into main
```

> 📍 **Image:** `Images/git-merge-workflow.png`

---

# ⚠️ What is a Merge Conflict?

A **Merge Conflict** occurs when Git cannot automatically combine changes from different branches.

This usually happens when:

- Two developers edit the same part of a file.
- The same file is changed differently in multiple branches.

> 💡 **Note:** Merge conflicts are a normal part of team development. Don't worry if you don't fully understand them yet—they will be covered in later classes.

---

# 💡 Best Practices

- Create a separate branch for each feature or bug fix.
- Avoid making direct changes to the `main` branch.
- Pull the latest changes before starting new work.
- Write meaningful commit messages.
- Review code before merging.

---

# 📚 Quick Revision

### Branch → Pull Request → Merge

```text
Create Branch
      │
      ▼
Make Changes
      │
      ▼
git add .
      │
      ▼
git commit -m "message"
      │
      ▼
git push
      │
      ▼
Create Pull Request
      │
      ▼
Code Review
      │
      ▼
Merge into main
```

---

# 📌 Command Cheat Sheet

| Command | Purpose |
|---------|----------|
| `git branch` | Create or view branches |
| `git checkout <branch>` | Switch to another branch |
| `git switch <branch>` | Switch branches (modern command) |
| `git push` | Upload a branch to GitHub |

> 💡 Pull Requests and Merge are mainly performed through the **GitHub website**.

---

# 🎯 Key Takeaways

- ✅ A branch lets you develop features independently.
- ✅ A Pull Request (PR) is used to request merging changes.
- ✅ Code is reviewed before it is merged.
- ✅ Merge combines approved changes into the `main` branch.
- ✅ Branch → PR → Merge is a common workflow in professional software development.

---

[⬆️ Back to Table of Contents](#-table-of-contents)
