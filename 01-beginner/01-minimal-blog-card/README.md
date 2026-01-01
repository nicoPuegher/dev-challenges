# 📇 Minimal Blog Card

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)
![Type](https://img.shields.io/badge/Type-UI%20Component-orange)
![Status](https://img.shields.io/badge/Status-Complete-success)

A clean, responsive, and modern blog card component built as part of the DevChallenges series. This project focuses on semantic HTML, modern CSS layout techniques, and performance optimization.

The solution features a mobile-first approach, fluid typography using CSS variables, and optimized image loading.

## What it does

The component renders a self-contained blog preview card that includes:

1. **Optimized Image:** Uses `srcset` and `sizes` to serve the appropriate image resolution based on the viewport.
2. **Category Tag:** A visually distinct badge for content categorization.
3. **Semantic Content:** Proper use of heading levels and paragraph spacing for readability.
4. **Responsive Layout:** Centered using Flexbox with a fixed-width container that scales gracefully.
5. **Theming Support:** Basic setup for `prefers-color-scheme` to handle system-level light/dark modes.

## Technical Highlights

The project implements several best practices:

* **Performance:** Preloading critical assets (fonts and hero images) to minimize Largest Contentful Paint (LCP).
* **BEM Methodology:** Uses Block-Element-Modifier naming convention for maintainable CSS.
* **Modern CSS:** Utilizes `100dvh` for full-height centering and custom properties (variables) for a consistent design system.
* **Accessibility:** Semantic tags like `<article>`, `<header>`, and `<footer>` for better screen reader support.

## Requirements

- Node.js (v18.x or higher recommended)
- A modern web browser

## Setup

```shell
# 1. Create a new directory for your project and enter it
mkdir dev-challenges
cd dev-challenges

# 2. Initialize a new git repository
git init

# 3. Add the remote origin
git remote add -f origin https://github.com/nicoPuegher/dev-challenges.git

# 4. Enable Sparse Checkout
git config core.sparseCheckout true

# 5. Tell Git which folder you want
echo "01-minimal-blog-card" >> .git/info/sparse-checkout

# 6. Pull the content
git pull origin main
```

Install dependencies:

```shell
npm install
```

Run the development server:

```shell
npm run dev
```

The application will be available at `http://localhost:5173`.

## Deployment

To create a production-ready build:

```shell
npm run build
```

This will generate a `dist/` folder with minified assets ready for hosting on platforms like Vercel, Netlify, or GitHub Pages.

## Notes

- Vite Integration: While the core is pure HTML/CSS, Vite is used as a lightning-fast build tool and dev server.
- Typography: Uses the 'Sora' font family via Google Fonts with optimized woff2 preloading.
- Project Purpose: Part of a series of frontend challenges to master layout precision and asset optimization.
