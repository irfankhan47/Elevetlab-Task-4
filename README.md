# DevOps Dummy Project - Task 4

This repository is created as part of **Task 4** of my DevOps internship to demonstrate Git version control workflows using a dummy DevOps project structure.

## 🧑‍💻 Task Objective

> **Build a version-controlled DevOps project using Git best practices**

---

## 📂 Project Structure

Devops-dummy-project/<br>
├── Docker/<br>
│ └── Dockerfile<br> 
├── Jenkins/<br>
│ └── Jenkinsfile<br> 
├── Ansible/<br>
│ └── playbook.yml<br>
├── .gitignore<br>
└── README.md<br>

---

## 🔧 Tools Used

- Git
- GitHub

---

## 🔄 Git Workflow Followed

- Initialized Git locally and pushed to GitHub
- Created `main`, `dev`, and `feature-1` branches
- Made changes in `feature-1` and merged to `dev` via pull request
- Added `.gitignore` to exclude unnecessary files
- Created version tag `v1.0`

---

## 🏷️ Git Tag

- `v1.0` — first release version of this dummy project

---

## 📁 .gitignore Includes

node_modules/ .env *.log

yaml
Copy
Edit

---

## ✅ Outcome

Learned real DevOps Git workflow:
- Branching
- Pull Requests
- Tagging versions
- Using `.gitignore`

---

## 💻 Git Commands Used (With Explanation)

```bash
git init                                  # Start Git tracking in the folder
git branch -M main                        # Rename default branch to main
git remote add origin <repo-url>         # Connect to GitHub repo

git add .                                 # Stage all changes
git commit -m "Initial commit"           # Save changes with a message
git push -u origin main                  # Push main branch to GitHub

git checkout -b dev                      # Create and switch to dev branch
git push origin dev                      # Push dev branch to GitHub

git checkout -b feature-1                # Create and switch to feature-1 branch
git push origin feature-1                # Push feature-1 to GitHub

# Make some file changes in feature-1...
git add .                                 # Stage changes
git commit -m "Updated README"           # Commit changes
git push origin feature-1                # Push changes to GitHub

# (On GitHub: create a Pull Request from feature-1 → dev)

git checkout dev                         # Switch to dev branch
git pull origin dev                      # Get the latest dev branch updates

git tag -a v1.0 -m "First version"       # Create a version tag
git push origin v1.0                     # Push the tag to GitHub

touch .gitignore                         # Create .gitignore file
echo "node_modules/" >> .gitignore       # Add ignored folders/files
echo ".env" >> .gitignore
echo "*.log" >> .gitignore
git add .gitignore                       # Stage .gitignore
git commit -m "Added .gitignore"         # Commit it
git push origin dev                      # Push to dev branch
