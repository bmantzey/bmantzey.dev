# Brandon Mantzey - Portfolio Website

Professional portfolio showcasing 16+ years of iOS development expertise across financial services, wearables, and agriculture.

## 🚀 Quick Start

### 1. Add Your Images

Place the following images in the appropriate folders:

#### Required Images:

**`images/headshot.jpg`**
- Your professional photo (Black_Shirt_and_Tie.jpg)
- Rename to `headshot.jpg`
- Recommended size: 400x400px minimum
- Format: JPG

**`images/app-store/garmin-dive.jpg`**
- Screenshot from Garmin Dive App Store page
- Get from: https://apps.apple.com/us/app/garmin-dive/id1522633851
- Recommended size: 1170x2532px (iPhone screenshot)
- Format: JPG or PNG

**`images/app-store/schwab-mobile.jpg`**
- Screenshot from Schwab Mobile App Store page  
- Get from: https://apps.apple.com/us/app/schwab-mobile/id407954616
- Recommended size: 1170x2532px (iPhone screenshot)
- Format: JPG or PNG

**`images/app-store/fieldnet.jpg`**
- Screenshot from FieldNET Mobile App Store page
- Get from: https://apps.apple.com/us/app/fieldnet/id1288019945
- Recommended size: 1170x2532px (iPhone screenshot)
- Format: JPG or PNG

**`images/projects/transition-hub-mockup.png`**
- Generic iPhone mockup (placeholder provided)
- Optional: Replace with custom design
- Format: PNG

### 2. File Structure

```
portfolio/
├── index.html              # Main HTML file
├── styles.css              # All styling
├── script.js               # Interactive features
├── README.md              # This file
└── images/
    ├── headshot.jpg       # YOUR PHOTO HERE
    ├── app-store/
    │   ├── garmin-dive.jpg
    │   ├── schwab-mobile.jpg
    │   └── fieldnet.jpg
    └── projects/
        └── transition-hub-mockup.png
```

### 3. Local Testing

Open `index.html` in your browser to preview the site locally.

**Option A: Double-click** the file  
**Option B: Use a local server** (recommended for full functionality):

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (if you have http-server installed)
npx http-server
```

Then visit: `http://localhost:8000`

### 4. Deploy to GitHub Pages

#### Method 1: Repository Named `bmantzey.github.io`

1. Create new repository: `bmantzey.github.io`
2. Upload all files (maintain folder structure)
3. Site auto-publishes at: `https://bmantzey.github.io`

#### Method 2: Project Repository with Custom Domain

1. Create repository: `portfolio` (or any name)
2. Upload all files
3. Go to Settings → Pages
4. Source: Deploy from branch `main` (or `master`)
5. Folder: `/ (root)`
6. Save
7. Site publishes at: `https://bmantzey.github.io/portfolio`

#### Custom Domain Setup (bmantzey.dev or mantzey.com)

1. In repository Settings → Pages → Custom domain:
   - Enter: `bmantzey.dev` or `mantzey.com`
2. In your domain registrar (where you bought the domain):
   - Add DNS records:
     - Type: `A` 
     - Name: `@`
     - Value: 
       - `185.199.108.153`
       - `185.199.109.153`
       - `185.199.110.153`
       - `185.199.111.153`
   - If using `www` subdomain, also add:
     - Type: `CNAME`
     - Name: `www`
     - Value: `bmantzey.github.io`
3. Wait for DNS propagation (can take up to 24 hours)
4. Enable "Enforce HTTPS" in GitHub Pages settings

## 📝 Customization

### Update Resume Link

The resume link points to Firebase Storage:
```
https://firebasestorage.googleapis.com/v0/b/swiftfolio-4bb5b.appspot.com/o/Brandon_Mantzey_Resume.pdf?alt=media
```

This auto-updates when you push a new PDF to Firebase. No website changes needed!

### Modify Content

- **Hero section:** Edit `index.html` lines 31-43
- **Projects:** Edit `index.html` lines 47-165
- **Timeline:** Edit `index.html` lines 170-230
- **Skills:** Edit `index.html` lines 235-385
- **Contact:** Edit `index.html` lines 390-465

### Change Colors

Edit `styles.css` lines 14-21 (CSS variables):

```css
:root {
    --color-accent: #0071e3;        /* Main blue */
    --color-accent-hover: #0077ed;  /* Hover blue */
    /* ... etc */
}
```

### Modify Animations

Edit `styles.css` animations section (lines 600+) or `script.js` scroll reveal settings.

## 🎨 Features

✅ **Responsive Design** - Mobile, tablet, desktop optimized  
✅ **Smooth Scrolling** - Elegant navigation  
✅ **Interactive Projects** - Expandable project details  
✅ **Collapsible Skills** - Progressive disclosure  
✅ **Mobile Menu** - Hamburger navigation  
✅ **Scroll Animations** - Fade-in effects  
✅ **App Store Links** - Direct links to live apps  
✅ **GitHub Integration** - Link to repositories  
✅ **Firebase Resume** - Auto-updating resume link  
✅ **Accessibility** - Keyboard navigation, ARIA labels  
✅ **Performance** - Optimized loading, debounced scrolling  

## 🖼️ How to Get App Store Screenshots

1. Visit the App Store page on your Mac or iOS device
2. Right-click screenshot → "Save Image As..."
3. Or use browser inspector to download full-res images
4. Rename to match required filenames
5. Place in `images/app-store/` folder

**Example URLs:**
- Garmin Dive: https://apps.apple.com/us/app/garmin-dive/id1522633851
- FieldNET: https://apps.apple.com/us/app/fieldnet/id1288019945
- Schwab Mobile: https://apps.apple.com/us/app/schwab-mobile/id407954616

## 🔧 Troubleshooting

**Images not showing?**
- Check file names match exactly (case-sensitive)
- Verify files are in correct folders
- Check browser console for errors (F12)

**Mobile menu not working?**
- Ensure `script.js` is loading
- Check browser console for JavaScript errors

**Site not updating on GitHub Pages?**
- Changes can take 1-5 minutes to deploy
- Try hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
- Check GitHub Actions tab for build status

**Custom domain not working?**
- Verify DNS records are correct
- Wait 24 hours for DNS propagation
- Check domain registrar settings

## 📱 Browser Support

✅ Chrome (latest)  
✅ Firefox (latest)  
✅ Safari (latest)  
✅ Edge (latest)  
✅ Mobile Safari (iOS 12+)  
✅ Chrome Mobile (Android 5+)  

## 📄 License

© 2024 Brandon Mantzey. All rights reserved.

## 🤝 Need Help?

If you encounter issues:

1. Check browser console (F12) for errors
2. Verify all images are in correct locations
3. Test locally before deploying
4. Check GitHub Pages build status

---

**Questions?** Contact: bmantzey@mac.com

Built with HTML, CSS, and vanilla JavaScript. No frameworks, no build step, just clean code.
