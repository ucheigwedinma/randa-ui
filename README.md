# Randa UI Registry

A lightweight static style guide for Randa brand assets and UI primitives.

## Overview

This project is a plain HTML/CSS registry used to preview:

- Brand assets (logo)
- Button variants
- Card styling
- Input styling

It has no build step and can run as a static site.

## Project Structure

```text
.
├── README.md
├── index.html
├── package.json
├── package-lock.json
├── site.webmanifest
├── css/
│   ├── tokens.css
│   ├── base.css
│   └── components.css
├── components/
├── assets/
│   ├── favicons/
│   │   ├── favicon.svg
│   │   ├── favicon-96x96.png
│   │   ├── favicon.ico
│   │   ├── apple-touch-icon.png
│   │   ├── web-app-manifest-192x192.png
│   │   └── web-app-manifest-512x512.png
│   ├── logos/
│   ├── icons/
│   └── fonts/
└── node_modules/
```

## Styling Architecture

- `css/tokens.css` defines design tokens (colors, spacing, radius, typography, transitions).
- `css/base.css` imports tokens and sets global element styles.
- `css/components.css` contains reusable component classes such as `.btn`, `.card`, and `.input`.

## Running Locally

### Option 1: Open directly

Open `index.html` in your browser.

### Option 2: Run a local static server

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Favicon and Web App Metadata

Favicon and PWA-related tags are defined in `index.html` `<head>`.

- Favicon image files currently live in `assets/favicons/`
- Web manifest is `site.webmanifest` at project root

## Dependencies

`package.json` currently includes:

- `lucide-react`

There are no npm scripts configured at this time.
