# 📚 Programming Hero - Smart Notes

## Class 2-4

# 💻 VS Code Terminal to Set Up Basic Git (Windows)

> **Class Duration:** _As covered in the course_

---

# 📑 Table of Contents

- [📖 What You'll Learn](#-what-youll-learn)
- [💻 Open Terminal in VS Code](#-open-terminal-in-vs-code)
- [🔍 Check Git Installation](#-check-git-installation)
- [👤 Set Your Git Username](#-set-your-git-username)
- [📧 Set Your Git Email](#-set-your-git-email)
- [✅ Verify Git Configuration](#-verify-git-configuration)
- [👤 Check Username](#-check-username)
- [📧 Check Email](#-check-email)
- [🌍 View Global Configuration](#-view-global-configuration)
- [🌐 Global vs Local Configuration](#-global-vs-local-configuration)
- [💡 Best Practices](#-best-practices)
- [⚠️ Common Mistakes](#️-common-mistakes)
- [📚 Quick Revision](#-quick-revision)
- [📌 Command Cheat Sheet](#-command-cheat-sheet)
- [🎯 Key Takeaways](#-key-takeaways)

---

# 📖 What You'll Learn

- Open Terminal in VS Code
- Check Git Installation
- Configure Git for the First Time
- Set Username & Email
- Verify Git Configuration

---

# 💻 Open Terminal in VS Code

There are two common ways to open the integrated terminal.

### Method 1

Go to:

```text
Terminal → New Terminal
```

### Method 2 (Shortcut)

```text
Ctrl + `
```

> 💡 The terminal opens at the bottom of VS Code.

---

# 🔍 Check Git Installation

Before using Git, make sure it is installed on your computer.

Run:

```bash
git --version
```

Example Output:

```text
git version 2.xx.x.windows.x
```

If a version number appears, Git is installed successfully.

> 📍 **Image:** `Images/git-version.png`

---

# 👤 Set Your Git Username

Configure the username that will appear in your commits.

```bash
git config --global user.name "Your Name"
```

Example:

```bash
git config --global user.name "John Doe"
```

> 💡 Use your real name or the name you want to display on GitHub.

---

# 📧 Set Your Git Email

Configure the email associated with your GitHub account.

```bash
git config --global user.email "you@example.com"
```

Example:

```bash
git config --global user.email "johndoe@gmail.com"
```

> ⚠️ It's recommended to use the same email as your GitHub account.

---

# 📌 Command Summary

| Command | Purpose |
|---------|----------|
| `git --version` | Check installed Git version |
| `git config --global user.name "Your Name"` | Set Git username |
| `git config --global user.email "you@example.com"` | Set Git email |

---

# ✅ Key Points

- Open the terminal from VS Code before running Git commands.
- Check Git installation using `git --version`.
- Configure your username and email only once on a new computer.
- Use the same email as your GitHub account for better consistency.

---

[⬆️ Back to Table of Contents](#-table-of-contents)


# ✅ Verify Git Configuration

After setting your username and email, it's a good idea to verify your configuration.

---

# 👤 Check Username

Run:

```bash
git config user.name
```

Example Output:

```text
John Doe
```

---

# 📧 Check Email

Run:

```bash
git config user.email
```

Example Output:

```text
johndoe@gmail.com
```

---

# 🌍 View Global Configuration

To see all your global Git settings:

```bash
git config --global --list
```

Example Output:

```text
user.name=John Doe
user.email=johndoe@gmail.com
```

> 📍 **Image:** `Images/git-config-list.png`

---

# 🌐 Global vs Local Configuration

| Global Configuration | Local Configuration |
|----------------------|---------------------|
| Applies to all Git repositories | Applies only to the current repository |
| Set using `--global` | Set without `--global` |
| Usually configured once | Used when a project needs different settings |

> 💡 For most beginners, using **Global Configuration** is the best choice.

---

# 📌 Command Summary

| Command | Purpose |
|---------|----------|
| `git config user.name` | View current username |
| `git config user.email` | View current email |
| `git config --global --list` | View all global Git settings |

---

# ✅ Key Points

- Verify your Git configuration after setup.
- `git config user.name` shows the configured username.
- `git config user.email` shows the configured email.
- `git config --global --list` displays all global Git settings.
- Global configuration is usually done only once per computer.

---

[⬆️ Back to Table of Contents](#-table-of-contents)


# 💡 Best Practices

Follow these tips while configuring Git for the first time:

- Use your **real name** or the name you want to appear in your commits.
- Use the **same email** as your GitHub account.
- Verify your configuration after setup.
- Configure Git only **once** on a new computer.
- Keep Git updated to the latest stable version.

---

# ⚠️ Common Mistakes

| Mistake | Solution |
|---------|----------|
| Git is not installed | Install Git and run `git --version` |
| Incorrect username | Update it using `git config --global user.name` |
| Wrong email address | Update it using `git config --global user.email` |
| Forgetting to verify settings | Run `git config --global --list` |

---

# 📚 Quick Revision

### Essential Git Setup Commands

```bash
git --version
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global --list
```

---

# 📌 Command Cheat Sheet

| Command | Purpose |
|---------|----------|
| `git --version` | Check installed Git version |
| `git config --global user.name "Your Name"` | Set Git username |
| `git config --global user.email "you@example.com"` | Set Git email |
| `git config user.name` | View current username |
| `git config user.email` | View current email |
| `git config --global --list` | Display all global Git settings |

---

# 🎯 Key Takeaways

- ✅ Configure Git before starting your first project.
- ✅ Set your username and email only once using `--global`.
- ✅ Use the same email as your GitHub account.
- ✅ Verify your configuration before using Git.
- ✅ Proper configuration helps Git identify your commits correctly.

[⬆️ Back to Table of Contents](#-table-of-contents)
