# Muhammad Ahmed Mufti, portfolio

Single-file static site (`index.html`) plus screenshots in `previews/`. No build step, no framework; Google Fonts are the only external dependency.

Live at https://ahmedmufti.github.io/portfolio/ (GitHub Pages, deployed from `master`).

## Structure

- Title block: name, role, location, status, links.
- Hero and live check: the visitor's browser pings each production site (`fetch` in `no-cors` mode) and shows whether it responded and the round-trip time. Nothing is cached or faked; free-tier hosts may show "waking up" for a moment.
- Sheets: one per live product, each with a current screenshot, what was built, the stack, and the figure it earned.
- Research plate, "Also built" table, toolbox, path (experience and education), contact.

## Editing

- Sites in the live check: the `SITES` array at the bottom of `index.html`.
- Screenshots: `previews/*.jpg`, 1200x750, captured with headless Edge at 1440x900 and resized. Update the "captured" date in each `figcaption` when you recapture.
- Colours and type: the `:root` block at the top of the `<style>`; dark mode tokens live under `prefers-color-scheme: dark`.

Every number on the page is taken from verified CV content. If a figure changes, update it here and in the CVs.
