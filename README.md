# Sahil Tiwari — Portfolio Website

Personal portfolio site for **Sahil Tiwari**, System Engineer at Endure Air Systems Pvt. Ltd., working on avionics and embedded systems for UAVs. Built as a static site and hosted on GitHub Pages.

**Live site:** https://sahiltiwari3336-sudo.github.io/my-webpage

## Overview

A single-page portfolio covering:

- **Home** — hero intro with photo, title, and quick links
- **About** — background summary and education
- **Experience** — career timeline (Endure Air Systems, Amos Aerospace, Shyam Technosolutions, and university R&D roles)
- **Skills** — languages, microcontrollers/hardware, dev tools, frameworks, and OS
- **Projects** — UAV/drone, IoT/automation, and PCB/circuit design projects
- **Achievements** — competitions, awards, and workshops
- **Contact** — email and social links (LinkedIn, Instagram, Facebook)

## Design

- Dark blueprint-navy theme by default, with a light/dark toggle (top-right of the nav bar) — the choice is remembered on return visits.
- Amber accent color with a soldermask-green "PCB trace" line that runs down the page as a scroll-progress indicator — a nod to the PCB design work in the Projects section.
- Fonts: Big Shoulders Display (headings), IBM Plex Mono (labels/nav), Manrope (body text).
- Fully responsive across desktop, tablet, and mobile, with a slide-out nav menu on smaller screens.

## Tech stack

Plain **HTML, CSS, and vanilla JavaScript** — no frameworks, no build step. Chosen deliberately so the site can be hosted directly on GitHub Pages with zero configuration.

## Project structure

```
my-webpage/
├── index.html      # Page structure and content
├── style.css        # Design tokens, layout, responsive rules, light/dark theme
├── script.js         # Nav toggle, scroll-spy, scroll-reveal animations, theme toggle
├── sahil.jpg          # Profile photo
└── README.md
```

## Running locally

1. Clone the repo:
   ```bash
   git clone https://github.com/sahiltiwari3336-sudo/my-webpage.git
   cd my-webpage
   ```
2. Open `index.html` directly in a browser, or use the **Live Server** extension in VS Code for auto-reload on save (right-click `index.html` → *Open with Live Server*).

## Deployment

Hosted via **GitHub Pages**, deployed from the `main` branch, root folder.

To publish changes:
```bash
git add .
git commit -m "Update site"
git push origin main
```
GitHub Pages rebuilds automatically within a minute or two of a push.

## Customizing

- **Photo:** replace `sahil.jpg` with a new image of the same name, or update the `src` in the `<img>` tag inside the `photoPlaceholder` div in `index.html`.
- **Content:** all section content lives directly in `index.html` — edit text within the relevant `<section>` block.
- **Colors/fonts:** adjust the CSS custom properties at the top of `style.css` (`:root` for dark theme, `[data-theme="light"]` for light theme).
- **Social links:** update the `href` values in the Contact section of `index.html`.
