╔═══════════════════════════════════════════════════════════════════════════════╗
║          🚀 RENDER.COM DEPLOYMENT GUIDE - ARJ TECH BUILD 🚀                  ║
╚═══════════════════════════════════════════════════════════════════════════════╝

📋 TABLE OF CONTENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. What You Have
2. Prerequisites
3. Step-by-Step Deployment
4. Verify Deployment
5. Custom Domain Setup
6. Troubleshooting


📦 WHAT YOU HAVE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✅ Complete Render.com Build Package:
   • dist/ folder - Production static files
   • render.yaml - Render configuration
   • package.json - Project metadata
   • .renderignore - Files to ignore

✅ What's Included:
   • index.html - Main page
   • assets/index.js - JavaScript (with product URLs)
   • assets/index.css - Professional styling
   • favicon.png & favicon.ico - Logos
   • robots.txt - SEO configuration

✅ Product URLs (Already Configured):
   • Nexus AI: https://nexus-two-beta-50.vercel.app/
   • Gym Manager: https://gymflowvercel.vercel.app/


✅ PREREQUISITES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

You need:
1. GitHub account (free: github.com)
2. Render.com account (free: render.com)
3. Git installed on your computer (optional but recommended)

That's it! No credit card required for free tier.


🚀 STEP-BY-STEP DEPLOYMENT (EASIEST METHOD)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

STEP 1: PREPARE YOUR GITHUB REPOSITORY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Option A: If you have existing GitHub repo (Ashutosh931998/ARJ-Tech)

1. Go to: github.com/Ashutosh931998/ARJ-Tech

2. Click "Add file" → "Upload files"

3. Upload these files from the render build:
   ✓ render.yaml
   ✓ package.json
   ✓ .renderignore
   ✓ dist/ folder (all files inside)

4. Commit with message: "Add Render.com deployment files"

5. Verify files are in your repo root


Option B: Create new repository

1. Go to: github.com/new

2. Create repository named "arj-tech-render"

3. Clone it locally:
   git clone https://github.com/YOUR_USERNAME/arj-tech-render.git
   cd arj-tech-render

4. Copy all files from render build into the folder

5. Push to GitHub:
   git add .
   git commit -m "Initial commit: Render deployment"
   git push origin main


STEP 2: CONNECT GITHUB TO RENDER.COM
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. Go to: render.com

2. Click "Sign up" or "Log in"
   (Use GitHub login for easiest setup)

3. Click "Connect account" → "GitHub"
   (Or "New +" button)

4. Click "Create New" → "Web Service"

5. Select "Connect a repository"

6. Search for your repository:
   • arj-tech-render OR
   • ARJ-Tech (if using existing)

7. Click "Connect"


STEP 3: CONFIGURE DEPLOYMENT SETTINGS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Render will automatically detect render.yaml, but verify:

1. Name: arj-tech (or your preferred name)

2. Environment: Node (or Static Site)

3. Build Command: echo "Pre-built static site"

4. Start Command: (leave empty for static)

5. Publish directory: ./dist

6. Plan: FREE (Recommended to start)

7. Click "Create Web Service"


STEP 4: WAIT FOR DEPLOYMENT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Render will now:
1. Clone your GitHub repo
2. Build the project (1-2 minutes)
3. Deploy to their servers
4. Assign you a free domain

Watch the build logs for progress.
It should finish with green "✓ Deployed" message.


🎉 YOUR SITE IS LIVE!
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

After deployment, Render gives you a FREE URL:
   https://arj-tech-xxxx.onrender.com

(The exact subdomain depends on your project name)

Share this URL with anyone!


✅ VERIFY DEPLOYMENT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

1. Click your Render project URL

2. Check these things load:
   ✓ Page title: "ARJ Tech — Digital Products That Matter"
   ✓ Logo and header visible
   ✓ Product cards displaying
   ✓ Images loading (placeholder.svg)
   ✓ Styling looks correct (gradients, colors)
   ✓ Links work

3. Click product links to verify they direct to:
   ✓ Nexus AI
   ✓ Gym Manager

4. Test on mobile:
   ✓ Responsive design works
   ✓ Menu accessible
   ✓ Buttons clickable

5. Open DevTools (F12) → Console
   ✓ No red errors
   ✓ See "ARJ Tech - Render.com Build" message


🌐 ADD CUSTOM DOMAIN (OPTIONAL)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

If you have a custom domain (like arj-tech.com):

1. In Render dashboard, click your project

2. Go to "Settings" → "Custom Domain"

3. Add your domain name

4. Follow Render's instructions to update DNS:
   • Go to your domain registrar
   • Add CNAME record pointing to Render
   • Wait up to 24 hours for DNS to propagate

5. HTTPS is automatic ✅


🔄 UPDATE YOUR SITE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

To make changes:

1. Edit files locally or on GitHub

2. Update the product URLs in dist/assets/index.js:
   const NEXUS_URL = "https://your-new-url.com/";
   const GYMFLOW_URL = "https://your-new-url.com/";

3. Commit and push to GitHub:
   git add .
   git commit -m "Update product URLs"
   git push origin main

4. Render automatically rebuilds and deploys ✅
   (Watch the build in Render dashboard)

5. Your changes are live in 1-2 minutes!


📝 EDIT FILES BEFORE DEPLOYING
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Important: Change these if needed BEFORE deploying:

1. Product URLs (dist/assets/index.js - lines 7-8):
   const NEXUS_URL = "YOUR_URL_HERE";
   const GYMFLOW_URL = "YOUR_URL_HERE";

2. Company email (dist/assets/index.js - line 31):
   email: "your-email@company.com";

3. Company phone (dist/assets/index.js - line 32):
   phone: "+1 (555) YOUR-PHONE";


🆘 TROUBLESHOOTING
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

❌ PROBLEM: Build fails
✅ SOLUTION:
   1. Check render.yaml is in repo root
   2. Check dist/ folder exists with files
   3. Verify file names: index.html, index.js, index.css
   4. Check Render build logs for specific error
   5. Rebuild: Click "Manual deploy" in Render dashboard

❌ PROBLEM: Page shows 404 or blank
✅ SOLUTION:
   1. Verify publishPath is set to ./dist
   2. Check dist/index.html exists
   3. Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
   4. Clear browser cache
   5. Check Render logs

❌ PROBLEM: Styles not loading
✅ SOLUTION:
   1. Check dist/assets/index.css exists
   2. Hard refresh browser
   3. Check CSS file size (should be ~40KB)
   4. Open DevTools → Network tab → check CSS loads
   5. No HTTP errors should show

❌ PROBLEM: Images not showing
✅ SOLUTION:
   1. Verify favicon.png, favicon.ico, placeholder.svg in dist/
   2. Hard refresh browser
   3. Check file sizes are reasonable
   4. Open DevTools → Console → check for 404 errors

❌ PROBLEM: Product links don't work
✅ SOLUTION:
   1. Check URLs in dist/assets/index.js
   2. Verify URLs start with https://
   3. Test URLs in new browser tab
   4. Redeploy if you changed URLs

❌ PROBLEM: Site is very slow
✅ SOLUTION:
   1. First load might be slow (Render "spins down" free tier)
   2. Wait 1-2 minutes, then refresh
   3. Check Render dashboard for CPU/memory usage
   4. Upgrade to paid tier if needed


📊 MONITORING YOUR SITE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

In Render Dashboard, you can:
1. View real-time logs
2. Check memory/CPU usage
3. See deployment history
4. Manual redeploy
5. Configure environment variables
6. Set up alerts


📞 GETTING HELP
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Need help?
• Render Docs: https://render.com/docs
• GitHub Docs: https://docs.github.com
• Contact Render Support: https://support.render.com


═══════════════════════════════════════════════════════════════════════════════

✅ YOU'RE ALL SET!

Follow the steps above and your site will be live on Render.com in minutes!

═══════════════════════════════════════════════════════════════════════════════

Quick Summary:
1. Upload files to GitHub
2. Go to Render.com
3. Click "Create Web Service"
4. Connect your GitHub repo
5. Wait for deployment
6. Done! Your site is live 🎉

═══════════════════════════════════════════════════════════════════════════════
