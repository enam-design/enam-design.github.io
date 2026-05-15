# Esther Nam — Portfolio

Static HTML portfolio. Three pages, no build step, no dependencies.

## Files

```
index.html                 — Home page
UX Audit Case Study.html   — UX Audit case study
WSOL Case Study.html       — Writing Solutions case study
images/                    — All referenced images
```

## Hosting on GitHub Pages

1. Create a new repo on github.com (e.g. `esther-nam-portfolio`).
2. Upload everything in this folder to the repo root (drag-and-drop works).
3. Repo Settings → Pages → Source: `Deploy from a branch` → Branch: `main`, folder: `/ (root)` → Save.
4. Wait ~1 minute. Your site is live at `https://<username>.github.io/<repo-name>/`.

## Making edits

### Quick text/copy changes (from the browser, no setup)
1. Open the file on github.com
2. Click the pencil icon (✏️) in the top right
3. Edit the text
4. Scroll down → "Commit changes"
5. Site rebuilds in ~1 minute

### Bigger changes (local, with preview)
1. Install [VS Code](https://code.visualstudio.com/) (free)
2. Install the "Live Preview" extension (free)
3. Clone the repo locally, open in VS Code, right-click any HTML → "Show Preview"
4. Edit, save, see changes live
5. Commit & push when happy

## Common edits — where to find things

| Want to change... | File | Look for... |
|---|---|---|
| Headline on the homepage | `index.html` | `<h1>I'm Esther...` |
| Your name / wordmark | all three files | `Esther Nam` (top-left of nav) |
| Case study card copy | `index.html` | `<a href="UX Audit...` block |
| Case study headline | each `*.html` | `class="case-title"` |
| Role / Timeline / Scope / Outcome | each `*.html` | `class="hero-meta"` |
| Brand accent color | each `*.html` | `--accent:` in `<style>` |
| Body font | each `*.html` | `Inter` (search & replace) |

## Notes

- The light/dark toggle reads/writes `localStorage` under key `case-palette`. Choice persists across pages on the same domain.
- All three HTML files share the same nav, theme system, and color tokens — but each is fully self-contained (no shared CSS/JS files). Edit each one independently.
- Images are PNGs. To swap one, replace the file at the same path with the same filename; no HTML change needed.
