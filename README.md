# Dead Product Museum — Starter

Hybrid Light/Dark Astro site with MDX exhibits and 3 example pages.

## Quick start (local)
1. Install Node.js 18+
2. `npm install`
3. `npm run dev`  (open http://localhost:4321)

## Deploy to Cloudflare Pages (recommended)
1. Create a new GitHub repository (empty)
2. Upload these files to the repo (or push via git)
3. In Cloudflare Pages: **Create project → Connect to Git → Select the repo**
4. Build command: `npm run build`
5. Build output directory: `dist`
6. Save → Cloudflare builds and deploys automatically

## Content model
- Exhibits live in `src/content/exhibits/*.mdx`
- Each file uses frontmatter:

  ```yaml
  ---
  title: Example Product
  years: 1990–2003
  cause: Consolidation and changing tastes
  summary: Short teaser
  ---
  ```

## Create a new exhibit
1. Duplicate an MDX file in `src/content/exhibits`
2. Update the frontmatter + body
3. Commit and push — deploy happens automatically

## Theming
- Light is default; toggle persists in `localStorage`
- Colors are defined in `src/styles/global.css`

## Roadmap
- Pagefind search
- Affiliate blocks (Amazon/eBay/Reverb)
- Brand pages + timelines
- JSON-LD for Articles, Breadcrumbs, ItemList, Product
