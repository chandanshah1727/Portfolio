# Chandan Shah — Personal Portfolio

A modern, dark-themed personal portfolio built with **HTML5**, **CSS3**, and a small amount of **vanilla JavaScript**. No frameworks.

## Quick start

1. Open `index.html` in your browser, **or**
2. Use a local server (recommended):

```bash
# From the portfolio folder
npx serve .
# or
python -m http.server 5500
```

Then visit `http://localhost:5500` (or the port shown).

## File structure

```
portfolio/
├── index.html          # All page content & sections
├── style.css           # Theme, layout, animations, responsive styles
├── script.js           # Navbar, menu, scroll effects, contact form
├── README.md
└── assets/
    ├── profile.jpg     # About section photo
    ├── resume.pdf      # Resume download (replace with yours)
    └── projects/       # Project thumbnail images
        ├── vehicle-rental.jpg
        ├── clothing-store.jpg
        └── resource-allocator.jpg
```

## What to personalize

Search the HTML for comments that start with `REPLACE` — or update these items:

| Item | Where |
|------|--------|
| Profile photo | `assets/profile.jpg` |
| Resume PDF | `assets/resume.pdf` |
| GitHub URL | Links marked in Hero, Contact, Footer, Projects |
| LinkedIn URL | Same places |
| Email | `mailto:` links and contact form |
| Phone | Contact section |
| Project GitHub / Live Demo URLs | Each project card in Projects |
| Project thumbnails | `assets/projects/*.jpg` |
| Stats numbers | `data-target` attributes in About |
| College / education details | Education timeline (already filled from your resume) |

## Sections included

1. Sticky glass navbar + mobile hamburger menu  
2. Hero with terminal-style visual  
3. About + stats  
4. Skills (Programming, Web, AI/ML, Tools)  
5. Projects (Vehicle Rental, Clothing Store, Adaptive Resource Allocator)  
6. Education timeline + training + certifications  
7. Resume download  
8. Contact (mailto form; Formspree-ready comments)  
9. Footer + back-to-top  

## Theme customization

Colors and fonts are CSS variables at the top of `style.css`:

```css
:root {
  --bg-primary: #0a0a0f;
  --accent: #6366f1;
  --accent-2: #8b5cf6;
  /* ... */
}
```

## Contact form

By default the form opens the visitor’s email app via `mailto:`.

To use [Formspree](https://formspree.io) later:

1. Create a form and copy the endpoint URL  
2. Set the form `action` to that URL and `method="POST"`  
3. Remove the mailto handler in `script.js`

## Browser support

Works on modern desktop and mobile browsers. Layout is tested conceptually for widths from **375px** to **1920px**.
