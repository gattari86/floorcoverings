# Deployment Guide - FCI Diagnostic Report

## Quick Start (3 Steps)

### Step 1: Push to GitHub

```bash
cd fci-report-package

# Initialize git (if not already done)
git init

# Add all files
git add .

# Create initial commit
git commit -m "Add FCI diagnostic report for Reinel Solano"

# Add remote (use your GitHub URL)
git remote add origin https://github.com/gattari86/floorcoverings.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

### Step 2: Connect to Vercel

1. **Go to Vercel**: Visit [vercel.com](https://vercel.com)
2. **Sign in** with GitHub (or create account)
3. **Click "New Project"**
4. **Select your GitHub repository** (`floorcoverings`)
5. **Click "Import"** - Vercel will auto-detect settings
6. **Click "Deploy"** - Will be live in 30-60 seconds

### Step 3: Share the Live Link

Your report will be live at:
```
https://floorcoverings.vercel.app
```

(Vercel will show you the exact URL after deployment)

---

## Detailed Step-by-Step Instructions

### Prerequisites

- GitHub account (free at github.com)
- Vercel account (free at vercel.com)
- Git installed on your computer

### Full Deployment Process

#### 1. Prepare Your Local Repository

```bash
# Navigate to the report directory
cd /Users/ricardogattas-moras/fci-report-package

# Check git status
git status

# You should see:
# - index.html
# - vercel.json
# - package.json
# - .gitignore
# - README.md
# - DEPLOYMENT_GUIDE.md
```

#### 2. Create GitHub Repository

If your GitHub repository doesn't exist yet:

1. Go to [github.com/new](https://github.com/new)
2. Name: `floorcoverings`
3. Description: "FCI Houston Heights - Diagnostic Report"
4. Choose "Public" or "Private"
5. **Don't** initialize with README (we have one)
6. Click "Create repository"

#### 3. Push Code to GitHub

```bash
# Add all files to git
git add .

# Create commit
git commit -m "Add FCI diagnostic report by Poppy Marketing"

# Add the remote repository
git remote add origin https://github.com/gattari86/floorcoverings.git

# Set branch to main
git branch -M main

# Push to GitHub
git push -u origin main

# Verify it worked
git log --oneline
# Should show your commit
```

#### 4. Deploy to Vercel

**Option A: Web Interface (Easiest)**

1. Go to [vercel.com](https://vercel.com)
2. Click "New Project"
3. Click "Import Git Repository"
4. Paste: `https://github.com/gattari86/floorcoverings`
5. Click "Import"
6. Vercel auto-detects your setup
7. Click "Deploy"
8. Wait 30-60 seconds for deployment

**Option B: CLI (Command Line)**

```bash
# Install Vercel CLI
npm install -g vercel

# Deploy from your project directory
vercel

# Follow the prompts:
# - Set project name: "floorcoverings"
# - Confirm deployment directory
# - Approve deployment

# Your site will be live at: https://floorcoverings.vercel.app
```

---

## Verification Checklist

After deployment, verify everything works:

- [ ] Site loads without errors
- [ ] All sections visible and properly styled
- [ ] Navigation links scroll smoothly
- [ ] Mobile responsive (test on phone)
- [ ] Colors display correctly
- [ ] Print preview looks good (Ctrl+P or Cmd+P)
- [ ] Images/graphics render properly
- [ ] No console errors (F12 → Console tab)

---

## Making Updates

After your initial deployment, updating is simple:

```bash
# Make changes to files locally
# (e.g., edit index.html)

# Add changes
git add .

# Commit
git commit -m "Update report content"

# Push to GitHub
git push

# Vercel auto-deploys!
# Your live site updates automatically
```

---

## Custom Domain (Optional)

To use a custom domain (e.g., `fci-report.yourdomain.com`):

1. Go to your Vercel project dashboard
2. Settings → Domains
3. Add your custom domain
4. Follow DNS configuration steps
5. Takes 5-10 minutes to propagate

---

## Troubleshooting

### "Repository not found"
- Make sure GitHub repo is public (if using public link)
- Verify URL is correct: `https://github.com/gattari86/floorcoverings`

### "Deployment failed"
- Check `.gitignore` - make sure you're not ignoring necessary files
- Verify `index.html` exists in the root directory
- Check `vercel.json` syntax (valid JSON)

### "404 on custom domain"
- DNS changes take 5-10 minutes to propagate
- Try clearing browser cache
- Check Vercel domain settings

### "Site looks wrong"
- Clear browser cache (Ctrl+Shift+Del or Cmd+Shift+Del)
- Try incognito/private window
- Check that CSS is loaded (F12 → Network tab)

---

## Security & Best Practices

✅ **Report is read-only** - No forms, no data collection
✅ **No sensitive data** - Public diagnostic information only
✅ **HTTPS enabled** - Vercel auto-enables HTTPS
✅ **CDN-delivered** - Fast global distribution
✅ **Auto-updates** - Changes push automatically

---

## Sharing Your Report

After deployment, share the live link:

```
https://floorcoverings.vercel.app
```

Or with a custom message:

```
"Floor Coverings International Houston Heights
Comprehensive Diagnostic Report

Prepared by: Poppy Marketing and Consulting

View the full report: https://floorcoverings.vercel.app"
```

---

## Questions?

Contact Poppy Marketing and Consulting:
- **Email**: hello@poppymarketingandconsulting.com
- **Website**: poppymarketingandconsulting.com
