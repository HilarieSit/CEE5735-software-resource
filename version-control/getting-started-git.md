---
description: >-
  Git is a popular version control system that allows you to save and access
  histories of files. Git is great for tracking & testing multiple versions of
  code and for collaborative coding.
---

# Getting started

## On this page:

1. [Installation & Guide](https://github.com/git-guides/install-git)
2. [General Idea & Basics](getting-started-git.md#general-idea-and-basics)
3. [GitHub](getting-started-git.md#github-remote-repositories)

## Installation & Guide

Follow the directions here to install git:

{% embed url="https://github.com/git-guides/install-git" %}

## General Idea & Basics

Git lets you use branches to test new features/code while keeping a clean record on the main master branch. This functionality is great: if the experimental feature is unsuccessful, it doesn't effect the copy on the master branch; otherwise, if successful, it can be merged back into the master branch. 

![https://nvie.com/posts/a-successful-git-branching-model/](../.gitbook/assets/image%20%284%29.png)

To create a local git repository, run `git init` in the desired directory. To add or update files in the local repo, first use `git add <filename>` to add individual files or  `git add .` to add all files \(excluding those in [.gitignore](getting-started-git.md#gitignore-file)\). This moves the updated files into the staging area and you can check the status using `git status`. Then, commit these changes to the local repo using `git commit -m <message>` and you can check commit history with `git log`. 

To collaborate, you would want to set up a remote repository on [GitHub](getting-started-git.md#github-remote-repositories). To update the files on the remote repo, use `git push`. To update your local repo \(_e.g._ when a collaborator has edited something in the remote repo\), use `git pull`. Be sure to use `git pull` before `git push`, and if there is a conflict, you may need to merge the code before pushing onto the remote repo.

![https://medium.com/@gagansuneja](../.gitbook/assets/image.png)

### .gitignore file

List the directories and files \(e.g. big data files, private info/keys, virtual environment directory, etc.\) that you don't want to track with git in a file named _.gitignore_.

## GitHub: Remote Repositories

GitHub is really popular for hosting remote Git repositories. Create an account on GitHub: 

{% embed url="https://github.com" %}

