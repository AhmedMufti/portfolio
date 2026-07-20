# Ahmed Mufti — Portfolio

Single-file static portfolio site (`index.html`). No build step, no dependencies beyond Google Fonts.

## Preview locally

Just open `index.html` in a browser, or:

```
npx serve .
```

## Deploy (Vercel, ~1 minute)

```
npm i -g vercel   # if not installed
vercel --prod
```

Or push the folder to a GitHub repo and enable GitHub Pages (Settings > Pages > deploy from branch), or drag the folder into https://app.netlify.com/drop.

## Editing

Everything lives in `index.html`:

- **The ledger** (hero metrics): search for `ledger-row`. Each row is a label, a `data-count` number, and a source link.
- **Projects**: search for `work-row`. Each has domain tags, title, blurb, stack line, links, and a right-side figure.
- **Colors/fonts**: the `:root` block at the top of the `<style>`.
- **Hover peeks**: `previews/*.png` are real screenshots of the live sites, shown in a popover when hovering the project title. Re-capture them when a site's landing page changes (1280x800 screenshots).

All numbers on the page are drawn from verified CV content. If a metric changes (e.g. roadmaps generated), update both the ledger row and the project row.
