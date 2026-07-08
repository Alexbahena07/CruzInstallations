Cruz Installations & Remodeling LLC

The official website for Cruz Installations & Remodeling LLC, a family-owned flooring and remodeling company serving Chicago, the surrounding suburbs, and southern Wisconsin. It's a single-page marketing site built with plain HTML and CSS, deployed on GitHub Pages under the custom domain cruzinstallations.com.

What it is

The whole site lives in one index.html file styled by global.css. There's no framework and no build step — it's a hand-written static page you can open in a browser as-is. The goal was a fast, clean, mobile-friendly landing page that shows off the company's services and real project photos, and makes it easy for a customer to get in touch.

Features

The page is broken into ten anchored sections that the nav links jump to: a hero with the company pitch and trust badges, a services grid (tile, laminate, carpet tile, V.C.T., LVP, vinyl, baseboards, and stairs), a "Past Projects" photo carousel, a mid-page call-to-action strip, a "Why Choose Cruz" section, a "How It Works" walkthrough, the company's story, a service-area section with an embedded Google map, an FAQ, and a contact section.

A couple of small pieces of vanilla JavaScript sit at the bottom of index.html: an auto-scrolling, infinitely looping carousel for the project photos (it pauses when you hover over it), and a hamburger toggle that opens and closes the nav menu on mobile. Font Awesome is pulled in from a CDN for the icons, and the layout is responsive down to phone widths.

Project structure

CruzInstallations/
├── index.html      # The entire single-page site (all sections + inline JS)
├── global.css      # All styling
├── CNAME           # Custom domain config for GitHub Pages (cruzinstallations.com)
├── images/         # Logo, favicon, and project photos used across the page
└── .DS_Store        # macOS artifact (safe to ignore / remove)

Tech stack


HTML5 — semantic single-page structure
CSS3 — all layout and styling in global.css, responsive design
Vanilla JavaScript — the carousel and mobile nav, no libraries
Font Awesome 6.5 — icons, loaded via CDN
GitHub Pages — hosting, with a CNAME pointing at the custom domain


Running it locally

Since there's no build step, you have two easy options. You can just open the file directly:

bashopen index.html

Or, if you'd rather serve it (which more closely matches how GitHub Pages runs it), start a quick local server from the repo root:

bashpython3 -m http.server 8000

Then visit http://localhost:8000 in your browser.

Deployment

The site is deployed through GitHub Pages from the main branch. The CNAME file maps the Pages site to cruzinstallations.com, so any push to main that touches index.html, global.css, or the images/ folder will go live once Pages rebuilds. To update project photos, drop new files into images/ and reference them from the carousel in index.html.

Contact


Phone: (773) 997-6074
Email: Flooringinstallation26@gmail.com
Facebook: CruzInstallations7



© 2026 Cruz Installations & Remodeling LLC. All rights reserved.
