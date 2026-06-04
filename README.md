# MVR Public Relations — Website

Live at **[mvr-pr.com](https://mvr-pr.com)**.

A static portfolio for MVR Public Relations, the Manila PR studio of Michaela Villaroman. Plain HTML/CSS/JS, no build step, no framework.

## Stack
- Static HTML across one homepage + five case studies
- One shared stylesheet (`styles.css`)
- `main.js` for mobile nav, scroll reveal, and the mailto contact form
- Hosted on Netlify with continuous deployment from this repo

## Local preview
```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Structure
```
index.html              Homepage
work/
  dr-shiba-kind-kibble.html
  prof-bengal.html
  golds-gym-hyrox.html
  sicilian-roast.html
  matsusaka-beef.html
404.html
styles.css
main.js
assets/
  work/                 Case-study hero photos
  press/                Outlet logos
  ...                   Favicons, OG images, brand marks
robots.txt, sitemap.xml, site.webmanifest
```

## Brand
- Red `#db423d` · deeper red `#c0392f` (AA-safe for small text) · ink `#231f20` · ivory `#f1f1f2`
- Type: Avenir Next with Manrope as the web fallback

## Deploy
Pushing to `main` triggers a Netlify build automatically. Manual deploys still work too:

```bash
netlify deploy --prod --dir=.
```
