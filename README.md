Complete Guide to Git and GitHub

Welcome to the ultimate guide for understanding and using Git and GitHub, from the basics to more advanced features.

Table of Contents

What is Git?

Why Use Git?

What is GitHub?

Installing Git

Basic Git Commands

Working with GitHub

Branching and Merging

Using GitHub Issues and Pull Requests

Common Git Errors and Fixes

1. What is Git?

Git is a distributed version control system that allows multiple people to work on a project simultaneously without overwriting each other’s changes. It tracks changes in files and coordinates work among multiple developers.

2. Why Use Git?

Collaboration: Work on the same project with others.

Version History: Track changes over time.

Branching and Merging: Develop features independently.

3. What is GitHub?

GitHub is a web-based platform for hosting Git repositories. It provides collaboration features like pull requests, code reviews, and issue tracking.

4. Installing Git

Windows

Download the Git installer from Git Official Website.

Run the installer and follow the steps.

Verify installation: Open Command Prompt and run:

git --version

macOS

Use Homebrew:

brew install git

Verify installation:

git --version

Linux

Use the package manager:

sudo apt-get install git

Verify installation:

git --version



5. Basic Git Commands

Command

Description

git init

Initialize a new repository

git clone <repo_url>

Clone a repository

git status

Check the status of changes

git add <file>

Stage changes

git commit -m "message"

Commit staged changes

git push origin <branch>

Push changes to remote

git pull

Fetch and merge changes from remote

6. Working with GitHub

Creating a Repository

Sign in to GitHub.

Click New under Repositories.

Enter repository name, description, and visibility.

Click Create repository.

Connecting Local Repository to GitHub

git remote add origin https://github.com/username/repository.git

Pushing to GitHub

git push -u origin main



7. Branching and Merging

Create a Branch

git branch feature-branch

Switch to Branch

git checkout feature-branch

Merge Branch

git checkout main
git merge feature-branch

8. Using GitHub Issues and Pull Requests

Creating an Issue

Go to the repository.

Click Issues > New Issue.

Fill in the title and description.

Creating a Pull Request

Push a branch to GitHub.

Click Compare & pull request.

Add details and create the pull request.



9. Common Git Errors and Fixes

Error

Cause

Solution

fatal: not a git repository

Not in a Git repository

Navigate to the correct directory or initialize with git init.

merge conflict

Conflicting changes

Edit conflicting files and run git commit.

Happy coding with Git and GitHub!


