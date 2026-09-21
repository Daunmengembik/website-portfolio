# adrianaryp.site

Static portfolio site. Plain HTML, CSS and a little JavaScript. No build step, no dependencies.

```
index.html                                   Home (about, experience, projects, education, skills)
projects/tactical-field-monitoring.html      Inovast Consulting project
projects/water-quality-monitor-refurbishment.html   BRIN RI project
projects/smart-water-monitoring.html         Final project
assets/style.css                             All styling (colors are variables at the top)
assets/main.js                               Theme toggle, active nav link, footer year
assets/images/                               Put your pictures here
```

Preview locally: open `index.html` in a browser, or run `python3 -m http.server` in this folder.

## Before you deploy

1. **Pictures.** Every "input picture here" box is a placeholder. Put your image in `assets/images/`, then in the HTML replace
   `<div class="pic-ph" ...>...</div>` with
   `<img src="../assets/images/your-file.jpg" alt="Describe the picture">`
   (use `assets/images/...` without the `../` on `index.html`).
   Each project page has a comment showing the exact line for the main pictures.
2. **Social links.** In `index.html`, replace the LinkedIn and GitHub URLs (search for `TODO`).
3. **Check the text** on each project page and add real details where you have them: measurements, results, part numbers, what you learned.
4. **Optional.** Add a personal paragraph to the About section, and a 1200x630 preview image for link sharing (see the commented `og:image` line).

## Deploy to adrianaryp.site

Any static host works.

- **Hostinger:** File Manager > `public_html` > upload everything in this folder (keep the folder structure), so `index.html` sits directly in `public_html`.
- **Netlify or Cloudflare Pages:** drag the folder into the dashboard, then add `adrianaryp.site` under Domain settings and follow the DNS instructions.
- **GitHub Pages:** push the folder to a repository, enable Pages, then add `adrianaryp.site` as the custom domain.

Fonts (Space Grotesk, JetBrains Mono) load from Google Fonts. If they're blocked, the site falls back to system fonts.
