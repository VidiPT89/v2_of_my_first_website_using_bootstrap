# ⚽ Estoril Praia Website v2 — Bootstrap 5 Redesign

> A complete rebuild of the Estoril Praia FC website using Bootstrap 5, with responsive grid, carousel, product cards, accordion blog, contact form, and photo gallery.

This is the second version of my Estoril Praia themed website, rebuilt from scratch using Bootstrap 5 instead of pure CSS Flexbox. The upgrade introduces responsive grid layouts, a collapsible navbar with hamburger menu, an image carousel with captions, product cards, a Fancybox-powered photo gallery with aspect-ratio cropping, an accordion component for the blog section featuring profiles of historical players (Jose Torres, Antonio Simoes, Fernando Santos, Eloi, Oscar Duarte, Diamantino Costa), a full contact section with form and embedded Google Maps, and real club content replacing the Lorem Ipsum from v1. The custom CSS layer preserves the iconic yellow (`#FFEE00`) and blue color scheme on top of Bootstrap's defaults.

## 📦 What's Inside

- 📱 Fully responsive Bootstrap 5 grid system with breakpoint-aware columns (`col-12 col-md-8`, `row-cols-2 row-cols-lg-6`)
- 🍔 Collapsible navbar with hamburger toggle for mobile (`navbar-toggler`, `navbar-expand-lg`)
- 🎠 Bootstrap Carousel with 6 slides, descriptive captions, and prev/next controls
- 🖼️ Photo gallery (12 images) with Fancybox lightbox integration and `aspect-ratio: 4/3` + `object-fit: cover`
- 🃏 6 product cards with `h-100` equal height, `flex-column` layout, and "Comprar" buttons
- 🪗 Bootstrap Accordion (dark theme, `data-bs-theme="dark"`) with 6 historic player profiles
- 📝 Contact form with Bootstrap form controls (name, email, subject, message + full-width submit button)
- 🗺️ Embedded Google Maps iframe (Estoril Praia SAD location, rounded corners)
- 📺 Embedded YouTube video (stadium section) with Bootstrap `ratio ratio-16x9` responsive wrapper
- ⬆️ Fixed "back to top" button (`position: fixed`, bottom-right, circular, blue/yellow)
- 🔤 Google Fonts (Orbitron) for section headings with `font-size: 2rem`
- 🎨 Font Awesome 7 icons for social media footer (Facebook, Instagram, YouTube, X, TikTok, LinkedIn)
- 📧 Real Estoril Praia contact emails organized in two columns (SAD departments + Club departments)
- ✍️ Real historical content: club founding story, stadium history, player biographies
- 🔄 Column reordering with `order-1 order-md-2` for responsive image/text swapping

## 🛠️ Tech Stack

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![Bootstrap 5](https://img.shields.io/badge/Bootstrap_5-7952B3?style=flat&logo=bootstrap&logoColor=white)
![Font Awesome](https://img.shields.io/badge/Font_Awesome_7-528DD7?style=flat&logo=fontawesome&logoColor=white)
![Google Fonts](https://img.shields.io/badge/Google_Fonts-4285F4?style=flat&logo=googlefonts&logoColor=white)

## 🏗️ Project Structure

```
v2_of_my_first_website_using_bootstrap/
├── index.html          # Main page (~1290 lines) with all Bootstrap components
├── styles.css          # Custom CSS layer (249 lines) on top of Bootstrap
└── images/
    ├── estorilpraia.png    # Club logo (navbar brand + header)
    ├── EPbandeira.JPG      # Header banner CSS background-image
    ├── EPfirstteam.jpg     # Team photo (Sobre section)
    ├── EP1.jpg - EP19.jpg  # Gallery + carousel photos (19 images)
    ├── EPgolo.jpg          # Goal celebration photo
    ├── EPgolo2.jpg         # Goal celebration photo 2
    ├── EPgolo21.JPG        # Hero full-width image
    ├── EPoldteam.JPG       # Historical team photo
    ├── EPrelva.jpg         # Stadium grass
    ├── EstadioEP.jpeg      # Stadium exterior
    ├── chuteiras.jpg       # Product: football boots (Adidas COPA)
    ├── lucasgr.jpg         # Product: goalkeeper gloves
    ├── caneleiras.jpg      # Product: shin guards
    ├── bola.jpg            # Product: Liga Portugal football
    ├── camisolatermica.jpg # Product: thermal shirt
    └── calcastermicas.jpg  # Product: thermal pants
```

## 🔄 v1 vs v2 Comparison

| Feature | v1 (Pure CSS) | v2 (Bootstrap 5) |
|---------|--------------|-------------------|
| **Layout** | Manual Flexbox, 992px max-width | Bootstrap Grid with responsive breakpoints |
| **Navigation** | Static horizontal Flexbox nav | Collapsible navbar with hamburger toggle |
| **Hero** | Single static image | Full-width image in grid column |
| **Images** | Single image per section | Carousel (6 slides) + Fancybox gallery (12 photos) |
| **Content** | Lorem Ipsum placeholder | Real Estoril Praia history, stadium info, player bios |
| **Products** | Single image + text | 6 product cards with descriptions and buy buttons |
| **Blog** | Image + text layout | Accordion with 6 expandable player profiles |
| **Contact** | Image + text layout | Form + Google Maps + organized email directory (15+ addresses) |
| **Icons** | Simple Icons SVGs (20x20px) | Font Awesome 7 social icons |
| **Footer** | Basic copyright + SVG icons | Bootstrap `list-group-horizontal` + Font Awesome |
| **Mobile** | Not responsive (fixed max-width) | Fully responsive with column reordering |
| **CSS Lines** | 209 | 249 (custom) + Bootstrap framework |

## 📱 Sections Overview

| Section | Bootstrap Components Used |
|---------|--------------------------|
| **Header** | Grid (`row`, `col-2`, `col`), `d-flex`, `align-items-center` |
| **Navbar** | `navbar`, `navbar-expand-lg`, `navbar-dark`, `navbar-toggler`, `collapse` |
| **Hero** | Full-width image in `col` with `p-0` and `w-100` class |
| **Sobre** | Grid with `col-12 col-md-8`, `order-2 order-md-1` responsive reordering |
| **Team** | Grid with `col-12 col-md-4`, image with `img-fluid` class |
| **Galeria** | `row-cols-2 row-cols-sm-3 row-cols-lg-4 row-cols-xl-6` + Carousel component |
| **Produtos** | `row-cols-2 row-cols-lg-6`, Cards with `h-100`, `flex-column`, `mt-auto` button |
| **Estadio** | Grid with `ratio ratio-16x9` YouTube embed + text column |
| **Blog** | Accordion (`accordion-item`, `collapse`, `data-bs-theme="dark"`) |
| **Contactos** | `col-md-6` columns, `list-unstyled`, form controls, Google Maps iframe |
| **Footer** | Grid with `list-group-horizontal`, Font Awesome `fa-brands` icons |

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/VidiPT89/v2_of_my_first_website_using_bootstrap.git

# 2. Open index.html in your browser
cd v2_of_my_first_website_using_bootstrap
open index.html    # macOS
# or: start index.html (Windows) / xdg-open index.html (Linux)
```

## 📝 Notes

- The page title is "Site EP com BootStrap" — still in Portuguese, reflecting the project's learning context
- The `<footer>` element is nested inside the last `<section id="contactos">` instead of being a direct child of `<body>` — this works visually but is semantically unusual and means the footer is technically part of the contacts section
- The gallery section mixes two Fancybox groups (`data-fancybox="galeria"` and `data-fancybox="EstorilPraia"`) across different photos — this is likely unintentional and causes the lightbox to split into two separate gallery slideshows
- The custom CSS overrides Bootstrap's blue `btn-primary` hover color only in the footer area — product cards keep Bootstrap's default blue buttons, creating an inconsistency
- Column reordering (`order-1 order-md-2`) is used effectively in the Sobre and Team sections to swap image/text positions between mobile (image on top) and desktop (image on side)
- The contact section contains real Estoril Praia SAD and Club email addresses (geral, comunicacao, marketing, juridico, contabilidade, scouting, depfutebol, security + club equivalents), organized into a professional two-column directory layout

---

Developed by **David Arsenio Martins** — *"Vidi"*
