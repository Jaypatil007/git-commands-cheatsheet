# Git Clone Guide

## 1. What is Cloning?
Cloning creates a local copy of a remote repository. It enables you to work offline and push changes later.

## 2. Cloning a Repository

**Command:**
```bash
git clone <repository-url>
```
**Example:**
```bash
git clone https://github.com/Jaypatil007/git-commands-cheatsheet.git
```

This creates a directory named after the repo, with all its files and history.

## 3. Cloning Into a Specific Directory

**Command:**
```bash
git clone <repository-url> <directory-name>
```
**Example:**
```bash
git clone https://github.com/Jaypatil007/git-commands-cheatsheet.git my-git-guide
```

## 4. Cloning a Specific Branch

**Command:**
```bash
git clone -b <branch-name> <repository-url>
```
**Example:**
```bash
git clone -b develop https://github.com/Jaypatil007/git-commands-cheatsheet.git
```

## 5. Cloning With Submodules

If your repo uses submodules:
```bash
git clone --recurse-submodules <repository-url>
```

## 6. Advanced: Clone a Shallow Copy

Speeds up cloning by only fetching recent history:
```bash
git clone --depth 1 <repository-url>
```

## 7. Common Issues

- **Authentication Required:** For private repos, use SSH or provide credentials.
- **Large Files:** Shallow clone, or use Git LFS for large files.

## 8. References

- [Official Git Docs: clone](https://git-scm.com/docs/git-clone)
