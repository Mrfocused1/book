# Bood Website - Deployment Guide

## Step-by-Step Deployment to Vercel via GitHub

### Prerequisites

- GitHub account
- Vercel account (free at [vercel.com](https://vercel.com))
- Git installed on your machine

### Step 1: Initialize Git Repository

```bash
cd "/Users/paulbridges/bood uk sample"
git init
```

### Step 2: Create GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Name your repository: `bood-website` (or your preferred name)
3. Keep it Public or Private (your choice)
4. **DO NOT** initialize with README, .gitignore, or license (we already have these)
5. Click "Create repository"

### Step 3: Add Files and Commit

```bash
# Add all files
git add .

# Commit
git commit -m "Initial commit: Bood website with responsive design and animations"

# Set main branch
git branch -M main
```

### Step 4: Connect to GitHub

Replace `YOUR_USERNAME` with your GitHub username and `YOUR_REPO_NAME` with your repository name:

```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

If prompted, enter your GitHub credentials or use a personal access token.

### Step 5: Deploy to Vercel

#### Option A: Deploy via Vercel Website (Recommended)

1. Go to [vercel.com](https://vercel.com) and sign in
2. Click "Add New Project" or "New Project"
3. Click "Import Git Repository"
4. Select your GitHub repository (`bood-website`)
5. Configure project:
   - **Project Name**: `bood` (or your preferred name)
   - **Framework Preset**: Other (leave as is)
   - **Root Directory**: `./` (default)
   - **Build Settings**: Leave blank (static HTML site)
6. Click "Deploy"

Your site will build and deploy in ~30 seconds!

#### Option B: Deploy via Vercel CLI

```bash
# Install Vercel CLI globally
npm install -g vercel

# Login to Vercel
vercel login

# Deploy
vercel

# Follow the prompts:
# - Set up and deploy? Yes
# - Which scope? (select your account)
# - Link to existing project? No
# - Project name? bood-website
# - Directory? ./
# - Auto-detected settings? Yes
```

### Step 6: View Your Live Site

After deployment, Vercel will provide you with:
- **Production URL**: `https://your-project-name.vercel.app`
- **Deployment URL**: Unique URL for this specific deployment

Visit your production URL to see your live site!

### Step 7: Set Up Custom Domain (Optional)

1. Go to your project dashboard on Vercel
2. Click "Settings" → "Domains"
3. Add your custom domain (e.g., `bood.com`)
4. Follow Vercel's instructions to update your DNS records
5. Wait for DNS propagation (~24-48 hours)

## Continuous Deployment

Once connected to GitHub, Vercel automatically:
- **Deploys** every push to the `main` branch to production
- **Creates preview deployments** for pull requests
- **Runs builds** and shows deploy status

To update your site:
```bash
# Make your changes
git add .
git commit -m "Description of changes"
git push origin main
```

Vercel will automatically deploy your changes in ~30 seconds!

## Environment Configuration

Your site is configured with:
- ✅ Responsive design (mobile-optimized)
- ✅ SEO meta tags
- ✅ Security headers
- ✅ Static file serving
- ✅ Custom 404 handling
- ✅ Fast CDN distribution

## Troubleshooting

### Build Fails
- Check that all HTML files are valid
- Ensure external resources (fonts, scripts) are accessible
- Review build logs in Vercel dashboard

### Site Not Loading
- Clear browser cache
- Check Vercel deployment status
- Verify domain settings (if using custom domain)

### Git Push Errors
- Ensure remote is correctly set: `git remote -v`
- Check GitHub credentials/token
- Try: `git push -f origin main` (use force carefully)

## Performance Optimization

Your site already includes:
- Lazy-loaded animations
- Optimized images
- CDN delivery
- Minimal JavaScript

For further optimization:
- Compress images to WebP format
- Add preload hints for critical resources
- Consider implementing service workers for offline support

## Monitoring

Monitor your site's performance:
- **Vercel Analytics**: Built-in traffic analytics
- **Lighthouse**: Run audits in Chrome DevTools
- **PageSpeed Insights**: Check performance scores

## Support

- **Vercel Docs**: [vercel.com/docs](https://vercel.com/docs)
- **GitHub Docs**: [docs.github.com](https://docs.github.com)
- **Vercel Support**: Contact via dashboard

---

## Quick Reference Commands

```bash
# Clone the repo (if starting from scratch)
git clone https://github.com/YOUR_USERNAME/bood-website.git
cd bood-website

# Make changes and deploy
git add .
git commit -m "Your message"
git push origin main

# Deploy via CLI
vercel --prod

# Check deployment status
vercel ls

# View logs
vercel logs
```

---

**Your Bood website is now live and ready for the world! 🌊✨**
