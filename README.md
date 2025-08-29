# Web-Development-Project
A concise, user-friendly README is below, tailored to the attached commit and repository contents, with setup, usage, file map, and contribution notes aligned to a static HTML/CSS/JS site that includes contact.php for form handling and multiple range-specific results pages.

Project overview
Percent2College Engineering Admission Recommender is a static web application that helps prospective engineering students quickly discover colleges aligned to their board exam percentage bands, using curated lists segmented by score ranges (e.g., 100–90, 90–80, …, 50 and below) and a simple, responsive UI built with HTML, CSS, and JavaScript. It includes a basic PHP endpoint for contact form submission if deployed on a PHP-capable host.

Features
Percentage-band pages: Prebuilt pages for common score ranges: 100–90, 90–80, 80–70, 70–60, 60–50, and 50-below, each with a styled table of institutes, locations, scores, and ranks for quick scanning.

Single-page landing: An index.html homepage with hero imagery, navigation, and links to each band page for fast navigation across segments.

Lightweight stack: Pure HTML, CSS (style.css), and vanilla JS (main.js) ensure fast load times and easy hosting on static hosts; no build step required.

Getting started
Prerequisites: Any static web server or a modern browser to open files directly; optional PHP support if using contact.php for form handling.

Quick run (local):

Option 1: Double-click index.html to open in a browser for local testing; range pages are linked from the homepage.

Option 2: Serve locally with a simple HTTP server (e.g., Python http.server) to mimic hosting and proper asset paths.

Hosting: Upload the repository files to any static host (GitHub Pages, Netlify) for the static site; for the contact form, deploy on a PHP-capable host (cPanel, Apache with PHP) and point the form action to contact.php.

File structure
index.html: Landing page linking to each percentage-band recommender page, using hero-bg.jpg and site assets.

100-90.html, 90-80.html, 80-70.html, 70-60.html, 60-50.html, 50-below.html: Precomposed results pages with institute tables; styled with consistent table CSS.

style.css: Global styles for typography, layout, hero, tables, and responsive tweaks across pages.

main.js: Client-side scripts for interactivity and navigation UX as used by index.html and related pages.

contact.php: Minimal backend endpoint intended for processing contact form submissions if hosted with PHP.

Assets: about1.jpg, about2.jpg, about3.jpg, hero-bg.jpg for visuals; favicon.png and apple-touch-icon.png for icons.

Usage
Browse by score: From the homepage, select the matching percentage range to open a curated list of engineering institutes with city, state, indicative score, and rank columns presented in a readable table layout.

Open external info: Many institute names are linked to external info pages in a new tab (rel="noopener noreferrer") for deeper research without losing context in the recommender site.

Contact: If enabled on a PHP host, submit the contact form to send queries through contact.php; ensure server mail settings or handler logic are configured per hosting environment.

Data and content notes
The range pages display static, human-curated institute entries with columns Name, City, State, Score, and Rank, intended for quick exploration rather than official counseling decisions.

Some links route to institute or aggregator pages for reference; validate current year rankings and cutoffs directly with official sources before finalizing choices.

Customization
Edit table rows: Open any range page (e.g., 60-50.html) and add, remove, or reorder <tr> entries to refine the recommendations by region, discipline, or updated ranks.

Theme and branding: Update style.css for colors, spacing, and typography; replace hero-bg.jpg and about images to align with institutional or project branding.

Navigation and UX: Modify index.html and main.js to add a score input form that routes users to a computed range or directly filters a unified table view.
