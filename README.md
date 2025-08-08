# DevOps Git Workflow Project :rocket:

## Overview

This project demonstrates a complete Git workflow from initialization to production release, following DevOps best practices. It includes branching strategies, pull requests, version tagging, and documentation.

## Steps Performed

1. Initialize Local Repository__
'''bash__
git init__
echo "DevOps Project" > README.md__
echo "node_modules/" > .gitignore__
git add . __
git commit -m "Initial commit"__
---
2. Push to GitHub__
git remote add origin https://github.com/sejalzend/github-devops-project.git__
git push -u origin main__
---
3. Create Branch Structure__
git checkout -b dev__
git push origin dev__
git checkout -b feature/login-button__
---
4. Make Feature Changes__
echo "Feature content" > feature.txt__
git add .__
git commit -m "Added a new feature file"__
git push origin feature/login-button__
---
5. Create Pull Request(PR)__
On GitHub: Compare & Pull Request feature/login-button --> dev__
Review and Merge PR__
---
6. Merge to Production__
Create PR: Compare dev --> main__
Use "Squash and Merge"__
---
7. Version Tagging__
git tag -a v1.0.0 -m "First stable release"__
git push origin v1.0.0
---


