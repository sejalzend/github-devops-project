# DevOps Git Workflow Project :rocket:

## Overview

This project demonstrates a complete Git workflow from initialization to production release, following DevOps best practices. It includes branching strategies, pull requests, version tagging, and documentation.

## Steps Performed

1. Initialize Local Repository

'''bash

- git init
- echo "DevOps Project" > README.md
- echo "node_modules/" > .gitignore
- git add . 
- git commit -m "Initial commit"

2. Push to GitHub
git remote add origin https://github.com/sejalzend/github-devops-project.git
git push -u origin main

3. Create Branch Structure
git checkout -b dev
git push origin dev
git checkout -b feature/login-button

4. Make Feature Changes
echo "Feature content" > feature.txt
git add .
git commit -m "Added a new feature file"
git push origin feature/login-button

5. Create Pull Request(PR)
On GitHub: Compare & Pull Request feature/login-button --> dev
Review and Merge PR

6. Merge to Production
Create PR: Compare dev --> main
Use "Squash and Merge"

7. Version Tagging
git tag -a v1.0.0 -m "First stable release" 
git push origin v1.0.0



