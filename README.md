# Semantic HTML Resume

## Project Description
This project is a personal resume webpage designed and built with strict adherence to modern semantic HTML standards and WCAG 2.1 AA accessibility guidelines. The resume is contained within a single HTML file (`index.html`) and styled using a single CSS file (`style.css`). It completely avoids generic elements like `<div>` and `<span>` in structural areas, utilizing `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, and `<dl>` for a semantically rich document. The layout is achieved using modern CSS Grid and Flexbox, featuring a responsive, premium dark mode aesthetic.

## How to Run
1. Download or clone this repository to your local machine.
2. Simply double-click the `index.html` file to open it in any modern web browser (e.g., Chrome, Firefox, Safari). No local server or build tools are required.

---

## Test Cases for Video Demonstration

For your video demonstration, you can present the following test cases to verify the functionality, accessibility, and resilience of the website:

### Normal Test Cases (Standard Functionality)
1. **Semantic Structure & Validation:** 
   - *Test:* Run the page through the [W3C HTML Validator](https://validator.w3.org/) or an Accessibility Checker (like axe DevTools).
   - *Expected:* The page passes without errors. Demonstrate the heading hierarchy strictly flows from `<h1>` to `<h2>` to `<h3>` without skipping levels, and dates are wrapped in `<time>` tags.
2. **Standard Desktop Layout:** 
   - *Test:* View the webpage on a standard 1080p desktop display.
   - *Expected:* The CSS Grid and Flexbox layouts structure the header, navigation, and lists neatly. Hover states and micro-animations activate smoothly.
3. **Keyboard Navigation:** 
   - *Test:* Navigate the entire page using only the `Tab` and `Enter` keys.
   - *Expected:* Focus states highlight correctly on all navigation links and contact info. Users can seamlessly jump to different sections via the sticky navigation bar without needing a mouse.

### Edge Test Cases (Stress Testing & Limits)
1. **Extreme Mobile Viewport (Responsive Design):** 
   - *Test:* Open browser Developer Tools and set the viewport to an ultra-narrow device (e.g., 320px width, iPhone SE).
   - *Expected:* The layout does not break. Multi-column grids (like the Skills section) gracefully collapse into a single column, text remains readable, and there is absolutely no horizontal scrolling.
2. **200% Zoom (Accessibility Reflow):** 
   - *Test:* Increase the browser zoom level to 200% on a standard desktop view.
   - *Expected:* Text scales appropriately without overlapping or getting clipped. The layout reflows to accommodate the larger text, ensuring visually impaired users can read the resume comfortably.
3. **Color Contrast Verification:** 
   - *Test:* Run a color contrast checker (like WCAG Color Contrast Analyzer) against the background (`#0d1117`) and text/accent colors (`#c9d1d9`, `#58a6ff`).
   - *Expected:* The contrast ratio easily exceeds the minimum 4.5:1 required by WCAG 2.1 AA, proving the premium dark theme is both beautiful and highly accessible.
