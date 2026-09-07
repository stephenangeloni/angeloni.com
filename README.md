# angeloni.com

The landing page for angeloni.com. Static HTML, no framework, no build step —
`index.html` is the whole site.

## Why the "other Angelonis" section exists

An email audit of this domain on 2026-09-06 found that 96% of inbound mail was
misdirected traffic intended for Grupo Angeloni, the Brazilian supermarket chain
at angeloni.com.br. Web traffic almost certainly arrives the same way, so the
page carries a clearly separated, plainly labelled section in Portuguese,
Italian and English pointing visitors to the company they actually want.

There is no affiliation with any of those companies. The framing is
deliberately "you may be looking for one of these", never a partnership.

## Notes

- Single file. The only other request is `favicon.svg`.
- Light and dark via `prefers-color-scheme`; no theme toggle, no JavaScript.
- Parallax uses CSS scroll-driven animations (`animation-timeline: view()`),
  wrapped in `@supports` and `prefers-reduced-motion: no-preference`. Browsers
  without support get a clean static page.
- `CNAME` pins the custom domain. Do not delete it.
- Deployed to GitHub Pages from `main`, served through Cloudflare (proxied).
