![banner](https://github.com/maurya-kavi/Git-and-GitHub-at-ChaiCode-Cohort-/blob/main/screenshort/Screenshot%202025-01-12%20004347.png)

# Welcome to Git and GitHub at ChaiCode Cohort!

This documentation will guide new developers joining the ChaiCode Cohort through using Git and GitHub effectively. Git is a vital version control tool, and GitHub provides a collaborative platform for managing code. Mastering these tools will ensure smooth collaboration and efficient version control for all projects.

---

![Git & Github](https://facialix.com/wp-content/uploads/2023/05/curso-git-y-github-facialix.jpg)

## Table of Contents
1. [What is Git?](#what-is-git)
2. [Why Use Git?](#why-use-git)
3. [What is GitHub?](#what-is-github)
4. [Installing Git](#installing-git)
5. [Configuring Git](#configuring-git)
6. [Cloning the ChaiCode Repository](#cloning-the-chaicode-repository)
7. [Basic Git Commands](#basic-git-commands)
8. [Commit Message Rules](#commit-message-rules)
9. [Branching Workflow](#branching-workflow)
10. [Pull Requests (PR)](#pull-requests-pr)
11. [Common Git Errors and Fixes](#common-git-errors-and-fixes)

---

## 1. What is Git?
Git is a distributed version control system that allows multiple people to work on a project simultaneously without overwriting each other’s changes. It tracks changes in files and coordinates work among multiple developers.

---

## 2. Why Use Git?
- **Collaboration**: Work on the same project with others.
- **Version History**: Track changes over time.
- **Branching and Merging**: Develop features independently.

---

## 3. What is GitHub?
GitHub is a web-based platform for hosting Git repositories. It provides collaboration features like pull requests, code reviews, and issue tracking.

---

## 4. Installing Git

### Windows
1. Download the Git installer from [Git Official Website](https://git-scm.com/).
2. Run the installer and follow the steps.
3. Verify installation: Open **Command Prompt** and run:
   ```bash
   git --version
   ```
![Git Installation](https://cdn.hashnode.com/res/hashnode/image/upload/v1736507024393/ad7e0ac6-7ccb-4716-ba84-9ed586084dd2.png?auto=compress,format&format=webp)

![git1](https://cdn.hashnode.com/res/hashnode/image/upload/v1736509626957/b4ff245d-2fe8-4094-92d8-df101d480feb.png?auto=compress,format&format=webp)

![git2](https://cdn.hashnode.com/res/hashnode/image/upload/v1736510452564/34cdfcdb-51ec-4347-8bb4-09bf063038e6.png?auto=compress,format&format=webp)

### macOS
1. Use Homebrew:
   ```bash
   brew install git
   ```
2. Verify installation:
   ```bash
   git --version
   ```

### Linux
1. Use the package manager:
   ```bash
   sudo apt-get install git
   ```
2. Verify installation:
   ```bash
   git --version
   ```

---

#SETTING UP Git & GitHub :-
## 5. Configuring Git
Set up your username and email for Git:
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```
1.If yor are new to GitHub - click on the Sign Up button. If you are already an existing user - click on Sign In . 
![config git](https://cdn.hashnode.com/res/hashnode/image/upload/v1736521367456/0c09ec5b-446d-432a-8968-91e4d6b9c0d0.gif?auto=format,compress&gif-q=60&format=webm)

2.Enter all the details and press Continue
![config2 git](https://cdn.hashnode.com/res/hashnode/image/upload/v1736523170089/38e267e7-9771-4167-a9a1-0fb38807bc0e.gif?auto=format,compress&gif-q=60&format=webm)


#CREATING A REPOSITORY:-
1. In GitHub a repository is like a project folder. To create a new repository click on the green new button on the left sidebar or, click on the "plus (+)” icon on the top-right corner of the nav bar.
![repo1](https://cdn.hashnode.com/res/hashnode/image/upload/v1736525983307/a9056555-3b9a-4359-ab92-61120cea0de7.png?auto=compress,format&format=webp)

2. Add a repository name, select visibility, add readme.md file if required.
![repos2](https://cdn.hashnode.com/res/hashnode/image/upload/v1736527368824/e5781647-c5be-4f40-ade2-24b77beae8f2.png?auto=compress,format&format=webp)


## 6. Cloning the ChaiCode Repository
To clone a repository:
```bash
git clone https://github.com/ChaiCode/example-repo.git
```
Navigate into the cloned repository:
```bash
cd example-repo
```

---

## 7. Basic Git Commands
| Command | Description |
|---------|-------------|
| `git init` | Initialize a new repository |
| `git status` | Check the status of changes |
| `git add <file>` | Stage changes |
| `git commit -m "message"` | Commit staged changes |
| `git push origin <branch>` | Push changes to remote |
| `git pull` | Fetch and merge changes from remote |
| `git log` | View commit history |

---

## 8. Commit Message Rules
- Use the present tense ("Add feature" not "Added feature").
- Capitalize the first letter.
- Keep the message short (50 characters or less).
- Use prefixes like `fix:`, `feat:`, `chore:`, `docs:` for categorization.

Examples:
```bash
feat: Add tea selection feature
fix: Resolve login issue for tea enthusiasts
docs: Update README with chai varieties
```

---

## 9. Branching Workflow
### Branching Strategy
- **main**: Stable production-ready code.
- **development**: Active development.
- **feature/branch-name**: Individual features.
![workflow](https://cdn.hashnode.com/res/hashnode/image/upload/v1736602223140/467581e2-0b11-4027-8d1a-9ee3a723b25f.png?auto=compress,format&format=webp)

### Create a Branch
```bash
git branch feature/tea-menu
```
### Switch to Branch
```bash
git checkout feature/tea-menu
```
### Merge Branch
```bash
git checkout main
git merge feature/tea-menu
```

---

## 10. Pull Requests (PR)
1. Push your branch to GitHub.
2. Click **Compare & pull request**.
3. Add details and create the pull request.

![GitHub Pull Request](https://www.earthdatascience.org/images/earth-analytics/git-version-control/github-create-new-pull-request.png)

### Writing PR Descriptions
- Provide a summary of changes.
- Mention any issues fixed.
- Request reviews from relevant team members.

---

## 11. Common Git Errors and Fixes
| Error | Cause | Solution |
|-------|-------|----------|
| `fatal: not a git repository` | Not in a Git repository | Navigate to the correct directory or initialize with `git init`. |
| `merge conflict` | Conflicting changes | Edit conflicting files and run `git commit`. |

---

Happy coding with Git and GitHub!


