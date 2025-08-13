# Roast & Ritual — Coffee Shop Website

This repository contains a simple multi-page coffee shop website built with HTML and Tailwind CSS classes applied directly in the markup. The site is responsive, modern, and designed to fill the full width of the viewport on all devices (all main wrappers use w-full / max-w-none).

Files:
- index.html — Home page with hero, features, interactive menu filtering, and newsletter modal.
- about.html — About page with story, roast philosophy, and team profiles.
- contact.html — Contact page with contact form and map placeholder.

Key features:
- Tailwind CSS is loaded via CDN so you can open the pages directly in a browser.
- Google Fonts are declared (Poppins and Merriweather). Each HTML file includes a comment indicating the fonts:
  - <!-- {{font: Poppins}} -->
  - <!-- {{font: Merriweather}} -->
  The fonts are also linked for immediate preview.
- Images use placeholders in the format required by the system: {{image: a detailed description}}. The platform that fetches images will replace these placeholders with appropriate images (Unsplash/Pexels/Pixabay).
- Interactive JavaScript included inline for:
  - Menu filtering by category (All, Espresso, Brew, Pastries)
  - Mobile nav toggle
  - Newsletter modal with subscription flow
  - Order buttons that show temporary feedback
  - Contact form validation and fake submit

Design guidelines followed:
- Full-width layout: main wrappers use w-full and max-w-none, avoiding fixed max-width classes so content spans the viewport.
- Responsive grids and stacks for mobile-friendly layouts.
- Tailwind utility classes are used throughout for spacing, color, and animations (hover/transition/transform).
- Subtle animations and hover effects on cards and buttons.

How to use:
1. Open index.html in a modern browser. Because Tailwind is loaded via CDN, no build step is required for preview.
2. To replace images locally, swap the img src attributes containing the {{image: ...}} placeholders with real image paths.
3. Customize copy, colors, or fonts directly in the HTML files.

Notes:
- The contact and newsletter forms simulate submission; there is no backend in this sample. Hook them up to a server or API to enable real submissions.
- The Google Font comments ({{font: ...}}) are intentionally present at the top of the HTML files — this helps automatic build systems detect and include fonts if integrated into a larger pipeline.

If you want additional pages (e.g., a shop, wholesale portal, or events calendar) or a build setup (Tailwind CLI / PostCSS), tell me what you need and I can add them.
