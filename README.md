# Atium RPG Manager website

A landing page for Atium RPG Manager, built with React, TypeScript, Vite, and Tailwind CSS. It reproduces the layout and Portuguese copy of the [original page](https://gabrielxgm.github.io/atium-page/) using screenshots from the [original repository](https://github.com/gabrielxgm/atium-page/).

## Run locally

Use Node.js 20.19+ (20.x) or 22.12+ and npm.

```sh
npm ci
npm run dev
```

Open the URL Vite prints, usually `http://localhost:5173/`.

## Commands

| Command | Purpose |
| --- | --- |
| `npm run dev` | Start the Vite development server. |
| `npm run build` | Type-check and build the site into `dist/`. |
| `npm run preview` | Serve the production build locally. |
| `npm run format` | Format the project with oxfmt. |

## Where things live

- `src/App.tsx` contains the page sections, navigation, and inline icons.
- `src/assets/` contains the app screenshots shown throughout the page.
- `src/index.css` loads the fonts and Tailwind CSS and defines global styles.
- `index.html` is the Vite entry page.
- `vite.config.ts` configures Vite, React, Tailwind CSS, and the Figma Make integration.
- `.figma/make/` contains the Figma Make settings and helper scripts.

The production build uses relative asset paths by default. `FIGMA_PUBLIC_URL` sets the base URL for Figma Make, while `GITHUB_PAGES_BASE` sets it for GitHub Pages.

## GitHub Pages

The site is published at [atiumrpg.github.io/atium-web-site](https://atiumrpg.github.io/atium-web-site/). Each push to `main` runs [the Pages workflow](.github/workflows/deploy-pages.yml), which installs dependencies, builds the site with `GITHUB_PAGES_BASE=/atium-web-site/`, and publishes `dist/`. The workflow can also be started manually from the Actions tab.

## Links to finish

The Windows, Linux, and macOS download buttons are disabled until installers are published. The reference page uses `#` placeholders for **GitHub** and **Suporte**; replace them with real destinations when they are available. **Ver pitch** opens the [pitch video](https://youtu.be/bLEmkXoMsTI) in a new tab.
