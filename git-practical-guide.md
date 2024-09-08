# Git Practical Guide for Beginners

This guide is designed for students who have GitHub accounts but are new to Git. We'll walk through installing Git, configuring it, and creating a repository that can be synced with GitHub.

## 1. Installing Git

### For Windows:
1. Go to https://git-scm.com/download/win
2. Download the installer for your system (32-bit or 64-bit)
3. Run the installer and follow the prompts, using the default options

### For macOS:
1. Open Terminal
2. Install Homebrew if you haven't already: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
3. Install Git: `brew install git`

### For Linux (Ubuntu/Debian):
1. Open Terminal
2. Update your package list: `sudo apt update`
3. Install Git: `sudo apt install git`

## 2. Configuring Git

After installation, open Command Prompt (Windows) or Terminal (macOS/Linux) and run these commands:

```
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

Replace "Your Name" with your actual name and "youremail@example.com" with the email associated with your GitHub account.

## 3. Creating a Local Repository

1. Open Command Prompt/Terminal
2. Navigate to where you want to create your project: `cd path/to/your/project`
3. Create a new directory: `mkdir my-first-repo`
4. Enter the directory: `cd my-first-repo`
5. Initialize the repository: `git init`

## 4. Adding and Committing Files

1. Create a file: `echo "Hello, Git!" > README.md`
2. Add the file to staging: `git add README.md`
3. Commit the changes: `git commit -m "Initial commit"`

## 5. Connecting to GitHub

1. Go to GitHub and log in
2. Click the '+' icon in the top right and select "New repository"
3. Name your repository (e.g., "my-first-repo")
4. Don't initialize with a README, .gitignore, or license
5. Click "Create repository"

## 6. Pushing Your Local Repository to GitHub

GitHub will show you commands to push an existing repository. Run these in your local repository:

```
git remote add origin https://github.com/your-username/my-first-repo.git
git branch -M main
git push -u origin main
```

Replace "your-username" with your actual GitHub username.

## 7. Fetching Changes from GitHub

If changes are made on GitHub (like editing a file directly on the website), you can fetch those changes:

1. Fetch the changes: `git fetch origin`
2. Merge the changes into your local main branch: `git merge origin/main`

Alternatively, you can use `git pull origin main` to fetch and merge in one step.

Congratulations! You've now set up Git, created a repository, and synced it with GitHub. Keep practicing these commands to become more comfortable with Git.
