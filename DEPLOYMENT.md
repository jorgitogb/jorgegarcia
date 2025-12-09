# GitHub Pages Deployment Guide

This guide will help you deploy your personal landing page to GitHub Pages.

## Prerequisites

- GitHub account
- Git installed locally
- Repository already initialized (✓ Complete)

## Deployment Steps

### 1. Commit Your Changes

```bash
# Add all files
git add .

# Commit with a message
git commit -m "Add personal landing page with GitHub Pages deployment"

# Push to GitHub
git push origin master
```

### 2. Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/jorgitogb/jorgegarcia`
2. Click on **Settings** (top menu)
3. In the left sidebar, click **Pages**
4. Under **Source**, select:
   - Source: **GitHub Actions**
5. The workflow will automatically deploy your site

### 3. Wait for Deployment

- Go to the **Actions** tab in your repository
- You'll see the "Deploy to GitHub Pages" workflow running
- Wait for it to complete (usually 1-2 minutes)
- Once complete, your site will be live!

## Your Site URL

After deployment, your site will be available at:

**https://jorgitogb.github.io/jorgegarcia/**

## Configuration Details

### Astro Configuration
The `astro.config.mjs` has been updated with:
- `site`: Your GitHub Pages URL
- `base`: Repository name for proper asset paths

### GitHub Actions Workflow
Located at `.github/workflows/deploy.yml`:
- Triggers on push to `master` branch
- Builds the Astro site
- Deploys to GitHub Pages automatically

## Troubleshooting

### If the workflow fails:

1. **Check Actions tab** for error messages
2. **Verify Node version**: The workflow uses Node 18
3. **Check build locally**: Run `npm run build` to ensure it works

### If assets don't load:

- Verify the `base` path in `astro.config.mjs` matches your repository name
- Clear browser cache and hard refresh (Ctrl+Shift+R)

### If you need to redeploy:

```bash
# Make changes to your code
git add .
git commit -m "Update landing page"
git push origin master
```

The workflow will automatically redeploy on every push to master.

## Manual Deployment (Alternative)

If you prefer to deploy manually without GitHub Actions:

```bash
# Build the site
npm run build

# The dist/ folder contains your built site
# You can deploy this folder to any static hosting service
```

## Next Steps

1. ✅ Commit and push your changes
2. ✅ Enable GitHub Pages in repository settings
3. ✅ Wait for the workflow to complete
4. ✅ Visit your live site!
5. 🎉 Share your new personal landing page!

## Updating Your Site

To update your site in the future:

1. Make changes to your code
2. Commit: `git commit -am "Your update message"`
3. Push: `git push origin master`
4. GitHub Actions will automatically rebuild and redeploy

---

**Ready to deploy?** Run the commands in Step 1 above!
