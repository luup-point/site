# LUUP. for festival organisers

Single static page (PT-PT / British English, toggle + browser detection). No build step, no dependencies.

- `index.html`: the whole page (styles and script inline; Archivo comes from Google Fonts). It contains no embedded images or video.
- `assets/`: **all media files** (video, phone screens, founders photo, link-preview image, logo). See `assets/README.md` for the file-by-file list with sizes. To swap one, overwrite the file and keep its name.
- `CNAME`: custom domain for GitHub Pages (`www.luuppoint.com`). Delete it or change it if you host elsewhere.

## Where to put the hero video
`assets/video/hero.mp4` (plus `assets/video/hero-poster.jpg`, its first frame). 4:5 portrait, H.264 MP4, no audio. It autoplays muted and loops continuously, with a script that restarts it if a browser pauses it.

## Things to set before launch
- Contact address: `festivals@luuppoint.com` (search/replace in `index.html`; it appears in two places in the CTA block).
- Replace the temporary hero video, the three mock-up phone screens (`assets/img/app-*.png`) and the founders photo.
- Canonical / Open Graph URL is `https://www.luuppoint.com/`; the link-preview image is `assets/img/og-image.jpg` (default logo card).

## GitHub Pages
1. Push this folder as the repo root, then Settings > Pages > Deploy from branch (`main`, `/ (root)`), tick *Enforce HTTPS*.
2. DNS at the registrar (already set): a `CNAME` record named `www` pointing to `luup-point.github.io.`. For the bare domain (`luuppoint.com`, no www) to work as well you would also need four `A` records to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`; GitHub then redirects it to www. Do not touch the MX records used by the email alias.
   Keep the `CNAME` file in this repo: if it is deleted, GitHub can drop the custom domain setting.
3. Check what `www.luuppoint.com` points to today before changing it.
