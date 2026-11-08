# abhay-dev

| File | Purpose |
|------|---------|
| `index.html`      | All visible content. Edit names, projects, jobs, certs, skills, contact. |
| `css/design.css`  | Look: colours (`:root` block at top), fonts, spacing, print. |
| `css/base.css`    | Accessibility rules. Don't edit. |
| `css/layout.css`  | Generated layout numbers. Rarely edit. |
| `js/site.js`      | Dark switch, depth toggles, timeline. Edit only if changing behaviour. |
| `content/Resume.pdf` | Replace with your CV. |

## Preview

    python -m http.server 8000 --directory abhay-dev
    # http://127.0.0.1:8000/

Don't open `index.html` via `file://` — the CSP blocks local CSS/JS on a null origin.

## Edit map (`index.html`)

- Name → `<h1 class="intro-name">`
- Tagline → `<p class="headline">`
- Availability → `<p class="avail">`
- Facts → `<ul class="facts">`
- Intro paragraphs → `<p class="lede">`
- CTA buttons → `<ul class="cta">`
- Result cards → `<ul class="results">`
- Projects → `<div class="proj-grid">`
- Timeline → `<ol class="tl-list">`
- Work → `<div class="jobs">`
- Education → `<article class="degree">`
- Certifications → `<ul class="certs">`
- Skills → `<ul class="skills">`
- Contact → `<ul class="routes">`
- Footer → `<footer class="foot">`

## Recolour

Open `css/design.css` — first block:

    :root {
      --bg: #FFFFFF;
      --ink: #000000;
      --link: #0037A6;
      --sans: system-ui, …;
      --mono: ui-monospace, …;
    }

Dark mode uses the same names under `:root[data-theme="dark"]`.
