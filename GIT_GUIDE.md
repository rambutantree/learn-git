# Git Guide

A quick reference for the most important Git commands used in this repository.

---

## 1. Clone a Repository

Cloning creates a local copy of a remote repository.

```bash
# Clone via HTTPS
git clone https://github.com/<username>/learn-git.git

# Clone via SSH (requires SSH key set up)
git clone git@github.com:<username>/learn-git.git

# Clone into a specific folder name
git clone https://github.com/<username>/learn-git.git my-folder
```

After cloning, move into the project directory:

```bash
cd learn-git
```

---

## 2. Pull Changes

Pulling fetches the latest commits from the remote and merges them into your current branch.

```bash
# Pull from the default remote (origin) and current branch
git pull

# Pull from a specific remote and branch
git pull origin main
```

**Tip:** Always pull before you start new work to avoid merge conflicts.

---

## 3. Stage and Commit Changes

Before pushing, you need to stage and commit your local changes.

```bash
# Check what has changed
git status

# Stage a single file
git add README.md

# Stage all changed files
git add .

# Commit with a descriptive message
git commit -m "Add notes about branching"
```

---

## 4. Push Changes

Pushing uploads your local commits to the remote repository.

```bash
# Push to the default remote and current branch
git push

# Push to a specific remote and branch
git push origin main

# Push a new local branch to the remote for the first time
git push -u origin my-feature-branch
```

---

## 5. Branching

Working on branches keeps the `main` branch stable.

```bash
# Create and switch to a new branch
git checkout -b my-feature-branch

# List all local branches
git branch

# Switch to an existing branch
git checkout main

# Delete a local branch after merging
git branch -d my-feature-branch
```

---

## 6. Checking History

```bash
# View recent commits (one line each)
git log --oneline

# View the full diff of the last commit
git show
```

---

## 7. Common Workflow Summary

```
git pull                        # get the latest changes
git checkout -b my-feature      # create a new branch
# ... edit or create .md files ...
git add .                       # stage changes
git commit -m "Describe change" # commit locally
git push -u origin my-feature   # push to GitHub
# Open a Pull Request on GitHub
```

---

## Further Reading

- [Official Git documentation](https://git-scm.com/doc)
- [GitHub Docs – Getting started](https://docs.github.com/en/get-started)
- [Pro Git book (free online)](https://git-scm.com/book/en/v2)
