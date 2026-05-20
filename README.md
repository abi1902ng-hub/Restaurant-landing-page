# 🌶 Saffron & Spice — Restaurant Website

A responsive restaurant landing page built with pure HTML and CSS, featuring a fully functional mobile navigation bar, hover effects, and a multi-section layout.

---

## 📋 Problem Statement

**Design a Responsive Navigation Bar**

Create a responsive navigation bar that works well on both desktop and mobile devices, using:
- HTML and CSS for structure and styling
- CSS media queries for responsiveness
- Hover effects for interactive elements

---

## 🌐 Live Preview

Open `index.html` directly in any modern browser — no build tools or dependencies required.

---

## 📁 Project Structure

```
restaurant-website/
├── index.html       # Main HTML file — all sections and nav markup
└── styles.css       # All styles — layout, responsive breakpoints, hover effects
```

---

## ✨ Features

### Responsive Navigation Bar
- **Desktop** — Horizontal nav with animated underline hover effects and a styled "Reserve Table" CTA button
- **Mobile (≤ 768px)** — CSS-only hamburger menu (no JavaScript) using a hidden checkbox toggle; slides in a full-height side drawer
- **Hamburger animation** — Three bars morph into an × icon when the menu is open
- **Backdrop** — Semi-transparent overlay appears behind the open drawer on mobile

### Sections
| Section | Description |
|---|---|
| **Hero** | Full-viewport background image with gradient overlay, tagline, and CTA buttons |
| **About** | Two-column grid with an image (zoom-on-hover), an "Award Winning" badge, and animated stat cards |
| **Menu** | Dark-themed card grid showcasing 3 dishes; cards lift and image zooms on hover |
| **Gallery** | CSS Grid masonry-style layout with colour-overlay hover effect |
| **Contact** | Reservation form with name, email, guest count, and special requests; focus/hover states on all inputs |
| **Footer** | Minimal dark footer with image credits |

### Interactivity (CSS only)
- Smooth scroll to all sections (`scroll-behavior: smooth`)
- Nav link underline slide-in on hover
- Menu cards lift (`translateY`) and rotate slightly on hover
- Gallery images scale and saturate on hover with a magenta gradient overlay
- Stats cards lift on hover
- About image zooms on hover; badge rotates slightly
- All transitions respect `prefers-reduced-motion`

---

## 🎨 Design System

### Colour Palette
| Variable | Hex | Usage |
|---|---|---|
| `--saffron` | `#f4a261` | Logo, accents, borders |
| `--coral` | `#e76f51` | Primary buttons, hover states |
| `--magenta` | `#c9184a` | Gradients, CTA highlights |
| `--teal` | `#2a9d8f` | Price badges, accent colour |
| `--gold` | `#e9c46a` | Hero tag, section labels |
| `--cream` | `#fff8f0` | Page background |
| `--charcoal` | `#1a1a2e` | Nav, footer, headings |

### Typography
- **Display / Headings** — `Playfair Display` (Google Fonts) — serif, elegant
- **Body / UI** — `Poppins` (Google Fonts) — sans-serif, clean

---

## 📐 Responsive Breakpoints

| Breakpoint | Layout Changes |
|---|---|
| `> 992px` | Full desktop layout — side-by-side grids, 3-column menu, 4-column gallery |
| `≤ 992px` | Tablet — single-column about/contact, 2-column menu and gallery |
| `≤ 768px` | Mobile — hamburger nav drawer, single-column menu, stacked hero buttons |
| `≤ 480px` | Small phones — single-column gallery, smaller section padding |

---

## 🚀 Getting Started

No installation or build step needed.

```bash
# Clone or download the project
git clone https://github.com/your-username/restaurant-website.git

# Open in browser
open index.html
# or just double-click index.html in your file explorer
```

---

## ♿ Accessibility

- Semantic HTML5 elements (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`)
- `aria-label` on the `<nav>` and checkbox toggle
- `aria-hidden` on decorative elements (logo icon, overlay)
- Descriptive `alt` text on all images
- Focus-visible styles on all form inputs
- Motion disabled for users who prefer reduced motion via `@media (prefers-reduced-motion: reduce)`

---

## 🛠️ Built With

- **HTML5** — Semantic markup
- **CSS3** — Custom properties, Grid, Flexbox, `clamp()`, `min()`, gradients, transitions
- **Google Fonts** — Playfair Display, Poppins
- **Unsplash** — Placeholder photography

---

## 📄 License

This project is for educational and demonstration purposes.  
Images sourced from [Unsplash](https://unsplash.com/) under the Unsplash License.
