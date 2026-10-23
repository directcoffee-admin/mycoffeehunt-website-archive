# Roadmap

Open items for publishing this archive (written 2026-10-23).

- [x] Enable GitHub Pages: Settings → Pages → Deploy from branch `main` / `/ (root)`. The integration token can't do this, so it must be done by hand.
- [x] Serve at `mycoffeehunt.com.au` (live, HTTPS enforced as of 2026-10-23):
  - [x] Set Custom domain to `mycoffeehunt.com.au` in Settings → Pages.
  - [x] DNS: point the apex at GitHub Pages with four A records (`185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`) and a `www` CNAME to `directcoffee-admin.github.io`. Note this replaces whatever the domain serves today.
  - [x] Enforce HTTPS.
- [x] Moved the site from the `mycoffeehunt.com.au/` subfolder to the repo root, so the homepage is `https://mycoffeehunt.com.au/` (once merged to `main`).
