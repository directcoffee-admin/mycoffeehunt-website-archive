# Roadmap

Open items for publishing this archive (written 2026-10-23).

- [x] Enable GitHub Pages: Settings → Pages → Deploy from branch `main` / `/ (root)`. The integration token can't do this, so it must be done by hand.
- [ ] Serve at `mycoffeehunt.com.au` (live over http as of 2026-10-23; DNS check passed, HTTPS pending):
  - [x] Set Custom domain to `mycoffeehunt.com.au` in Settings → Pages.
  - [x] DNS: point the apex at GitHub Pages with four A records (`185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`) and a `www` CNAME to `directcoffee-admin.github.io`. Note this replaces whatever the domain serves today.
  - [ ] Tick Enforce HTTPS once the certificate is issued. If still greyed out after a few hours, Remove and re-add the custom domain to retrigger issuance.
- [ ] Optional: move the contents of `mycoffeehunt.com.au/` to the repo root so URLs are `mycoffeehunt.com.au/` rather than `mycoffeehunt.com.au/mycoffeehunt.com.au/` (the root `index.html` redirect currently covers this).
