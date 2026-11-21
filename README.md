# Sunscreen website

Static single-page site for sunscreen.energy. Moved off Lovable on Nov 21, 2026 — hosted free on GitHub Pages.

## Files

- `index.html` — the whole site (copy + dark stealth styling, no build step, no dependencies)
- `CNAME` — custom domain (`sunscreen.energy`) for GitHub Pages

## Deploy

Push to the `main` branch of the repo with GitHub Pages enabled (deploy from branch, root folder). GitHub Pages serves the custom domain and provisions HTTPS automatically once DNS points at it.

## DNS

`sunscreen.energy` is proxied through Cloudflare. Point the apex record at GitHub Pages:

- A records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- `www` CNAME: `<username>.github.io` (optional)

Remove the old Lovable origin record. Keep the Cloudflare proxy on; SSL mode Full (strict) works with GitHub Pages HTTPS.

## Editing

Edit `index.html` directly and push — no Lovable, no build, no monthly fee.
