# 📚 Programming Hero - Smart Notes

## Class 2-3

# 🚀 Introduction to Basic Git Commands: `git init`, `git add`, `git commit`

> **Class Duration:** 12 Minutes

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [🚀 What is `git init`?](#-what-is-git-init)
- [📂 What Happens After `git init`?](#-what-happens-after-git-init)
- [📁 What is the `.git` Folder?](#-what-is-the-git-folder)
- [🔍 Check Repository Status](#-check-repository-status)
- [➕ What is `git add`?](#-what-is-git-add)
- [📂 Add a Specific File](#-add-a-specific-file)
- [📁 Add All Files](#-add-all-files)
- [⚖️ `git add <file>` vs `git add .`](#️-git-add-file-vs-git-add-)
- [🔄 Git Staging Workflow](#-git-staging-workflow)
- [💾 What is `git commit`?](#-what-is-git-commit)
- [🚀 Create Your First Commit](#-create-your-first-commit)
- [📝 Good Commit Message Examples](#-good-commit-message-examples)
- [🔄 Complete Git Workflow](#-complete-git-workflow)
- [📌 Command Summary](#-command-summary)
- [📚 Quick Revision](#-quick-revision)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- What is `git init`
- What is a Git Repository
- Initialize a Local Repository
- What is `.git` Folder
- Check Repository Status using `git status`

---

# 🚀 What is `git init`?

`git init` is the first command used to start tracking a project with Git.

It creates a **new Git repository** inside your project folder.

```bash
git init
```

---

# 📂 What Happens After `git init`?

Before running `git init`:

```text
Project Folder
│
├── index.html
├── style.css
└── script.js
```

After running `git init`:

```text
Project Folder
│
├── .git/
├── index.html
├── style.css
└── script.js
```

> 📍 **Image:** `Images/git-init.png`

---

# 📁 What is the `.git` Folder?

The `.git` folder is automatically created after running `git init`.

It contains:

- Repository history
- Commits
- Branch information
- Project metadata
- Git configuration

> ⚠️ **Important:** Never delete the `.git` folder unless you want to remove Git from the project.

---

# 🔍 Check Repository Status

Use the following command to check the current status of your repository.

```bash
git status
```

It shows:

- New files
- Modified files
- Staged files
- Untracked files
- Current branch

---

# 📌 Command Summary

| Command | Purpose |
|---------|----------|
| `git init` | Initialize a new Git repository |
| `git status` | Check the current repository status |

---

# ✅ Key Points

- `git init` creates a new Git repository.
- Running `git init` creates a hidden `.git` folder.
- The `.git` folder stores all Git-related data.
- `git status` helps you see the current state of your project.

---

[⬆️ Back to Table of Contents](#-table-of-contents)


# ➕ What is `git add`?

After making changes to your project, Git does **not** automatically include them in the next commit.

The `git add` command moves selected changes from the **Working Directory** to the **Staging Area**.

---

# 📂 Add a Specific File

To stage a single file:

```bash
git add index.html
```

You can also stage multiple files one by one:

```bash
git add style.css
git add script.js
```

---

# 📁 Add All Files

To stage **all new and modified files** at once:

```bash
git add .
```

> 💡 `.` (dot) means **the current directory**.

---

# ⚖️ `git add <file>` vs `git add .`

| Command | Purpose |
|---------|----------|
| `git add index.html` | Stage a specific file |
| `git add .` | Stage all changes in the current directory |

---

# 🔄 Git Staging Workflow

```text
Working Directory
        │
    git add
        ▼
 Staging Area
```

> 📍 **Image:** `Images/git-add-workflow.png`

---

# 📝 Check the Status Again

After running `git add`, check the repository status:

```bash
git status
```

Staged files will appear in **green**, indicating they are ready to be committed.

---

# 📌 Command Summary

| Command | Purpose |
|---------|----------|
| `git add index.html` | Stage a specific file |
| `git add .` | Stage all changes |
| `git status` | Check staged and unstaged changes |

---

# ✅ Key Points

- `git add` stages files before committing.
- Only **staged files** are included in the next commit.
- Use `git add <file>` for specific files.
- Use `git add .` to stage all changes.
- Always verify your changes with `git status`.

---

[⬆️ Back to Table of Contents](#-table-of-contents)


# 💾 What is `git commit`?

A **commit** is a snapshot of your project at a specific point in time.

After staging your files with `git add`, use `git commit` to permanently save those changes in the Git repository.

---

# 🚀 Create Your First Commit

```bash
git commit -m "Initial commit"
```

### Explanation

- `git commit` → Saves the staged changes.
- `-m` → Adds a commit message.
- `"Initial commit"` → Describes what was saved.

> 💡 Write short and meaningful commit messages so you can easily understand your project history later.

---

# 📝 Good Commit Message Examples

```text
Initial commit
Add navigation bar
Create login page
Fix button alignment
Update README
```

---

# 🔄 Complete Git Workflow

```text
Create Project
      │
      ▼
   git init
      │
      ▼
 Edit Files
      │
      ▼
   git add
      │
      ▼
 git commit
```

> 📍 **Image:** `Images/basic-git-workflow.png`

---

# 📌 Command Summary

| Command | Purpose |
|---------|----------|
| `git init` | Initialize a Git repository |
| `git status` | Check repository status |
| `git add` | Stage files for commit |
| `git commit -m "message"` | Save staged changes with a message |

---

# 📚 Quick Revision

- **`git init`** → Start a Git repository.
- **`git status`** → View the current repository status.
- **`git add`** → Move changes to the Staging Area.
- **`git commit`** → Save staged changes as a snapshot.

---

# 🎯 Key Takeaways

- ✅ Every Git project starts with `git init`.
- ✅ Use `git status` to check the current state of your repository.
- ✅ Stage changes using `git add` before committing.
- ✅ A commit creates a snapshot of your project.
- ✅ Clear commit messages make project history easier to understand.

[⬆️ Back to Table of Contents](#-table-of-contents)
