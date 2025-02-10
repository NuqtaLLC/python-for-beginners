# Introduction to Git: A Beginner's Guide

## Lesson Objectives
By the end of this lesson, you will:
- Understand what Git is and why it is useful.
- Learn how to install and configure Git.
- Understand basic Git commands for version control.
- Learn how to create, clone, and manage repositories.
- Use Git to track changes in a project.

## What is Git?
Git is a distributed version control system that allows multiple developers to collaborate on a project. It helps track changes, revert to previous versions, and merge code from different contributors.

### Why Use Git?
- **Version Control**: Keeps track of changes and history of a project.
- **Collaboration**: Multiple developers can work on the same project.
- **Branching and Merging**: Work on different features without affecting the main codebase.
- **Backup**: Keeps a safe history of your code in case of mistakes.

## Installing Git
1. **Windows**:
   - Download Git from [git-scm.com](https://git-scm.com/downloads) and follow the installation steps.
2. **Mac**:
   - Install using Homebrew: `brew install git`
3. **Linux**:
   - Use the package manager: `sudo apt install git` (Debian-based) or `sudo yum install git` (Red Hat-based).

## Configuring Git
After installing, configure Git with your name and email:
```sh
$ git config --global user.name "Your Name"
$ git config --global user.email "your.email@example.com"
```
To check your configuration:
```sh
$ git config --list
```

## Basic Git Workflow
### 1. Initializing a Repository
To start tracking a project with Git:
```sh
$ git init
```
This creates a hidden `.git` directory that stores version control information.

### 2. Cloning a Repository
To copy an existing repository from a remote source (e.g., GitHub):
```sh
$ git clone https://github.com/user/repo.git
```

### 3. Checking Status
To see which files have changed:
```sh
$ git status
```

### 4. Adding Changes
To add a file to the staging area:
```sh
$ git add filename.txt
```
To add all files:
```sh
$ git add .
```

### 5. Committing Changes
After adding files, save them to the repository:
```sh
$ git commit -m "Added new feature"
```

### 6. Viewing Commit History
To see past commits:
```sh
$ git log
```

### 7. Pushing to a Remote Repository
To upload local commits to a remote repository:
```sh
$ git push origin main
```

### 8. Pulling Changes from a Remote Repository
To get the latest updates from a remote repository:
```sh
$ git pull origin main
```

## Working with Branches
Branches allow you to work on different features separately.

### 1. Creating a New Branch
```sh
$ git branch new-feature
```

### 2. Switching to a Branch
```sh
$ git checkout new-feature
```
Or, using the newer command:
```sh
$ git switch new-feature
```

### 3. Merging Branches
Once you are done working on a branch, merge it into the main branch:
```sh
$ git checkout main
$ git merge new-feature
```

### 4. Deleting a Branch
```sh
$ git branch -d new-feature
```

## Summary
- **Git tracks changes** in a project and allows collaboration.
- **Repositories** store version history.
- **Commits** save changes with messages describing updates.
- **Branches** allow parallel development.
- **Push and pull** commands sync local and remote repositories.

## Next Steps
- Try setting up a Git repository and committing changes.
- Practice branching and merging.
- Learn about GitHub for remote collaboration.

This concludes our introduction to Git. Happy coding!

