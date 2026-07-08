# flowlamina.com

Hand-coded static site for Flowlamina. No build step, no framework, no dependencies.

## Files

- `index.html` — the entire site (single page)
- `style.css` — all styling; brand colours defined as CSS variables at the top
- `assets/` — logo + favicon (sourced from `proposal/static/` in the main workspace)
- `CNAME` — tells GitHub Pages the custom domain (`flowlamina.com`); do not delete
- `404.html` — branded not-found page

## Editing

Edit `index.html` / `style.css` directly, then preview locally:

```sh
python3 -m http.server 8080   # open http://localhost:8080
```

## Deploying

Hosted on GitHub Pages from the `main` branch of `harshan-jpg/flowlamina-site`:

```sh
git add -A && git commit -m "Update site" && git push
```

Live ~30 seconds after push. DNS: Namecheap A records (@ → GitHub Pages IPs
185.199.108/109/110/111.153) + CNAME `www` → `harshan-jpg.github.io`.
