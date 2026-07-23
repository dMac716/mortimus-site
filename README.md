# mortimus-site

Landing page for **Mortimus** — honest edge-AI wildfire smoke detection for
Sage / Waggle camera nodes (Sage Grande: Summer of AI 2026).

- **Live:** https://mortimus.me (custom apex domain, served via GitHub Pages)
- **Pre-DNS preview:** https://dmac716.github.io/mortimus-site/
- **Code:** https://github.com/dMac716/Mortimus

This repo is intentionally single-purpose: one self-contained `index.html`
(no external assets, no build step) plus a `CNAME` pinning the apex domain.

## DNS (apex domain on GitHub Pages)

At the registrar for `mortimus.me`, create four A records and four AAAA records
pointing the apex `@` at GitHub Pages:

    A     @   185.199.108.153
    A     @   185.199.109.153
    A     @   185.199.110.153
    A     @   185.199.111.153
    AAAA  @   2606:50c0:8000::153
    AAAA  @   2606:50c0:8001::153
    AAAA  @   2606:50c0:8002::153
    AAAA  @   2606:50c0:8003::153

Optional `www` alias:

    CNAME www   dmac716.github.io.
