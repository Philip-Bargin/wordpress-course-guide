# WordPress Course Guide — Deployment Instructions

## 🚀 Hosting on GitHub Pages

### Step 1 — Create a GitHub Repository
1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click **"New repository"**
3. Name it: `wordpress-course-guide` (or any name you prefer)
4. Set visibility: **Public** (required for free GitHub Pages)
5. Click **"Create repository"**

### Step 2 — Upload the Files
**Option A — Via the GitHub Website (easiest):**
1. Inside your new repository, click **"Add file" → "Upload files"**
2. Drag and drop `index.html` into the upload area
3. Click **"Commit changes"**

**Option B — Via Git (recommended):**
```bash
git init
git add index.html
git commit -m "Initial commit: WordPress course guide"
git branch -M main
git remote add origin https://github.com/Philip-Bargin/wordpress-course-guide.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. In your repository, click **Settings** (top menu)
2. In the left sidebar, scroll to **"Pages"**
3. Under **"Branch"**, select `main` and folder `/root`
4. Click **"Save"**
5. Wait 1–2 minutes, then visit: `https://Philip-Bargin.github.io/wordpress-course-guide/`

---

## 📄 Generating the PDF

The guide has a built-in **"Download / Print as PDF"** button that uses your browser's print function.

### Method 1 — Use the Button (Recommended)
1. Open the webpage in **Google Chrome** or **Microsoft Edge**
2. Click the amber **"⬇ Download / Print as PDF"** button
3. In the print dialog:
   - Destination: **"Save as PDF"**
   - Layout: **Portrait**
   - Margins: **Default** or **Minimum**
   - Scale: **85–90%** (fits more content per page)
   - Options: ✅ **Background graphics** (keeps colored section headers)
4. Click **"Save"**

### Method 2 — Keyboard Shortcut
- Press `Ctrl + P` (Windows / Linux) or `Cmd + P` (Mac)
- Follow same settings as above

### Tips for Best PDF Output
- Use **Google Chrome** for the most accurate CSS rendering in print
- Enable **"Background graphics"** in print options to preserve green section headers and colored boxes
- The sidebar table of contents is automatically hidden in print mode
- All "Download PDF" buttons are hidden in the printed output

---

## 📁 File Structure

```
wordpress-course-guide/
└── index.html          # Complete guide — all HTML & CSS in one file
└── README.md           # This deployment guide
```

The entire guide is self-contained in a **single HTML file** with embedded CSS. No build process, no dependencies, no framework required.

---

## ✅ Compatibility

| Browser | Rendering | PDF Export |
|---|---|---|
| Google Chrome (latest) | ✅ Full | ✅ Best |
| Microsoft Edge (latest) | ✅ Full | ✅ Good |
| Firefox (latest) | ✅ Full | ✅ Good |
| Safari (latest) | ✅ Full | ✅ Good |
| Mobile Chrome | ✅ Responsive | ⚠️ Use desktop for PDF |

---

## 🎨 Customisation

To change the colour scheme, edit the CSS variables at the top of the `<style>` block in `index.html`:

```css
:root {
  --green-800: #1B4332;   /* Primary dark green */
  --amber-500: #D97706;   /* Accent amber/orange */
  --cream:     #FAF7F2;   /* Page background */
}
```

To update the bakery name throughout, use Find & Replace (`Ctrl+H`) to replace:
- `Sweet Palm Bakery` with your preferred name
- `Monrovia` with your preferred city
- `+231 777 123 456` with your preferred phone number

---

*Guide created for instructional use. All business names and details are fictional.*
