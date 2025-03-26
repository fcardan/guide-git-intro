# 📖 Guide: Git Commands

## 🔹 Introduction
Git is a powerful version control system that helps developers collaborate and track changes efficiently. This guide covers essential Git commands, best practices, and tips to enhance your workflow.

---

## 🔹 Initial Setup

### Install Git
Download and install Git from [git-scm.com](https://git-scm.com/).

### Configure Git
```sh
# Set up your username and email (important for commit history)
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# Verify configuration
git config --list
```

---

## 🔹 Basic Git Workflow

### 1️⃣ Clone a Repository
```sh
git clone https://github.com/user/repository.git
```

### 2️⃣ Check Repository Status
```sh
git status
```

### 3️⃣ Add Files to Staging Area
```sh
git add <file>  # Add a specific file
git add .       # Add all changes
```

### 4️⃣ Commit Changes
```sh
git commit -m "Describe your change"
```

### 5️⃣ Push Changes to Remote Repository
```sh
git push origin <branch>
```

### 6️⃣ Pull Latest Changes
```sh
git pull origin <branch>
```

---

## 🔹 Working with Branches

### Create a New Branch
```sh
git branch <new-branch>
```

### Switch to a Branch
```sh
git checkout <branch>
```
OR
```sh
git switch <branch>
```

### Create & Switch to a Branch
```sh
git checkout -b <new-branch>
```
OR
```sh
git switch -c <new-branch>
```

### Merge Branches
```sh
git checkout main
git merge <branch>
```
OR
```sh
git switch main
git merge <branch>
```

### Delete a Branch
```sh
git branch -d <branch>
```

---

## 🔹 Advanced Git Commands

### Undoing Changes
```sh
git checkout -- <file>   # Discard changes in working directory
git reset HEAD <file>    # Unstage a file
git reset --hard HEAD    # Reset to last commit
```

### Rebase (Rewriting History)
```sh
git rebase main
```

### Cherry-pick (Apply Specific Commits)
```sh
git cherry-pick <commit-hash>
```

### Stash Changes
```sh
git stash           # Save uncommitted changes
git stash pop       # Apply stashed changes
git stash list      # View stashed changes
```

---

## 🔹 Best Practices

- Use **meaningful commit messages**
- Keep branches **small and focused**
- Regularly **pull latest changes** before working
- **Avoid pushing directly** to `main` or `master`
- Use **feature branches** for new developments
- **Review changes** before committing

---

## 🔹 Additional Resources

- [Official Git Documentation](https://git-scm.com/doc)
- [GitHub Learning Lab](https://lab.github.com/)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)

---

## 🔹 License

This repository is licensed. This means you are free to share and adapt this content for any purpose, even commercially, as long as you provide appropriate credit to the original author. For more details, please refer to the [LICENSE.md](https://github.com/fcardan/guide-git-commands/blob/main/LICENSE.md) file.

---

💡 *Following these best practices will help maintain clean and efficient repositories!* 🚀
