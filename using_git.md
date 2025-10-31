# Git Installation and Usage Guide

Git is a **version control system** that lets you track changes in your code, collaborate with others, and manage projects efficiently.  
This guide will walk you through **installing Git**, **setting it up**, and **using basic commands** to get started.

---

## 1. Installing Git

### Windows
1. Go to the [official Git website](https://git-scm.com/download/win).
2. The download should start automatically. Run the installer once it finishes.
3. Accept the default options unless you have a specific need to change them.
4. After installation, open **Git Bash** (installed with Git) or **Command Prompt**.
5. Verify installation:
   ```bash
   git --version
   ```
   You should see output like `git version 2.44.0` (version may vary).

---

### macOS
1. You can install Git in several ways:

   **Option 1 – Using Homebrew (recommended):**
   ```bash
   brew install git
   ```

   **Option 2 – Using Xcode Command Line Tools:**
   ```bash
   xcode-select --install
   ```

2. Verify installation:
   ```bash
   git --version
   ```

---

### Linux (Ubuntu/Debian)
1. Update your package list and install Git:
   ```bash
   sudo apt update
   sudo apt install git
   ```

2. Verify installation:
   ```bash
   git --version
   ```

---

## 2. Setting Up Git

Before using Git, configure your name and email (this information is stored in commits):

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

To verify your settings:
```bash
git config --list
```

---

## 3. Creating or Cloning a Repository

### Create a New Repository
If you want to start a new project:
```bash
mkdir my-project
cd my-project
git init
```
This creates a hidden `.git` folder that tracks your files.

### Clone an Existing Repository
To copy a remote project (e.g., from GitHub):
```bash
git clone https://github.com/username/repository.git
```

---

## 4. Basic Git Workflow

Below is the standard Git workflow for making and saving changes.

### 1️. Check the Repository Status
```bash
git status
```
Shows which files have been modified, added, or are untracked.

### 2️. Add Files to the Staging Area
```bash
git add filename
```
Or add all modified files:
```bash
git add .
```

### 3️. Commit Your Changes
```bash
git commit -m "Describe what you changed"
```

### 4️. View Commit History
```bash
git log
```

---

## 5. Working with Remote Repositories

### Add a Remote Repository
If your local repo isn’t linked yet:
```bash
git remote add origin https://github.com/username/repository.git
```

### Push Changes to GitHub
```bash
git push -u origin main
```
Use `main` or `master`, depending on your branch name.

### Pull the Latest Changes
```bash
git pull origin main
```

---

## 6. Branching

Branches let you work on features separately from the main codebase.

### Create a Branch
```bash
git branch feature-branch
```

### Switch to a Branch
```bash
git checkout feature-branch
```

### Combine Branches (Merge)
First, switch to the branch you want to merge **into** (usually `main`):
```bash
git checkout main
git merge feature-branch
```

### Delete a Branch
```bash
git branch -d feature-branch
```

---

## 7. Useful Commands Summary

| Command | Description |
|----------|-------------|
| `git init` | Create a new Git repository |
| `git clone <url>` | Copy an existing repository |
| `git status` | Check current status of files |
| `git add <file>` | Stage changes |
| `git commit -m "message"` | Save changes with a message |
| `git log` | View commit history |
| `git remote add origin <url>` | Link local repo to remote |
| `git push` | Upload commits to remote |
| `git pull` | Download latest changes |
| `git branch` | List branches |
| `git checkout <branch>` | Switch branches |
| `git merge <branch>` | Merge another branch |
| `git diff` | Show file differences |
| `git reset` | Unstage files or undo commits |

---

## 8. Tips for Beginners

- Make small, frequent commits with clear messages.
- Always pull before pushing to avoid conflicts.
- Use `.gitignore` to exclude files you don’t want tracked (e.g., build files, logs).
- You can view unstaged changes using:
  ```bash
  git diff
  ```
- If you make a mistake, don’t panic — Git keeps history! You can revert, reset, or checkout older commits safely.

---

## 9. Further Learning

- [Pro Git Book (Free)](https://git-scm.com/book/en/v2)
- [GitHub Guides](https://guides.github.com/)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)

---

*Written for beginners learning Git for the first time. Feel free to share or modify this guide for your own projects!*