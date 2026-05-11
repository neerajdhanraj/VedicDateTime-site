# VedicDateTime website (GitHub Pages)

This folder contains a **Quarto** website intended to be published with **GitHub Pages**.

## Local preview

1. Install Quarto: https://quarto.org/
2. From this folder:

```bash
quarto preview
```

## Build

```bash
quarto render
```

This renders the site to `docs/` (configured in `_quarto.yml`).

## Publish on GitHub Pages (project site)

1. Commit the website source files (this `site/` folder) and the generated `docs/` folder to your default branch (e.g., `main`).
2. In GitHub repo → **Settings** → **Pages**:
   - Source: **Deploy from a branch**
   - Branch: `main`
   - Folder: `/docs`
3. Save.

The project site URL is:

- `https://<OWNER>.github.io/<REPO>/`

Example:

- `https://neerajdhanraj.github.io/VedicDateTime/`

## Custom domain (optional)

GitHub Pages redirects to a custom domain if:

- **Settings → Pages → Custom domain** is set, or
- a `CNAME` file exists in the published site root (e.g., `docs/CNAME`)

To enable a custom domain later:

1. Set the custom domain in **Settings → Pages**.
2. Add a `docs/CNAME` file with your domain name.
3. Configure DNS at your domain provider.
