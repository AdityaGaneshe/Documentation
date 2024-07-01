# Documentation
# Git Basics and GitHub Repository Management Tutorial
## Introduction to Git and GitHub
### What is Git?
Git is a distributed version control system that allows multiple people to work on a project simultaneously without overriding each other's changes. It helps track changes, revert to previous states, and manage code across various branches.

### What is GitHub?
GitHub is a cloud-based platform that hosts Git repositories. It provides tools for collaboration, issue tracking, code review, and more.

## Installing Git
1. **Windows:**
   - Download and install Git from [git-scm.com](https://git-scm.com/).
   - Follow the installation instructions.

2. **Mac:**
   - Install Git using Homebrew:
     ```bash
     brew install git
     ```

3. **Linux:**
   - Install Git using the package manager:
     ```bash
     sudo apt-get install git
     ```

## Configuring Git

After installing Git, configure it with your name and email address. This information will be associated with your commits.

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

## Basic Git Commands

### Creating a Repository

To create a new Git repository, navigate to your project directory and run:

```bash
git init
```

This command initializes a new Git repository in the current directory.

### Cloning a Repository

To clone an existing repository from GitHub:

```bash
git clone https://github.com/username/repository.git
```

This command creates a copy of the repository on your local machine.

### Staging and Committing Changes

1. **Staging Changes:**
   Add files to the staging area:

   ```bash
   git add filename
   ```

   Or add all changes:

   ```bash
   git add .
   ```

2. **Committing Changes:**
   Commit the staged changes with a descriptive message:

   ```bash
   git commit -m "Your commit message"
   ```

### Branching and Merging

1. **Creating a Branch:**
   ```bash
   git branch branch-name
   ```

2. **Switching to a Branch:**
   ```bash
   git checkout branch-name
   ```

3. **Merging a Branch:**
   Switch to the branch you want to merge into (e.g., `main`), then:

   ```bash
   git merge branch-name
   ```

### Viewing Commit History

View the commit history to see what changes have been made:

```bash
git log
```

### Pushing and Pulling Changes

1. **Pushing Changes:**
   Push your changes to the remote repository:

   ```bash
   git push origin branch-name
   ```

2. **Pulling Changes:**
   Pull the latest changes from the remote repository:

   ```bash
   git pull origin branch-name
   ```

## Managing GitHub Repositories

### Creating a GitHub Repository

1. **Sign in to GitHub:**
   Go to [GitHub](https://github.com/) and sign in or create an account.

2. **Create a New Repository:**
   - Click the "+" icon in the upper-right corner and select "New repository."
   - Fill in the repository name and description.
   - Choose to make the repository public or private.
   - Click "Create repository."

### Connecting a Local Repository to GitHub

After creating a repository on GitHub, connect your local repository to it:

```bash
git remote add origin https://github.com/username/repository.git
```

Push your local changes to the remote repository:

```bash
git push -u origin main
```

### Collaborating with Others

To collaborate with others, you can invite collaborators to your repository via GitHub. They will need to clone the repository and set up their own local versions.

### Using Pull Requests

Pull requests are a way to propose changes to a repository. To create a pull request:

1. **Create a Branch:**
   ```bash
   git checkout -b feature-branch
   ```

2. **Make Changes and Commit:**
   ```bash
   git add .
   git commit -m "Add new feature"
   ```

3. **Push the Branch:**
   ```bash
   git push origin feature-branch
   ```

4. **Create a Pull Request:**
   - Go to the repository on GitHub.
   - Click on the "Pull requests" tab.
   - Click "New pull request."
   - Select your branch and describe the changes.
   - Click "Create pull request."

## Best Practices

1. **Commit Often:**
   Make small, frequent commits with clear messages.

2. **Use Branches:**
   Work on new features or bug fixes in separate branches to keep the main branch stable.

3. **Write Descriptive Commit Messages:**
   Provide clear and concise messages that explain the purpose of the changes.

4. **Review Code:**
   Use pull requests to review code before merging it into the main branch.

5. **Keep Repositories Clean:**
   Regularly delete stale branches and keep the repository organized.
