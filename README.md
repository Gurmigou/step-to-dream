# За крок до мрії

Landing page for Krystyna Kyrylenko's coaching program, built with [Astro](https://astro.build). Mobile-first, follows the original 390px design mockup, with a responsive desktop layout.

## Run

```bash
npm install
npm run dev      # http://localhost:4321
npm run build    # static output in dist/
npm run preview
```

## Where to edit

| What | File |
|---|---|
| Links (Instagram, Telegram, booking, diagnostic PDF, offer, privacy), prices, open spots | `src/config/site.ts` |
| Repeated copy: cards, sessions, FAQ, reviews, method, changes, nav | `src/data/content.ts` |
| Section markup and section-specific styles | `src/components/sections/*.astro` |
| Colors, fonts, shared primitives (`.pill`, `.num`, `.card`, `.hscroll`) | `src/styles/global.css` |
| Photos and certificates (auto-optimized to WebP) | `src/assets/` |

## Placeholders to fill in

- `site.links.*` in `src/config/site.ts` currently point to page anchors. Replace them with real Telegram, booking (Calendly or similar), diagnostic PDF, offer, and privacy URLs.
- Session details ("Що відбувається на сесії"): `sessions[].details` in `src/data/content.ts` is marked `[уточнити: …]`.
- FAQ "Як оплатити? Чи можна частинами?": the answer is marked `[уточнити: …]`.
