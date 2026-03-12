# Najashi Abdullah - Visual Resume

A minimalist, award-winning visual resume combining Japanese aesthetics with Apple's precision and modern web interactions.

## 🎨 Design Philosophy

This portfolio embodies:
- **Japanese Minimalism**: Clean lines, generous white space, subtle grain texture
- **Apple Precision**: Sophisticated typography, smooth interactions, attention to detail
- **Awwwards Quality**: Scroll animations, micro-interactions, elegant transitions

## 🚀 Quick Deploy to Vercel

### Method 1: One-Click Deploy (Recommended)

1. **Push to GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Visual resume"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/najashi-portfolio.git
   git push -u origin main
   ```

2. **Deploy to Vercel**:
   - Go to [vercel.com](https://vercel.com)
   - Sign in with GitHub
   - Click "New Project"
   - Import your GitHub repository
   - Click "Deploy" (Vercel auto-detects the static HTML)
   - Your site will be live at `https://your-project.vercel.app`

3. **Add Custom Domain** (najashi.abdullah):
   - In Vercel dashboard, go to your project
   - Click "Settings" → "Domains"
   - Add your custom domain: `najashi.abdullah`
   - Follow Vercel's DNS configuration instructions
   - Update your domain registrar's DNS records:
     - Add CNAME record pointing to `cname.vercel-dns.com`
     - Or add A record pointing to Vercel's IP

### Method 2: Vercel CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Follow prompts to link to your account
# Your site will be deployed instantly
```

## 📱 QR Code Setup

Once deployed, generate a QR code for your live URL:

1. **Using Online Tools**:
   - Visit [qr-code-generator.com](https://www.qr-code-generator.com/)
   - Enter your Vercel URL (or custom domain)
   - Download as high-res PNG or SVG
   - Print on business cards, resume, or display digitally

2. **Using CLI** (Node.js):
   ```bash
   npx qrcode-terminal https://your-site.vercel.app
   ```

## 🛠️ Local Development

```bash
# Option 1: Python HTTP Server
python3 -m http.server 8000

# Option 2: Node.js HTTP Server
npx http-server -p 8000

# Option 3: PHP Server
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## 📂 Project Structure

```
najashi-portfolio/
├── index.html          # Main portfolio page
├── package.json        # Project metadata
├── README.md          # This file
├── .gitignore         # Git ignore rules
└── vercel.json        # Vercel configuration
```

## 🎯 Features

- **Responsive Design**: Perfect on mobile, tablet, and desktop
- **Smooth Scrolling**: Elegant navigation between sections
- **Scroll Animations**: Content reveals as you scroll
- **Sticky Navigation**: Always accessible menu
- **Performance Optimized**: Fast loading, minimal dependencies
- **SEO Ready**: Semantic HTML, meta tags
- **Accessibility**: WCAG compliant

## 🔧 Customization

### Colors
Edit CSS variables in `index.html`:
```css
:root {
    --color-ink: #1a1a1a;      /* Text color */
    --color-paper: #fafaf8;    /* Background */
    --color-accent: #d64545;   /* Accent color */
    --color-muted: #6b6b6b;    /* Secondary text */
    --color-border: #e8e8e5;   /* Borders */
}
```

### Typography
Update Google Fonts link and CSS variables:
```css
--font-display: 'Sora', -apple-system, sans-serif;
--font-body: 'Crimson Pro', Georgia, serif;
```

### Content
Update the `experiences` and `skills` arrays in the React component.

## 🌐 Domain Setup

### Purchasing najashi.abdullah Domain

Since `.abdullah` is not a standard TLD, you have two options:

1. **Use a subdomain**: `najashi.yourdomain.com`
2. **Purchase similar domain**: 
   - `najashi.com`
   - `najashiabdullah.com`
   - `najashi.dev`
   - `najashi.me`

### DNS Configuration for Custom Domain

After purchasing, configure DNS in your domain registrar:

**For Vercel**:
- Type: `CNAME`
- Name: `@` (or subdomain)
- Value: `cname.vercel-dns.com`

Or use A record:
- Type: `A`
- Name: `@`
- Value: `76.76.21.21`

## 📊 Analytics Setup (Optional)

Add Google Analytics or Vercel Analytics:

```html
<!-- Add before </head> -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR_GA_ID');
</script>
```

Or enable Vercel Analytics in your dashboard (one click).

## 🐛 Troubleshooting

### Site not loading?
- Check Vercel deployment logs
- Ensure `index.html` is in root directory
- Clear browser cache

### Animations not working?
- Ensure JavaScript is enabled
- Check browser console for errors
- Try different browser

### Custom domain not working?
- Wait 24-48 hours for DNS propagation
- Verify DNS records with `dig` or `nslookup`
- Check Vercel domain settings

## 📞 Support

For issues or questions:
- Email: Najashi.abdullah@gmail.com
- LinkedIn: [linkedin.com/in/najashi-abdullah](https://linkedin.com/in/najashi-abdullah)

## 📄 License

MIT License - Feel free to use this as a template for your own portfolio!

---

**Built with intention. Designed for impact.**
