# Priya Aswani — Personal Website

Static personal site for [Priya Aswani](https://www.linkedin.com/in/priyaaswani1): AI/ML architecture, agentic systems, defense & mission simulation, and security graphs.

**Production domain (planned):** [priyaaswani.com](https://priyaaswani.com)  
**Target repository:** [https://github.com/paswani/Website](https://github.com/paswani/Website)

Plain HTML, CSS, and a small amount of vanilla JavaScript. No build step, no framework, host-agnostic.

## Contents

| Path | Purpose |
|------|---------|
| `index.html` | Single-page site (hero, about, experience, competencies, education, contact) |
| `css/styles.css` | Layout, typography, responsive styles |
| `js/main.js` | Mobile nav toggle, sticky header state, copyright year |
| `LICENSE` | MIT license for site source |
| `README.md` | This file |

## Local preview

From this directory:

```bash
cd /path/to/priyaaswani-site
python3 -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000) in a browser.

Any static file server works (for example `npx serve .` or VS Code Live Server).

## Deploy

This folder is ready to publish as a static site root:

- **GitHub Pages** — push to the target repo above; enable Pages from the branch root (or `/docs` if you prefer). Custom domain: `priyaaswani.com` (add a `CNAME` file containing `priyaaswani.com` if required by your host).
- **Netlify / Cloudflare Pages / Vercel / S3+CloudFront** — point the publish directory at this folder; no build command needed.
- **Any nginx / Apache / CDN** — serve `index.html` and the `css/` / `js/` assets as static files.

HTTPS and DNS for `priyaaswani.com` are configured at the registrar / host; the site itself has no server-side dependencies.

## Design notes

- Dark, restrained palette with a warm accent; serif headings + sans body.
- Semantic HTML landmarks, skip link, focus styles, and reduced-motion respect.
- Mobile-first nav collapse; experience timeline stacks on small screens.
- Resume PDF is **not** included in the public site; contact is via LinkedIn.

## License

Site source is licensed under the MIT License — see [LICENSE](LICENSE). Content (biographical text, experience claims) remains © Priya Aswani.
