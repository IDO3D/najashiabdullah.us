# 🚀 Quick Deployment Guide

## Step 1: Push to GitHub

```bash
# Initialize Git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Najashi Abdullah visual resume"

# Create main branch
git branch -M main

# Add your GitHub repository
git remote add origin https://github.com/YOUR_USERNAME/najashi-portfolio.git

# Push to GitHub
git push -u origin main
```

## Step 2: Deploy to Vercel

### Option A: Via Vercel Website (Easiest)
1. Go to https://vercel.com
2. Sign in with GitHub
3. Click "New Project"
4. Select your `najashi-portfolio` repository
5. Click "Deploy"
6. Done! Your site is live 🎉

### Option B: Via Vercel CLI
```bash
# Install Vercel CLI globally
npm install -g vercel

# Login to Vercel
vercel login

# Deploy
vercel

# Follow the prompts
```

## Step 3: Custom Domain Setup

1. In Vercel dashboard, go to your project
2. Click "Settings" → "Domains"
3. Click "Add Domain"
4. Enter your domain (e.g., `najashi.me`, `najashiabdullah.com`)
5. Follow DNS configuration instructions:

   **DNS Records to Add** (in your domain registrar):
   ```
   Type: CNAME
   Name: @
   Value: cname.vercel-dns.com
   ```
   
   Or use A record:
   ```
   Type: A
   Name: @
   Value: 76.76.21.21
   ```

6. Wait for DNS propagation (can take up to 48 hours, usually much faster)

## Step 4: Generate QR Code

Once your site is live:

1. Go to https://www.qr-code-generator.com/
2. Enter your live URL
3. Customize design (optional)
4. Download as PNG or SVG
5. Use on:
   - Business cards
   - Resume header
   - LinkedIn profile
   - Email signature
   - Presentations

## 🎯 Your Live URLs

After deployment, you'll have:
- **Vercel URL**: `https://najashi-portfolio.vercel.app`
- **Custom Domain**: `https://your-domain.com` (after setup)

## 📱 Test Your Site

Before sharing:
1. Test on mobile devices (QR code primary use case)
2. Test in different browsers (Chrome, Safari, Firefox)
3. Check load speed: https://pagespeed.web.dev/
4. Verify all links work
5. Test smooth scrolling

## 🔥 Pro Tips

- **Free SSL**: Vercel automatically provides HTTPS
- **Auto-deploys**: Every push to main branch auto-deploys
- **Preview URLs**: Every PR gets a preview URL
- **Analytics**: Enable Vercel Analytics for visitor insights
- **Performance**: Site scores 95+ on Lighthouse by default

## ❓ Need Help?

- Vercel Docs: https://vercel.com/docs
- GitHub Help: https://docs.github.com
- Contact: Najashi.abdullah@gmail.com

---

**Time to deploy: ~5 minutes**
**Cost: $0 (Vercel free tier)**
