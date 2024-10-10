---
title: Basic Git Tutorial - Common Commands and Terms
published: 2024-09-21
description: "Git is the most popular version control system (VCS) today, helping to manage source code effectively when working in groups or individually. For beginners, Git can be quite complicated, but once you master the basic commands and terms, it will become a very useful tool. In this article, we will learn some basic Git terms and commands with practical examples."
image: "./cover.jpeg"
tags: ["Git"]
category: Web Developer
draft: false
---

> Cover image source: [Source](https://ositcom.com/static/images/images/git-blog-header_1.png)

Git is the most popular version control system (VCS) today, helping to manage source code effectively when working in groups or individually. For beginners, Git can be quite complicated, but once you master the basic commands and terms, it will become a very useful tool. In this article, we will learn some basic Git terms and commands with practical examples.

---
## **Basic terms in Git**

### 1. **Repository (Repo)**
A repository or Repo is a folder that contains your entire project, including all files and their historical versions. When working with Git, you will store your source code in a repository to easily track changes and share with others.

- **Example:** When you start a new repo, Git will track all the changes you make in that directory.
### 2. **Branch**
A branch is a branch of the main version, which helps you work on new features without affecting the main source code (usually the `master` or `main` branch). Once you're done, you can merge the changes from the sub-branch back into the main branch.

- **Example:** When you're working on a new feature, you can create a new branch to experiment with without disrupting the main project.
### 3. **Conflict**
A conflict occurs when two or more different changes are made to the same file in different branches, and Git can't automatically merge them. When a conflict occurs, you have to resolve it manually by choosing which version to keep.

- **Example:** When multiple people work on a project, conflicts can arise when editing the same line of code.

### 4. **Local**
Locals are files and changes on your local computer. When you make changes to your project, they are saved locally before you push them to a server or remote repository.

- **Example:** All changes you make on your computer are local until they are pushed to GitHub or another remote server.

### 5. **Remote**
Remotes are files and changes stored on a remote server, such as GitHub, GitLab, or Bitbucket. This is where you share your source code with others.

- **Example:** You can push changes from your local to a remote repository to share with your team members.

---
## **Basic Git Commands**
### 1. **git init**
This command is used to initialize a new, empty repo. It can also convert an existing project into a Git repo:

```bash
git init
```
- **Example:** When you start a new project, you use the `git init` command to have Git track all the changes in that directory.

### 2. **git status**
This command helps check the status of the repo, showing which files have changed and which have not been saved:

```bash
git status
```
- **Example:** Before committing, you can use this command to see which changes have not been added to the staging area.

### 3. **git add**
This command prepares the file for commit. It puts the file from the working directory into the staging area:

```bash
git add <filename>
```
Or to add all files:
```bash
git add .

```

- **Example:** If you have changed many files in the project, instead of adding them one by one, you can use `git add .` to add them all.
### 4. **git reset**
This command is used to undo changes that have been added to the staging area but not yet committed:

```bash
git reset <filename>
```

- **Example:** If you accidentally added a file to the staging area but then did not want to commit it, you can use `git reset` to remove the file from the staging area.
### 5. **git commit -m 'message'**
This command saves the changes to Git along with a brief description message:

```bash
git commit -m "Initial commit"
```

- **Example:** Whenever you complete a feature or fix a bug, you will use `git commit` to save the current version of the project.

### 6. **git log**
This command shows the history of commits that have been made in the repo:

```bash
git log
```

- **Example:** To view old versions or track the change history of a project, you can use `git log`.
### 7. **git checkout**
This command switches between branches in the repository:

```bash
git checkout <branch name>
```

- **Example:** When you want to switch to working on a different branch, you can use `git checkout`.

### 8. **git merge**
This command merges changes from another branch into the current branch:

```bash
git merge <branch name>
```

- **Example:** After completing a feature in a sub-branch, you can merge it into the `master` branch.

### 9. **git push**
This command pushes changes from the local repository to the remote repository:

```bash
git push origin <branch name>
```

- **Example:** After committing, you can use `git push` to push changes from your local computer to GitHub.
### 10. **git clone**
This command copies a repo from a remote to a local one:

```bash
git clone <repo url>
```

- **Example:** When you want to download source code from GitHub to your computer, you will use the `git clone` command.

---
### **Create a .gitignore file**
Sometimes you don't want to push certain files to a remote repository (like a configuration file or a library). To do this, you create a `.gitignore` file and add the file or directory name you want to ignore to it.

```bash
touch .gitignore
```
- **Example:** If you want to ignore a `.env` file, you just add that file name to `.gitignore`.

---

This article has introduced the basics of Git, including important terms and commands. Once you master Git, you'll be able to manage projects efficiently and collaborate easily with others. Practice using Git on real projects to get a deeper understanding of how it works.

See the homepage for more information: [Boo Space Blog](www.boospace.blog)
Site resources: [Boo Space Gumroad](https://boospace.gumroad.com)
Additional products: [Linktr](https://linktr.ee/boospace)