# SE-Josh.github.io

This repository contains the static files for **Josh's personal portfolio website**. The site is built with Vue and bundled into plain HTML, CSS, and JavaScript so it can be deployed directly to GitHub Pages or any other static file host.

## Project Structure

- `index.html` – entry point for the website
- `js/` and `css/` – compiled JavaScript and style sheets
- `src/` – source Vue components used to build the site
- `img/`, `projectsImg/` and `fonts/` – static assets referenced by the pages
- `portfolio.pdf` – downloadable PDF version of the portfolio

The contents of `src/` show the original Vue Single File Components used before building the final bundle found in `css/` and `js/`.

## Running Locally

The site is a pure static bundle, so you can open `index.html` directly in a browser or serve the folder with any simple HTTP server. For example:

```bash
python3 -m http.server
```

Then visit `http://localhost:8000` to view the portfolio.

## Customization

To modify or extend the website, edit the Vue files in `src/` and rebuild the project using your preferred Vue build tooling (e.g. Vue CLI or Vite). The repository does not contain build scripts, so you may need to create a new Vue project and copy these components if you plan to rebuild from source.


