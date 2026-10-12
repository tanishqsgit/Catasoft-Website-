# CataSoft Website (Local Clone)

This is a complete local replica of [https://catasoft.vercel.app/](https://catasoft.vercel.app/) including all static pages, styles, fonts, assets, and scripts.

---

## 🚀 How to Run Locally

### Option 1: Using Node.js (Recommended)
You can run the server directly using npm or node:

```bash
npm start
```
or
```bash
node server.js
```

Then open your browser and navigate to:
👉 **[http://localhost:3000](http://localhost:3000)**

*(To run on a different port, set `PORT=8080 node server.js` or set the environment variable).*

---

### Option 2: Using Python
If you prefer Python's built-in HTTP server:

```bash
python -m http.server 3000
```
Then visit **[http://localhost:3000](http://localhost:3000)**.

---

### Option 3: Using VS Code Live Server
Right-click on `index.html` and select **"Open with Live Server"**.

---

## 📁 Directory Structure

```text
catasoft/
├── index.html                               # Main landing page HTML
├── server.js                                # Zero-dependency Node.js HTTP server
├── package.json                             # Project metadata and run scripts
├── README.md                                # Instructions
├── images/                                  # High-resolution website images
│   ├── catasoft-logo.png                    # Brand logo
│   ├── hero-plant.png                       # Hero section background
│   ├── bim-model.png                        # BIM model graphic
│   └── point-cloud.png                      # Point cloud 3D graphics
├── apple-icon.png                           # Apple touch icon
├── icon.svg                                 # Vector brand favicon
├── icon-dark-32x32.png                      # Dark theme favicon
├── icon-light-32x32.png                     # Light theme favicon
└── _next/                                   # Next.js static bundles
    └── static/
        └── immutable/
            ├── chunks/                      # Stylesheet and JavaScript bundles
            └── media/                       # Web fonts (Geist, Geist Mono, etc.)
```
