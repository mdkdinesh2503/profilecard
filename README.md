# Profile Card

A single-page, responsive profile card built with HTML, CSS, and vanilla JavaScript. It displays personal info, a profile image, and social links with smooth hover and click interactions.

## Overview

This project is a minimal, self-contained profile/portfolio card. All markup, styles, and scripts live in one `index.html` file. It uses CSS variables, Flexbox, and a mobile-first media query for small screens.

## Project Structure

```
profilecard/
├── index.html      # Single file: HTML, CSS, and JS
├── mdk.jpg         # Profile photo
├── Title_logo.png  # Favicon (browser tab icon)
└── README.md       # This file
```

## Features

- **Profile card layout** – Name, location, role, email, and profile image in a centered card.
- **Social links** – Icons for Facebook, Instagram, WhatsApp, LinkedIn, and GitHub with external links.
- **Image interaction** – Clicking the profile image toggles an “active” state that expands the image (intended for use with the `.active` class in CSS).
- **Hover effects**
  - Social icons slide in from the left with staggered delays on card hover.
  - “Read More” button scales and inverts colors on hover.
- **Responsive design** – Media query at `max-width: 400px` adjusts card size, image dimensions, and icon size for small screens.
- **Basic UX safeguards** – Ctrl key and right-click are disabled via JavaScript.

## Tech Stack

| Layer   | Technology                          |
|--------|-------------------------------------|
| Markup | HTML5                               |
| Styles | CSS3 (variables, Flexbox, transitions) |
| Icons  | [Font Awesome 5.15.3](https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css) (CDN) |
| Script | Vanilla JavaScript (no frameworks)  |

## Design

- **Colors** – Brown (`#414141`), light brown (`#b2a9a9`), and white, defined as CSS custom properties in `:root`.
- **Typography** – System font stack: Verdana, Geneva, Tahoma, sans-serif.
- **Layout** – Centered card (max-width 538px), fixed card size (400×500px, 300×400px on small screens).

## How to Run

1. Clone or download the repo.
2. Ensure `index.html`, `mdk.jpg`, and `Title_logo.png` are in the same directory.
3. Open `index.html` in a browser (e.g. double-click or “Open with” your browser).

No build step or server is required. For local development you can also use a simple static server (e.g. `npx serve .` or VS Code “Live Server”) if you prefer.

## Customization

- **Content** – Edit the name, location, role, email, “Read More” URL, and social links inside `index.html`.
- **Assets** – Replace `mdk.jpg` and `Title_logo.png` with your own image and favicon; keep the same filenames or update the `href`/`src` in the HTML.
- **Theme** – Change the palette by updating the CSS variables in the `:root` block (`--brown`, `--light-brown`, `--white`, etc.).

## Browser Support

Works in modern browsers that support CSS custom properties, Flexbox, and basic DOM APIs. Font Awesome is loaded from a CDN and requires internet access when viewing the page.

## License

Use and modify as needed for personal or academic projects.
