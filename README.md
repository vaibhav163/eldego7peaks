# Eldeco 7 Peaks — React Website

A modern, luxury real estate website for **Eldeco 7 Peaks**, Greater Noida.  
Built with **React 18 + Vite**. No external UI libraries — pure React with inline styles.

---

## 🚀 Getting Started

### 1. Install dependencies
```bash
npm install
```

### 2. Start development server
```bash
npm run dev
```
Open [http://localhost:5173](http://localhost:5173) in your browser.

### 3. Build for production
```bash
npm run build
```

---

## 📁 Project Structure

```
eldeco-7-peaks/
├── index.html
├── vite.config.js
├── package.json
└── src/
    ├── main.jsx                  # React entry point
    ├── App.jsx                   # Root component + modal state
    ├── constants/
    │   ├── data.js               # All content data (stats, plans, amenities, etc.)
    │   └── theme.js              # Color tokens
    ├── hooks/
    │   └── useReveal.js          # useReveal + useScrolled custom hooks
    └── components/
        ├── GlobalStyles.jsx      # Google Fonts + CSS reset
        ├── UI.jsx                # Shared: Reveal, SectionLabel, SectionTitle, Buttons
        ├── Navbar.jsx            # Sticky nav with mobile menu
        ├── Hero.jsx              # Split hero with stats & price tag
        ├── About.jsx             # About section with feature grid
        ├── FloorPlanSVG.jsx      # SVG schematic by plan ID
        ├── FloorPlans.jsx        # Tabbed floor plan viewer
        ├── Amenities.jsx         # Bento photo grid + pill list
        ├── Gallery.jsx           # Asymmetric masonry gallery
        ├── DeveloperStrip.jsx    # Eldeco credentials banner
        ├── Location.jsx          # Dark panel + Google Maps iframe
        ├── EnquiryModal.jsx      # Controlled form modal w/ success state
        ├── FloatingBar.jsx       # Scroll-triggered sticky CTA bar
        └── Footer.jsx            # Site footer with links
```

---

## ✨ Features

- **Fully responsive** — mobile-first with media queries
- **Scroll animations** — custom `useReveal` hook with IntersectionObserver
- **Interactive Floor Plans** — tab switching between 3 BHK, 3 BHK+, 4 BHK
- **Enquiry Modal** — form with success confirmation state
- **Floating CTA bar** — appears after scrolling 500px
- **Sticky Navbar** — shadow/border appears on scroll
- **Google Maps** integration for location section

---

## 🎨 Customisation

| What to change | Where |
|---|---|
| Colors / tokens | `src/constants/theme.js` |
| Project data (stats, prices, distances) | `src/constants/data.js` |
| Images | Replace Unsplash URLs in `data.js` and component files |
| Phone number | `Navbar.jsx` and `FloatingBar.jsx` |
| Google Maps embed | `Location.jsx` — replace the `src` URL in the `<iframe>` |

---

## 🛠 Tech Stack

- React 18
- Vite 5
- No CSS framework — inline styles + `<style>` blocks
- No external component libraries
