# Branching Guide in Git

## Table of Contents
1. [Introduction to Branching](#introduction-to-branching)
2. [Creating a Branch](#creating-a-branch)
3. [Switching Branches](#switching-branches)
4. [Merging Branches](#merging-branches)
5. [Rebasing Branches](#rebasing-branches)
6. [Deleting Branches](#deleting-branches)
7. [Checking Branches](#checking-branches)
8. [Conclusion](#conclusion)

## Introduction to Branching
Branching in Git allows you to diverge from the main line of development and continue to work independently without affecting the main codebase.

## Creating a Branch
To create a new branch, use:
```bash
git branch <branch-name>
```
Example:
```bash
git branch feature-x
```

## Switching Branches
To switch to a different branch, use:
```bash
git checkout <branch-name>
```
Example:
```bash
git checkout feature-x
```
Alternatively, you can create and switch in one command:
```bash
git checkout -b <branch-name>
```

## Merging Branches
To merge changes from one branch into another, first switch to the target branch and then use:
```bash
git merge <branch-name>
```
Example:
```bash
git checkout main
git merge feature-x
```

## Rebasing Branches
Rebasing allows you to move or combine a sequence of commits to a new base commit. Use:
```bash
git rebase <branch-name>
```
Example:
```bash
git checkout feature-x
git rebase main
```

## Deleting Branches
To delete a branch that is no longer needed, use:
```bash
git branch -d <branch-name>
```
Example:
```bash
git branch -d feature-x
```

## Checking Branches
To see a list of all branches, use:
```bash
git branch
```
To see the current branch, check:
```bash
git branch --show-current
```

## Conclusion
Branching is a powerful feature in Git that allows for efficient parallel development. Understanding how to create, manage, and merge branches is essential for effective version control.
