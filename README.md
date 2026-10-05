# spinworth.tech

Static site for Spinworth Limited, the holding company for Begu, Brolick and Spinworth.

No build step: every file is served as-is from the root of `main` by GitHub Pages.

| File | Purpose |
| --- | --- |
| `index.html` | The page (inline CSS, no JavaScript) |
| `404.html` | Not-found page |
| `assets/` | Logos, icons and the social-share image |
| `site.webmanifest`, `favicon.ico` | Browser and home-screen icons |
| `robots.txt`, `sitemap.xml` | Search engines |
| `CNAME` | Custom domain `www.spinworth.tech` |
| `.nojekyll` | Serve files untouched (no Jekyll processing) |

## Preview locally

```bash
python3 -m http.server 8765
```

## DNS

- `www` CNAME → `<github-username>.github.io`
- `spinworth.tech` A → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`

GitHub redirects the apex to `www`. Tick "Enforce HTTPS" in Settings → Pages once the certificate is issued.
