# BBOP Dataset Website

Your academic project page for PhD applications.

## 🚀 Quick Deploy to GitHub Pages (15 min)

### Step 1: Create a GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Name it something like `bbop-dataset` or `social-neural-imaging`
3. Make it **Public** (required for free GitHub Pages)
4. Click "Create repository"

### Step 2: Upload Your Files

**Option A: Upload via GitHub web interface (easiest)**

1. On your new repo page, click "uploading an existing file"
2. Drag and drop these files:
   - `index.html` (the website)
   - `poster_sfn_2024.pdf` (rename your SfN poster to this)
   - `poster_bmes_2024.pdf` (your BMES poster)
   - Any images you extract from your poster (put in `assets/` folder)

**Option B: Use Git command line**
```bash
git clone https://github.com/YOUR_USERNAME/bbop-dataset.git
cd bbop-dataset
# copy your files here
git add .
git commit -m "Initial website"
git push
```

### Step 3: Enable GitHub Pages

1. Go to your repo on GitHub
2. Click **Settings** (tab at top)
3. Scroll down to **Pages** (left sidebar)
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 1-2 minutes, then your site is live at:
   ```
   https://YOUR_USERNAME.github.io/bbop-dataset/
   ```

### Step 4: Update Links in index.html

Before uploading, find and replace these placeholders:

| Find | Replace with |
|------|--------------|
| `https://github.com/YOUR_USERNAME/bbop` | Your actual GitHub repo URL |
| `poster_sfn_2025.pdf` | Your actual poster filename |
| `mailto:lingxuan.qi@duke.edu` | Your email |
| `cv.pdf` | Your CV filename (if adding) |

---

## 📁 Recommended File Structure

```
bbop-dataset/
├── index.html              # Main website
├── poster_sfn_2024.pdf     # SfN poster
├── poster_bmes_2024.pdf    # BMES poster  
├── cv.pdf                  # Optional: your CV
├── README.md               # This file
└── assets/                 # Images folder
    ├── system-schematic.png
    ├── arena-setup.png
    ├── pipeline-diagram.png
    └── results-figure.png
```

---

## 🖼️ Adding Images from Your Poster

To extract figures from your poster PDF:

**On Mac:**
1. Open poster in Preview
2. Use rectangle select tool
3. Cmd+C to copy, then Cmd+N to create new image
4. Save as PNG

**On Windows:**
1. Open in Adobe Acrobat or PDF viewer
2. Use Snapshot/Select tool
3. Paste into Paint, save as PNG

**Or use an online tool:**
- [PDF to PNG converter](https://www.ilovepdf.com/pdf_to_jpg)

Then in `index.html`, replace the placeholder divs with actual images:

```html
<!-- Replace this: -->
<div class="figure-placeholder">...</div>

<!-- With this: -->
<img src="assets/system-schematic.png" alt="System schematic">
```

---

## 🔗 Put This URL on Your CV

Once live, add to your CV under Publications or Projects:

```
Project Website: https://YOUR_USERNAME.github.io/bbop-dataset/
```

Or create a shorter link using a custom domain later.

---

## ❓ Troubleshooting

**Site not showing up?**
- Wait 2-5 minutes after enabling Pages
- Check Settings → Pages for any error messages
- Make sure repo is Public

**Images not loading?**
- Check filenames match exactly (case-sensitive!)
- Use relative paths: `assets/image.png` not `/assets/image.png`

**Want a custom domain?**
- Buy a domain (Namecheap, Google Domains, etc.)
- Add a CNAME file to your repo
- Configure DNS - GitHub has docs for this

---

## 🎨 Customizing

**Change colors:**
Look for `:root` at the top of the CSS in index.html:
```css
--color-accent: #003366;  /* Duke blue - change this */
```

**Add more sections:**
Copy an existing `<section>` block and modify.

---

Good luck with your PhD applications! 🎓
