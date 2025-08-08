# DevOps Git Project – Complete Documentation

## Objective
This project demonstrates a complete Git-based DevOps workflow, including repository initialization, branching, merging via pull requests, proper documentation, ignoring unnecessary files, tagging releases, and recording tasks in Markdown.

---

## Tools Used
- **Git** – Version control system
- **GitHub** – Remote repository hosting

---

## Step 1: Initialize Repository & Push to GitHub
**Actions:**
- Created a local project folder.
- Initialized Git repository.
- Created `README.md`.
- Staged and committed files.
- Linked to GitHub and pushed to `main` branch.

**Commands:**

mkdir devops-git-task
cd devops-git-task
git init
echo "# DevOps Git Project" > README.md
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yogeshpenumur/Version-Controlled-System-DevOps-task-4 
git push -u origin main

 ## Step 2: Create Branches

 **Commands:**
 # Create development branch
git checkout -b dev
git push -u origin dev

# Create feature branch
git checkout -b feature/add-ci-pipeline

git push -u origin feature/add-ci-pipeline

## Step 3: Use Pull Requests to Merge
- Go to your GitHub repository.
- Click Compare & Pull Request to merge feature/add-ci-pipeline → dev.
- Merge the PR.
- Create another PR from dev → main.
- Merge it.
Result: Code flows from feature branches → dev → main.

## Step 4: Use .gitignore
# Create .gitignore
# Ignore Python cache
__pycache__/
*.pyc

**Commands:**

# Commit .gitignore
git add .gitignore
git commit -m "Add .gitignore file"
git push


## Step 5: Add Git Tags
# Add a version tag
git tag v1.0

# Push tags to GitHub
git push origin v1.0
Result: Version v1.0 tagged for release tracking

## Step 6 : Document Tasks Using Markdown

# DevOps Git Project Tasks

## Task 1: Initialize Repo
- Created repo locally
- Pushed to GitHub

## Task 2: Branching
- Created dev and feature branches

## Task 3: Merging
- Used PRs for merging

## Task 4: Documentation
- Added README.md and .gitignore
- Tagged version v1.0

 **Commands:**

 # Commit and push
git add TASKS.md
git commit -m "Add tasks documentation"
git push
