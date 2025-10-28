# Git Setup Guide

## Step 1: Install Git (if needed)
Download and install Git from: https://git-scm.com/download/win

## Step 2: Configure Git (first time only)
```powershell
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

## Step 3: Initialize Repository
```powershell
cd "c:\Users\user\Downloads\PowerHealthViz"
git init
git add .
git commit -m "Initial commit: Power BI Healthcare Analysis project"
```

## Step 4: Create GitHub Repository
1. Go to https://github.com/new
2. Repository name: `PowerHealthViz` (or your preferred name)
3. Description: "Power BI Healthcare Data Analysis and Visualization"
4. Keep it Public (to showcase)
5. **Do NOT** initialize with README (we already have one)
6. Click "Create repository"

## Step 5: Push to GitHub
Replace `YOUR_USERNAME` with your GitHub username:

```powershell
git remote add origin https://github.com/YOUR_USERNAME/PowerHealthViz.git
git branch -M main
git push -u origin main
```

## Alternative: Using GitHub CLI
```powershell
gh repo create PowerHealthViz --public --source=. --remote=origin --push
```

---
**Note:** After setup, you can delete this file from the repository.
