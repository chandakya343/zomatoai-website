# 🚀 GitHub Pages Deployment Guide

## Files to Upload

Upload **ONLY** these 4 files to GitHub:

```
presentation_website/
├── index.html    ✅ Main presentation page
├── styles.css    ✅ All styling
├── script.js     ✅ Animations and interactions
└── README.md     ✅ Documentation
```

**DO NOT UPLOAD:**
- ❌ Python files (.py) - Won't run on GitHub Pages
- ❌ .env file - Contains API key!
- ❌ Database files (.csv, .json)
- ❌ Any files outside presentation_website/

---

## Quick Deployment Steps

### Option 1: GitHub Web Interface (Easiest)

1. **Create Repository**
   - Go to: https://github.com/new
   - Name: `zomatoai-presentation`
   - Public ✓
   - Create repository

2. **Upload Files**
   - Click "uploading an existing file"
   - Drag these 4 files: `index.html`, `styles.css`, `script.js`, `README.md`
   - Commit message: "ZomatoAI presentation website"
   - Commit changes

3. **Enable GitHub Pages**
   - Settings → Pages (left sidebar)
   - Source: "main" branch
   - Save
   - Wait ~1 minute

4. **Get Your URL**
   - `https://YOUR_USERNAME.github.io/zomatoai-presentation/`

---

### Option 2: Command Line

```bash
# Navigate to presentation folder
cd /Users/aryanchandak/projects/ZomatoAI_Manager/presentation_website

# Initialize git
git init

# Add ONLY the website files
git add index.html styles.css script.js README.md

# Commit
git commit -m "ZomatoAI presentation website"

# Create repo on GitHub first, then:
git remote add origin https://github.com/YOUR_USERNAME/zomatoai-presentation.git
git branch -M main
git push -u origin main

# Enable Pages in GitHub settings
```

---

## Verification Checklist

Before deploying:
- [ ] Test `index.html` locally (open in browser)
- [ ] All animations work
- [ ] Responsive on mobile (resize browser)
- [ ] No API keys in files
- [ ] Content is proofread

After deploying:
- [ ] Site loads at GitHub Pages URL
- [ ] All styles applied correctly
- [ ] Animations work
- [ ] Scroll is smooth
- [ ] All sections visible

---

## Sharing with Zomato AI PM

**Email Template:**

```
Subject: ZomatoAI - AI PM Application Demo

Hi [PM Name],

I've built ZomatoAI - an AI-powered solution to choice paralysis 
in food ordering.

🌐 Interactive Presentation: 
   https://YOUR_USERNAME.github.io/zomatoai-presentation/

The presentation explains:
• The problem (choice paralysis with 1000+ dishes)
• My solution (multi-agent AI system)
• Technical architecture
• Why tunability is key
• Future improvements

I've also built a working Streamlit demo with:
✓ Multi-agent orchestration
✓ Smart memory management  
✓ Live recommendations
✓ Complete source code

Happy to share the code and demo it live!

Best regards,
Aryan Chandak
```

---

## Two-Repository Strategy (Recommended)

### Repository 1: Presentation (PUBLIC)
- **Name:** `zomatoai-presentation`
- **Contents:** HTML/CSS/JS only
- **Purpose:** Easy to share, professional presentation
- **GitHub Pages:** Enabled
- **URL:** Share this with everyone

### Repository 2: Full Code (PRIVATE - Optional)
- **Name:** `zomatoai-manager`
- **Contents:** Complete Python app, agents, memory system
- **Purpose:** Show technical depth to interested parties
- **Access:** Grant access to Zomato team only
- **No Pages:** Just code repository

**Benefits:**
- Presentation is publicly viewable
- Code is protected until you're ready to share
- Professional separation of concerns

---

## Common Issues & Solutions

**Issue:** "GitHub Pages shows 404"
- **Solution:** Make sure `index.html` is in the root of your repo
- **Solution:** Check that Pages is enabled in Settings

**Issue:** "Styles not loading"
- **Solution:** Check that `styles.css` and `script.js` are in same folder as `index.html`
- **Solution:** Verify file names are exact (case-sensitive)

**Issue:** "Animations not working"
- **Solution:** Give it a minute to fully deploy
- **Solution:** Hard refresh (Cmd+Shift+R or Ctrl+Shift+F5)

---

## Quick Deploy Checklist

```bash
# 1. Are you in the right folder?
cd /Users/aryanchandak/projects/ZomatoAI_Manager/presentation_website
pwd  # Should show: .../presentation_website

# 2. Do you have all files?
ls
# Should see: index.html, styles.css, script.js, README.md

# 3. Test locally
open index.html
# Verify everything works

# 4. Create GitHub repo (via website)
# Visit: https://github.com/new

# 5. Upload files (drag and drop on GitHub)
# Or use git commands above

# 6. Enable Pages (Settings → Pages → main branch)

# 7. Get your URL and share!
# https://YOUR_USERNAME.github.io/REPO_NAME/
```

---

**That's it! Just 4 files to upload.** 🎉

The presentation is a static website (HTML/CSS/JS), so it's perfect for GitHub Pages. The Python app stays on your local machine for live demos.

---

**Ready to deploy?** Just upload those 4 files and enable Pages! 🚀

