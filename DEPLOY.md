# Deployment Guide — technical.skillshikshya.com

## Files in this delivery
| File | What it is | Who needs it |
|---|---|---|
| `skillshikshya-technical-WEBSITE-deploy.zip` | Production build (static files: HTML/JS/CSS/images/sitemap/robots) | Whoever uploads to hosting |
| `skillshikshya-technical-SOURCE-CODE.zip` | Full React + TypeScript source (no node_modules) | Development team |

---

## Option A — Instant public link (fastest, zero setup)
Open the latest version card in this conversation and click **「发布」 (Publish)**.
You get a public URL immediately — share it with anyone, anywhere.

## Option B — Your own hosting / domain (technical.skillshikshya.com)

The build works on **any static host with zero server configuration** (hash-based routing + relative asset paths).

### Netlify (easiest, free)
1. Go to https://app.netlify.com/drop
2. Drag-and-drop the **contents** of `skillshikshya-technical-WEBSITE-deploy.zip` (the unzipped folder)
3. Site is live on a `*.netlify.app` URL in seconds
4. Site settings → Domain management → add `technical.skillshikshya.com`, then create a CNAME record `technical` → your Netlify URL in your domain DNS

### Vercel (free)
1. `npm i -g vercel`
2. Unzip the deploy zip, `cd` into it, run `vercel` → follow prompts
3. Add `technical.skillshikshya.com` in project domains + DNS CNAME

### cPanel / traditional hosting (e.g. your current provider)
1. Unzip `skillshikshya-technical-WEBSITE-deploy.zip`
2. Upload ALL files to the subdomain's document root (e.g. `public_html/technical/` or wherever the subdomain points)
3. Done — no `.htaccess` rewrite rules needed (hash routing)

### GitHub Pages (free)
1. Create a repo, push the unzipped deploy contents
2. Settings → Pages → deploy from branch → root

---

## Switching to clean URLs at launch (optional, recommended for SEO)
The site currently uses hash URLs (`/#/courses/`) so it works everywhere with zero config.
For maximum SEO on your real domain:
1. In source: change `HashRouter` → `BrowserRouter` in `src/main.tsx`
2. Change `base: './'` → `base: '/'` in `vite.config.ts`
3. `npm install && npm run build`
4. Configure your host for SPA fallback (serve `index.html` for unknown paths — one line on Netlify/Vercel/nginx)
5. The included `sitemap.xml` already lists the clean production URLs — submit it in Google Search Console

## After going live — launch checklist
- [ ] Replace placeholder phone/WhatsApp numbers in `src/data/site.ts` with real ones, rebuild
- [ ] Verify Google Search Console + submit sitemap.xml
- [ ] Set up GA4 / Google Tag Manager
- [ ] Claim Google Business Profile (New Baneshwar location)
- [ ] Connect forms to a real inbox/CRM (drop a `fetch()` into the marked TODO in `src/components/InquiryForm.tsx`)
