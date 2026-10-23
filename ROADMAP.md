# Roadmap

Open items for publishing this archive (written 2026-10-23).

- [ ] Enable GitHub Pages: Settings → Pages → Deploy from branch `main` / `/ (root)`. The integration token can't do this, so it must be done by hand.
- [ ] Serve at `mycoffeehunt.com.au`:
  - [ ] Add a `CNAME` file at the repo root containing `mycoffeehunt.com.au`.
  - [ ] Set Custom domain to `mycoffeehunt.com.au` in Settings → Pages.
  - [ ] DNS: point the apex at GitHub Pages with four A records (`185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`) and a `www` CNAME to `directcoffee-admin.github.io`. Note this replaces whatever the domain serves today.
  - [ ] Tick Enforce HTTPS once the certificate is issued.
- [ ] Optional: move the contents of `mycoffeehunt.com.au/` to the repo root so URLs are `mycoffeehunt.com.au/` rather than `mycoffeehunt.com.au/mycoffeehunt.com.au/` (the root `index.html` redirect currently covers this).
