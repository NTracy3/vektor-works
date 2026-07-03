# Vektor.Works

Static website for [vektor.works](https://www.vektor.works) — construction consulting / owner's representative firm. Hosted on GitHub Pages. Migrated from Squarespace in July 2026.

## Structure

```
index.html       Home page (includes the Contact section, #vk-contact)
about.html       About page  (served at /about)
services.html    Services page (served at /services)
404.html         Shown for any address that doesn't exist
favicon.ico      Browser tab icon
CNAME            Tells GitHub Pages the custom domain (www.vektor.works)
.nojekyll        Tells GitHub Pages to serve files as-is
images/          All site photos (previously hosted on Squarespace's servers)
```

Each page is fully self-contained: its CSS lives in a `<style>` block and its
JavaScript in a `<script>` block inside the same file. Fonts (Roboto and
Roboto Condensed) load from Google Fonts.

## Editing

Edit the HTML files directly, then commit and push to the `main` branch.
GitHub Pages republishes automatically within a minute or two.

To preview locally, run this from the project folder and open
<http://localhost:8742>:

```
python3 -m http.server 8742
```

Note: local preview links between pages use extensionless paths (`/about`),
which the local server doesn't resolve — type `/about.html` in the address
bar instead. On GitHub Pages, `/about` works as-is.
