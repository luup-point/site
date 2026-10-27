# LUUP. for festival organisers

Single static page (PT-PT / British English, toggle + browser detection). No build step, no dependencies.

- `index.html`: the whole page (styles and script inline; Archivo comes from Google Fonts)
- `luup-logo.png`: logo (off-white, only works on dark backgrounds)
- `CNAME`: custom domain for GitHub Pages (`luuppoint.com`). Delete it or change it if you host elsewhere.

## Things to set before launch
- Contact address: `festivals@luuppoint.com` (search/replace in `index.html`; it appears in two places in the CTA block).
- Replace the video placeholder, the founders' photo placeholder and the `#` privacy / terms links.
- Canonical / Open Graph URL is `https://luuppoint.com/`. There is no `og:image` yet (add a 1200x630 image for link previews).

## GitHub Pages
1. Push this folder as the repo root, then Settings > Pages > Deploy from branch (`main`, `/ (root)`), tick *Enforce HTTPS*.
2. DNS at the registrar, for an apex domain: four `A` records to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153` (plus a `CNAME` for `www` to `<user>.github.io`). Do not touch the MX records used by the email alias.
3. Check what `luuppoint.com` points to today before changing it.
