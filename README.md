# Git

This repository contains useful Git commands that I personally use when working with local and remote repositories through the console.

Here, I document the exact steps I followed to create my GitHub portfolio and some additional useful commands.

## Table of Contents

- [Setting Up the Repository](#setting-up-the-repository)
  - [Cloning the Repository](#cloning-the-repository)
  - [Checking the Repository Status](#checking-the-repository-status)
  - [Opening VS Code from the Console](#opening-vs-code-from-the-console)
  - [Staging Changes](#staging-changes)
  - [Committing Changes](#committing-changes)
  - [Pushing Commits](#pushing-commits)
  - [Pulling Latest Changes](#pulling-latest-changes)
  - [Viewing Commit History](#viewing-commit-history)
  - [Resetting Changes](#resetting-changes)
- [Working with Branches](#working-with-branches)
  - [Creating a New Branch](#creating-a-new-branch)
  - [Listing All Branches](#listing-all-branches)
  - [Switching to Another Branch](#switching-to-another-branch)
  - [Creating and Switching to a New Branch](#creating-and-switching-to-a-new-branch)
  - [Merging Branches](#merging-branches)
  - [Deleting a Branch](#deleting-a-branch)
  - [Handling Merge Conflicts](#handling-merge-conflicts)

## Setting Up the Repository

### Creating the Repository

```sh
git init mayrituals
```

If your GitHub username matches the repository name, GitHub automatically creates a special `README.md` file that can be used to set up a portfolio.

### Cloning the Repository

```sh
git clone https://github.com/mayrituals/mayrituals.git
```

Copy the repository link from GitHub and use the command above to clone it to your local machine.

### Checking the Repository Status

```sh
git status
```

This command helps verify if there are any changes or untracked files in the repository.

### Opening VS Code from the Console

```sh
code mayrituals
```

This opens VS Code, allowing you to start editing files. Don't forget to save changes (`CTRL + S`).

### Staging Changes

```sh
git add .
```

or for specific files:

```sh
git add filename.ext
```

This prepares the changes to be committed.

### Committing Changes

```sh
git commit -m "Updated portfolio description"
```

### Pushing Commits

```sh
git push
```

This uploads local commits to the remote GitHub repository.

### Pulling Latest Changes

```sh
git pull
```

Use this if changes were made remotely and you need to update your local copy.

### Viewing Commit History

```sh
git log
```

This displays the commit history of the repository.

### Resetting Changes

```sh
git reset --hard HEAD~1
```

This resets the repository to the previous commit, discarding all changes.

## Working with Branches

### Creating a New Branch

```sh
git branch feature-branch
```

### Listing All Branches

```sh
git branch
```

### Switching to Another Branch

```sh
git checkout feature-branch
```

or

```sh
git switch feature-branch
```

### Creating and Switching to a New Branch

```sh
git checkout -b new-branch
```

or

```sh
git switch -c new-branch
```

### Merging Branches

```sh
git checkout main
git merge feature-branch
```

This merges `feature-branch` into the `main` branch.

### Deleting a Branch

```sh
git branch -d feature-branch
```

Use this to delete a branch after merging it into `main`. If the branch hasn’t been merged yet, force delete it with:

```sh
git branch -D feature-branch
```

### Handling Merge Conflicts

If you encounter a merge conflict, Git will notify you. Open the conflicting files and manually resolve the conflicts. After resolving them, run:

```sh
git add .
git commit -m "Resolved merge conflict"
```

This finalizes the merge and commits the resolved changes.

---

This guide serves as my personal reference when working with Git. I hope it helps others as well!
