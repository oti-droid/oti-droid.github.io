# DiMe (prototype)

Static, dependency-free website. 23 indexable pages, no build step needed to host.

## Deploy (pick one, free tiers)
- **Cloudflare Pages / Netlify:** create a project, upload this folder (or connect the repo). No build command; publish directory is the repo root. Use a root domain or the provided subdomain.
- **GitHub Pages:** works from a *user/organisation* site or a custom domain. Links are root-relative (`/about/`), so a project site under `/repo-name/` will break them.

## Before you deploy
1. Run `SITE_URL=https://your-real-domain node build.js` (script is separate) so canonical links and `sitemap.xml` use your domain. Currently set to https://oti-droid.github.io.
2. Forms are demos: they store nothing. Keep the demo labels until connected.
3. Legal pages are a draft, not reviewed by a lawyer.

## Measure
Run Lighthouse on /, /ai-for-managers/, /guide/ and /resources/ (Chrome DevTools > Lighthouse, mobile), and a WAVE accessibility check. Test on a real phone.
