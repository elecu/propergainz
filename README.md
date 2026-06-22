# Plant-Based Fitness & Nutrition Coaching Site

A single-page marketing and booking site for a vegetarian/vegan strength nutrition and training coaching business. Live at the project's GitHub Pages / static hosting deployment.

## What it does

- Presents the coach's services (personalized nutrition plans, training programming, plant-based coaching) and pricing tiers.
- Bilingual UI (English/Spanish) with a client-side language switcher that persists the choice in `localStorage`.
- Promotes two companion fitness apps the coach built: OjasFuel (food/barcode lookup for vegan/vegetarian status and macro tracking) and RepStack (browser-based workout logger).
- Lets visitors pay or book directly via PayPal and Buy Me a Coffee links, and routes new clients to a Google Form intake.
- Tracks visits with Google Analytics (gtag.js) and handles a contact form submission through the Web3Forms API.
- Scroll-triggered fade/slide-in animations for sections as the user scrolls down the page.

## How it's built

- **Single static file**: the entire site is one `index.html` containing structure, CSS, and JavaScript — no build step, framework, or bundler.
- **Styling**: plain CSS3 with custom properties (CSS variables) for theming, flexbox/grid layouts, and keyframe animations.
- **Internationalization**: a JavaScript `translations` object maps element IDs to English/Spanish strings; switching language updates the DOM's `textContent` directly rather than reloading the page.
- **Interactivity**: vanilla JavaScript (no external JS frameworks) for the language toggle, scroll-based reveal animations, and the contact form's `fetch` call to Web3Forms.
- **Analytics**: Google Tag Manager / gtag.js snippet loaded asynchronously.
- **Assets**: static images (logos, payment icons, screenshots) served alongside the HTML.

## Tech stack summary

HTML5, CSS3, vanilla JavaScript (ES6+) — no frameworks, no dependencies, no build tooling. Deployed as a static site.
