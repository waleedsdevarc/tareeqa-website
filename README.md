# Tareeqa

Source for [tareeqa.site](https://tareeqa.site), the public documentation site for Tareeqa, a free science tutoring program for deaf and hard-of-hearing students in Gujranwala, Pakistan, founded and led by Waleed Ahmed Syed in partnership with Bibi 'N' Baba School.

The site documents what the program does, how lessons are designed, and its tracked outcomes (attendance, lesson plans, and before/after grades).

## Stack

Static HTML, CSS, and inline SVG. No build step, no JavaScript, no framework.

```
├── index.html          Home
├── about/index.html     About
├── impact/index.html    Impact
├── privacy/index.html   Privacy policy
├── css/style.css        Shared styles
├── assets/               Logo, illustration, and Open Graph image (SVG/PNG)
├── robots.txt
├── sitemap.xml
├── llms.txt
└── CNAME                 Custom domain (tareeqa.site)
```

## Running locally

No build step is needed. Open `index.html` directly in a browser, or serve the folder with any static file server, for example:

```bash
npx serve .
```

## Deployment

Pushes to `main` trigger the GitHub Actions workflow in `.github/workflows/deploy.yml`, which publishes the repository root to GitHub Pages at the custom domain configured in `CNAME`.

## License

All rights reserved. See [LICENSE](LICENSE).
