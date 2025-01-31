# Git Basic Commands

## Introduction
Git is a distributed version control system used for tracking changes in source code. Below are the fundamental Git commands to help you get started.

---

## 1. Git Configuration
Set up your Git environment:
```sh
# Set username
git config --global user.name "Your Name"

# Set email
git config --global user.email "your.email@example.com"

# Check configuration
git config --list
```

---

## 2. Initialize a Repository
Create a new Git repository:
```sh
git init
```
Clone an existing repository:
```sh
git clone <repository_url>
```

---

## 3. Basic Workflow
### Check Repository Status
```sh
git status
```

### Add Files to Staging Area
```sh
git add <file_name>  # Add a specific file
git add .            # Add all files
```

### Commit Changes
```sh
git commit -m "Your commit message"
```

### Push Changes to Remote Repository
```sh
git push origin <branch_name>
```

---

## 4. Branching in Git
### Create a New Branch
```sh
git branch <branch_name>
```

### Switch to a Branch
```sh
git checkout <branch_name>
```
OR
```sh
git switch <branch_name>
```

### Create and Switch to a New Branch
```sh
git checkout -b <branch_name>
```
OR
```sh
git switch -c <branch_name>
```

### List All Branches
```sh
git branch
```

### Delete a Branch
```sh
git branch -d <branch_name>
```

---

## 5. Merging Branches
### Merge a Branch into the Current Branch
```sh
git merge <branch_name>
```

### Resolve Merge Conflicts
If there are conflicts, Git will prompt you to resolve them manually. After resolving conflicts:
```sh
git add .
git commit -m "Resolved merge conflict"
```

---

## 6. Pulling Changes
Fetch and merge changes from a remote repository:
```sh
git pull origin <branch_name>
```

---

## 7. Closing a Feature Branch
Once a feature is merged, delete the branch to keep the repository clean:
```sh
git branch -d <branch_name>
```
If the branch has been pushed to the remote repository, delete it remotely as well:
```sh
git push origin --delete <branch_name>
```

---

## Conclusion
These are the fundamental Git commands that will help you work efficiently with version control. Always make sure to follow best practices like using meaningful commit messages and keeping your branches organized.

