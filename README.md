# ARJ Tech - Render.com Deployment

A modern, production-ready website for ARJ Tech with Nexus AI and Gym Manager product links.

## 🚀 Quick Deploy

1. **Upload to GitHub**
   - Go to your GitHub repo
   - Upload all files from this build

2. **Deploy to Render**
   - Go to render.com
   - Connect your GitHub repo
   - Render auto-deploys from render.yaml

3. **Done!** 🎉
   - Your site is live at `https://arj-tech-xxxx.onrender.com`

[See RENDER-QUICK-START.txt for detailed steps]

## 📦 What's Included

- **dist/** - Production static files
  - index.html - Main page
  - assets/index.js - JavaScript with product URLs
  - assets/index.css - Professional styling
  - favicon.png, favicon.ico - Logos
  - robots.txt - SEO configuration

- **render.yaml** - Render deployment config
- **package.json** - Project metadata
- **.renderignore** - Files to ignore

## 🔗 Product Links

- Nexus AI: https://nexus-two-beta-50.vercel.app/
- Gym Manager: https://gymflowvercel.vercel.app/

## 📝 Edit URLs (Optional)

Edit `dist/assets/index.js` lines 8-9:

```javascript
const NEXUS_URL = "your-url-here";
const GYMFLOW_URL = "your-url-here";
```

Then push to GitHub - Render auto-rebuilds!

## 🎨 Features

✓ Modern dark theme with gradients  
✓ Fully responsive design  
✓ Smooth animations  
✓ SEO optimized  
✓ Mobile-friendly  
✓ No dependencies  
✓ Production ready  

## 🌐 Add Custom Domain

1. In Render dashboard → Custom Domain
2. Add your domain
3. Update DNS records (CNAME)
4. Wait 24 hours for DNS propagation
5. HTTPS automatic

## 📚 Documentation

- **RENDER-QUICK-START.txt** - 5-minute deployment guide
- **RENDER-DEPLOYMENT-GUIDE.md** - Complete reference
- https://render.com/docs - Official Render docs

## 🆘 Troubleshooting

**Build fails?**
- Check render.yaml exists at repo root
- Verify dist/ folder has all files
- Check Render build logs

**Page blank?**
- Hard refresh (Ctrl+Shift+R)
- Wait 2 minutes
- Check browser console (F12)

**Need help?**
- https://support.render.com
- https://render.com/docs

## 📊 Monitoring

In Render dashboard:
- View real-time logs
- Check memory/CPU usage
- See deployment history
- Manual redeploy button

## 🔄 Auto-Updates

Every git push to GitHub:
1. Render detects change
2. Auto-rebuilds (1-2 min)
3. Auto-deploys
4. Changes live!

## ✅ Before Deploying

Edit if needed:
- Product URLs (dist/assets/index.js)
- Company email/phone (dist/assets/index.js)
- Colors (dist/assets/index.css)

Push to GitHub, Render auto-rebuilds!

## 📄 License

MIT License

---

**Version:** 1.0.0  
**Platform:** Render.com  
**Status:** Production Ready ✅
