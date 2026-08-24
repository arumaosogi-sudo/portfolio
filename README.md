# Portfolio — Nitiphum Hongson

Personal portfolio site. Hand-coded, no framework — a single `index.html` with plain CSS and
about 30 lines of JavaScript.

**Live:** https://arumaosogi-sudo.github.io/portfolio/

## What's in it

- Sticky two-column layout — the left side stays put while the content scrolls
- **Thai / English toggle** (remembers your choice in `localStorage`)
- Reveal-on-scroll and nav highlighting via `IntersectionObserver` — no scroll listeners
- Responsive down to mobile, with a sticky section label instead of the side nav
- Respects `prefers-reduced-motion`

## Files

```
index.html     the entire site
profile.jpg    profile photo
og-card.png    1200x630 social preview image
```

## Running it

No build step — open `index.html`, or serve the folder:

```bash
npx serve .
```

## Deploying

**GitHub Pages** — push this folder to a repo, then Settings → Pages → Source: `main` branch, `/root`.
Live at `https://<username>.github.io/<repo>/` in about a minute.

**Vercel** — vercel.com → Add New → Project → import the repo → Deploy. No configuration needed;
Vercel serves static files as-is.

## Editing

Every piece of text exists twice — once inside `<span data-en>` and once inside `<span data-th>`.
Edit both, or the language toggle will show a gap. Colours live in the `:root` block at the top of
the `<style>` tag.

---

Built by **Nitiphum Hongson** · [github.com/arumaosogi-sudo](https://github.com/arumaosogi-sudo) · aruma.osogi@gmail.com
