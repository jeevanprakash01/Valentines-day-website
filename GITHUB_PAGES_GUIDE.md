# GitHub Pages Hosting Guide

## Step-by-Step Instructions

### Step 1: Create a GitHub Account (if you don't have one)
- Go to https://github.com
- Sign up for a free account

### Step 2: Create a New Repository
1. Click the "+" icon in the top right corner
2. Select "New repository"
3. Name your repository (e.g., "valentine-website" or "moonshine")
4. Make it **Public** (required for free GitHub Pages)
5. **DO NOT** initialize with README, .gitignore, or license (we already have files)
6. Click "Create repository"

### Step 3: Initialize Git and Push Your Code

Open PowerShell/Terminal in your project folder and run:

```powershell
# Navigate to your project folder
cd "C:\Users\HP\Downloads\moonshine-main\moonshine-main"

# Initialize git repository
git init

# Add all files
git add .

# Commit the files
git commit -m "Initial commit - Valentine website"

# Add your GitHub repository (replace YOUR_USERNAME and YOUR_REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Important:** Replace `YOUR_USERNAME` with your GitHub username and `YOUR_REPO_NAME` with your repository name.

### Step 4: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click on **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under **Source**, select:
   - Branch: **main**
   - Folder: **/ (root)**
5. Click **Save**

### Step 5: Access Your Website
- GitHub will provide you a URL like: `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`
- It may take 1-2 minutes to deploy
- You'll see a green checkmark when it's ready

## Quick Commands Reference

```powershell
# If you need to update your website later:
git add .
git commit -m "Update website"
git push
```

## Troubleshooting

- **404 Error**: Wait 2-3 minutes after enabling Pages, it takes time to deploy
- **Styles not loading**: Make sure all paths are relative (they are in your code ✅)
- **Images not showing**: Check that image files are in the correct folders
- **Can't push**: Make sure you're authenticated with GitHub (use GitHub Desktop or configure Git credentials)

## Your Website URL Format
Once deployed, your site will be at:
`https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`

For example, if your username is `johndoe` and repo is `valentine-website`:
`https://johndoe.github.io/valentine-website/`
