# ARJ Tech Build - Vercel Deployment

This is a production-ready build for ARJ Tech website with links to Nexus AI and Gym Manager products.

## 📋 Project Structure

```
arj-tech-build/
├── dist/                    # Production build files
│   ├── index.html          # Main HTML file
│   ├── robots.txt          # SEO robots configuration
│   ├── assets/
│   │   ├── index.js        # Main JavaScript
│   │   └── index.css       # Stylesheet
│   └── [favicons & images] # Static assets
├── vercel.json             # Vercel configuration
├── .vercelignore           # Files to ignore in deployment
├── package.json            # Project metadata
└── README.md               # This file
```

## 🔗 Product URLs

The build currently contains these product URLs:

- **Nexus AI**: `https://nexus-two-beta-50.vercel.app/`
- **Gym Manager**: `https://gymflowvercel.vercel.app/`

### Updating URLs

To change the product URLs, edit `/dist/assets/index.js`:

```javascript
const NEXUS_URL = "https://your-nexus-url.com/";
const GYMFLOW_URL = "https://your-gymflow-url.com/";
```

## 🚀 Deployment to Vercel

### Option 1: Using Vercel CLI (Recommended)

```bash
# Install Vercel CLI globally
npm install -g vercel

# Navigate to the project directory
cd arj-tech-build

# Deploy to Vercel
vercel --prod
```

### Option 2: Using GitHub Integration

1. Push this folder to a GitHub repository
2. Go to [Vercel Dashboard](https://vercel.com/dashboard)
3. Click "Add New Project"
4. Select your GitHub repository
5. Vercel will auto-detect the configuration
6. Click "Deploy"

### Option 3: Manual Upload

1. Go to [Vercel Dashboard](https://vercel.com)
2. Click "Add New Project"
3. Select "Other" (do not connect to Git)
4. Upload the `dist` folder as your build output
5. Configure:
   - **Build Command**: `echo 'Build complete'`
   - **Output Directory**: `dist`

## 📝 Configuration

### vercel.json

The `vercel.json` file contains:
- **Rewrites**: Routes all requests to `index.html` for SPA support
- **Headers**: Caching rules for assets and pages
- **buildCommand**: Simple pass-through (pre-built)

### Environment Variables

No environment variables are required for basic deployment.

## 🔒 Security & Performance

- ✅ Caching headers configured for optimal performance
- ✅ Immutable asset caching (1 year)
- ✅ Page caching (1 hour)
- ✅ robots.txt configured for search engines
- ✅ Mobile-responsive design
- ✅ SEO meta tags included

## 📱 Features

- Modern, responsive design
- Product showcase with hover effects
- Direct links to Nexus AI and Gym Manager
- Professional styling with gradient backgrounds
- Mobile-optimized layout

## 🎨 Customization

### Styling

Edit `/dist/assets/index.css` to customize:
- Colors (currently using blue gradient: `#6496ff` to `#4070ff`)
- Fonts and typography
- Layout and spacing
- Animations and transitions

### Content

Edit `/dist/assets/index.js` to modify:
- Product names and descriptions
- Features list
- Links and URLs
- Page content

## 📊 Analytics & Monitoring

After deployment, you can:
1. View analytics in Vercel Dashboard
2. Check performance metrics
3. Monitor error logs
4. Track deployments and rollbacks

## 🆘 Troubleshooting

**Q: Website shows blank page?**
- Check browser console for errors
- Verify `dist/assets/index.js` is loading
- Ensure HTML file is at the root

**Q: URLs not updating?**
- Clear browser cache (Ctrl+Shift+Del)
- Rebuild and redeploy
- Check JavaScript console for errors

**Q: Slow performance?**
- Check Vercel Analytics
- Verify caching headers
- Optimize image sizes

## 📞 Support

For issues or questions about deployment, refer to:
- [Vercel Documentation](https://vercel.com/docs)
- [ARJ Tech](https://arj-tech.com)

---

**Version**: 1.0.0  
**Last Updated**: March 2024
