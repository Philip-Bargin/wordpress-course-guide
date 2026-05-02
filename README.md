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
