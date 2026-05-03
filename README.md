# Dr. B Arvind — Personal Brand Website

A premium, fully responsive personal brand website for **Dr. B Arvind**, Consultant Oral & Maxillofacial Oncosurgeon, Hyderabad.

---

## 📁 Project Structure

```
dr-arvind-website/
├── index.html              ← Main website file
├── assets/
│   ├── css/
│   │   └── style.css       ← All styles (premium medical aesthetic)
│   └── js/
│       └── main.js         ← Interactions: navbar, accordion, animations
└── README.md               ← This file
```

---

## 🚀 How to Run the Project

### Option 1 — Open Directly in Browser (Simplest)

1. Unzip the downloaded file `dr-arvind-website.zip`
2. Open the extracted folder
3. Double-click `index.html`
4. The website opens in your default browser — **no server needed**

---

### Option 2 — Using VS Code Live Server (Recommended for Development)

1. Unzip the folder
2. Open the folder in **Visual Studio Code**
3. Install the **Live Server** extension (by Ritwick Dey) from the Extensions panel
4. Right-click `index.html` → **"Open with Live Server"**
5. The site opens at `http://127.0.0.1:5500`

---

### Option 3 — Using Python Local Server

If you have Python installed:

```bash
# Navigate into the project folder
cd dr-arvind-website

# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Then open your browser and go to: **http://localhost:8000**

---

### Option 4 — Using Node.js (npx serve)

```bash
cd dr-arvind-website
npx serve .
```

Then visit: **http://localhost:3000**

---

## 🖼️ Adding Real Images

The website currently has **image placeholders**. To add real photos:

1. Place doctor photos inside `assets/images/` (e.g., `doctor-hero.jpg`, `doctor-about.jpg`)
2. In `index.html`, replace the placeholder `<div>` blocks like:

```html
<!-- Replace this: -->
<div class="hero-image-placeholder">...</div>

<!-- With this: -->
<img src="assets/images/doctor-hero.jpg" alt="Dr. B Arvind" 
     style="width:100%; border-radius: var(--radius-lg); object-fit:cover;" />
```

---

## 🗺️ Embedding Google Maps

To replace the map placeholders with real maps:

1. Go to [maps.google.com](https://maps.google.com)
2. Search for the clinic address
3. Click **Share → Embed a map → Copy HTML**
4. Replace the `<div class="location-map-placeholder">` with the `<iframe>` code
5. Set the iframe `width="100%"` and `height="200"`

---

## 🎥 Adding a Video

To add a real video to the hero section:

```html
<!-- Replace the .video-placeholder div with: -->
<video controls poster="assets/images/video-thumb.jpg" 
       style="width:100%; border-radius: var(--radius-lg);">
  <source src="assets/images/intro-video.mp4" type="video/mp4">
</video>
```

Or embed a YouTube video:

```html
<iframe width="100%" style="aspect-ratio:16/9; border-radius:20px; border:none;"
  src="https://www.youtube.com/embed/YOUR_VIDEO_ID"
  allowfullscreen></iframe>
```

---

## ✏️ Customisation

All design variables are in `assets/css/style.css` at the top under `:root {}`:

```css
:root {
  --navy: #0B1A2E;       /* Primary dark colour */
  --gold: #C9A84C;       /* Accent gold */
  --teal: #1B6B7B;       /* Clinic accent */
  --font-display: 'Cormorant Garamond', serif;
  --font-body: 'DM Sans', sans-serif;
}
```

---

## 📱 Responsive Breakpoints

| Breakpoint | Layout |
|---|---|
| > 1100px | Full desktop, 4-column grids |
| 900–1100px | 2-column grids |
| 640–900px | Single column, mobile nav |
| < 640px | Compact mobile layout |

---

## ✅ Features Included

- Fixed navbar with scroll effect
- Hero with animated stat counters
- Trust bar
- 4-card expertise section
- About section with qualifications
- Hospital section (clearly separated from clinic)
- Dhriti Dental clinic section with team + services
- 2-branch location cards
- Dental tourism section
- Working FAQ accordion
- Final dual CTA
- Footer with all contact info
- Smooth scroll animations (Intersection Observer)
- Fully mobile responsive
- Mobile hamburger menu

---

## 📞 Contact Details (Pre-filled)

| | |
|---|---|
| Nallagandla | +91 83310 03232 |
| Manikonda | +91 79811 00921 |
| Email | dhritidentals@gmail.com |

---

*Built for Dr. B Arvind — Oral & Maxillofacial Oncosurgeon, Hyderabad*
