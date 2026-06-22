# Jungdesign portfolio

A fast, fully static Astro site for David Jung. The artwork catalogue drives the painting gallery and generates a detail page for every work.

## Run locally

```bash
npm install
npm run dev
```

Use `npm run build` for a production build. The generated site is in `dist/` and can be deployed directly to Cloudflare Pages, Netlify, or Vercel. Use build command `npm run build` and output directory `dist`.

## Add or edit artwork

1. Put a web-ready JPG, PNG, AVIF, or WebP in `public/images/artworks/`.
2. Add one object to `src/data/artworks.json`. Copy an existing object so all fields remain present.
3. Give it a unique lowercase `slug` with hyphens. Its detail URL will be `/paintings/your-slug/`.
4. Replace placeholder year, medium, dimensions, note and availability as facts become known.
5. Write useful alt text describing the image rather than repeating the title.

The order in the JSON file controls gallery and previous/next order. Category names also generate the gallery filters automatically.

## Before launch

- Contact email links currently use `jungdesign@gmail.com` in `src/pages/contact.astro`.
- Confirm artwork titles and metadata with David.
- Replace process placeholder notes with David’s words.
- Add design archive material as it is digitised.
- Update the canonical `site` value in `astro.config.mjs` if the domain changes.

The site uses remote Google Fonts with robust local fallbacks. For maximum privacy and resilience, self-host Archivo Black, Barlow Condensed and DM Sans before launch.
