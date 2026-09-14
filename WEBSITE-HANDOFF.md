# technical.skillshikshya.com — Build Handoff (Step by Step)

**What was delivered:** a complete, working multi-page website (React 19 + TypeScript + Vite 7 + Tailwind 3.4 + shadcn/ui), built directly from the SRS + competitor research. It is the reference implementation your dev and design teams work from — every page, section order, keyword target, and schema rule from the SRS is implemented and visible in the browser preview.

---

## 1. Site map (everything that was built)

| # | Route | Page | Primary keyword target |
|---|---|---|---|
| 1 | `/` | Homepage (13 sections) | vocational training institute Nepal |
| 2 | `/courses/` | Courses hub (filter pills, 10 courses, 4 categories) | vocational courses Nepal |
| 3 | `/courses/:slug/` ×10 | Course detail template (see §3) | "[trade] course in Nepal" per course |
| 4 | `/foreign-employment-preparation/` | NSTB skill-test abroad hub (biggest keyword gap) | NSTB skill test Nepal |
| 5 | `/skill-test-and-certification/` | CTEVT vs NSTB explainer (trust page) | CTEVT NSTB certification Nepal |
| 6 | `/corporate-and-group-training/` | B2B page + proposal form | corporate vocational training Nepal |
| 7 | `/success-stories/` | 9 real testimonials, filterable by trade | graduate success stories |
| 8 | `/graduate-registry/` | Certificate-ID verification tool (4 sample records) | employer verification |
| 9 | `/blog/` + `/blog/:slug/` ×4 | SEO content engine with 4 full articles | informational clusters |
| 10 | `/about/` | Story, accreditation, instructors, facility | about / CTEVT registered centre |
| 11 | `/contact-and-counseling/` | Primary conversion page | free counseling |

**Global elements on every page:** sticky navbar (Courses · Foreign Employment · Certification · Success Stories · Corporate Training · About · phone · Free Counseling), WhatsApp FAB bottom-right (pre-filled chat), pre-footer dark CTA banner (per-route copy variants), full footer with course links + CTEVT Reg. No. 2018-KTM-0421.

---

## 2. Homepage — 13 sections, step by step (SRS §7.1 implemented)

1. Hero: "Learn a skill. Get certified. Get hired." + inline free-counseling form + trust pills (CTEVT / NSTB Level 1 & 2 / 2,000+ Placed / Since 2018)
2. Accreditation strip: CTEVT · NSTB · Ministry of Labour & Employment
3. Upcoming Batch Dates — August 2026 (3 batch cards, "only N seats left" bars — data-driven, not hardcoded)
4. "Pick your trade field" — 4 icon category tiles with course counts + from-price
5. Salary table — Local vs Gulf vs Europe vs Japan G2G by trade
6. "Built around getting hired" — 4 numbered differentiators (active instructors / 80% labs / NSTB prep / 90%+ placement)
7. Employer & agency partner marquee
8. **Course-finder quiz** — 3 questions → recommended course, deep-links (protect this; no competitor has it)
9. Instructor profiles (3 real instructors with credentials)
10. **Verified Graduate Registry** teaser lookup (SS-2026-001…004 demo IDs)
11. Testimonials (5-star cards)
12. Fees & Payment Options (5% upfront discount / 50-50 installment / scholarship)
13. Foreign-employment CTA banner (separate copy from general CTA)

## 3. Course detail template — the SEO money pages (SRS §7.3 implemented)

Each of the 10 course pages has, in order: breadcrumbs → H1 "[Course] Course in Nepal" → above-fold trust bar (CTEVT · NSTB · duration · certificate · placement) → overview → who-it's-for (local job / self-employment / abroad) → curriculum accordion (week-by-week modules) → duration & fee (real numbers + payment options) → eligibility → career outcomes w/ salary data → certificate & NSTB level mapping → 5-question FAQ (schema-marked) → sticky sidebar (inquiry form + gated brochure download + quick facts) → related courses. Real data: fees Rs 8,000–25,000, durations 6 weeks–3 months.

## 4. SEO implementation (live in code)

- Unique `<title>` + meta description per page/route (keyword-first patterns from SRS §6)
- JSON-LD per page type: Organization + LocalBusiness + WebSite (home) · Course + FAQPage + BreadcrumbList (all 10 course pages) · ItemList (courses hub) · FAQPage (certification, foreign employment) · BlogPosting (4 posts) · ContactPage + LocalBusiness (contact) · AboutPage + Organization (about) · 9× Review (success stories)
- One H1 per page, semantic H2/H3 hierarchy, breadcrumbs with schema, descriptive alt text
- Internal linking rule enforced: every course page links to category hub, certification page, foreign-employment hub, and 2–3 related courses; blog posts link to relevant courses
- FAQ accordions render full text in DOM (crawlable)

## 5. Content & data architecture (for the dev team)

All content lives in `src/data/*.ts` (courses, categories, batches, testimonials, instructors, registry, salary table, blog posts, site contact info) — a single source of truth designed for later CMS migration. Batch dates / seats-left are data-driven per SRS (never hardcode them in JSX). Forms are client-side functional (validation + success states) and ready to wire to CRM/WhatsApp Business API/GA4 events per SRS §9.3–9.4.

## 6. Design system (for the design team)

Tokens implemented in Tailwind: forest `#0E3B2E` · brand `#1C6B4C` · amber `#F2A93B` · mint `#EAF3EC` · ink `#16231C` · muted `#5B6660` · WhatsApp `#25D366`. Fonts: Sora (headings), Inter (body), IBM Plex Mono (eyebrow labels). 15 reusable components (CourseCard, BatchCard, StepCard, StatBlock, FAQAccordion, TestimonialCard, FilterPills, TrustBadgePill, SalaryTable, CTABanner, WhatsAppFab…). Motion: Lenis smooth scroll, GSAP scroll reveals, kinetic hero headlines, count-up stats — all with `prefers-reduced-motion` fallbacks. Full specs: `/mnt/agents/output/design/` (12 design docs).

## 7. Step-by-step for your teams

**Design team:** (1) open the preview and walk all 11 page types against `/mnt/agents/output/design/*.md`; (2) confirm brand font licensing (Sora/Inter vs licensed brand fonts); (3) swap placeholder photography with real campus/student photos when available (all images are in `public/`, referenced as `/<filename>`); (4) verify amber-on-white contrast per WCAG 2.1 AA (SRS §9.5).

**Dev team:** (1) confirm subdomain vs subfolder BEFORE launch (SRS §0 — biggest ranking lever); (2) wire forms to CRM with UTM retention + GA4 events (SRS §9.3); (3) point WhatsApp FAB to the real business number; (4) connect batch/seat data + Graduate Registry to a real database; (5) add XML sitemap + robots.txt at deploy; (6) set up Google Business Profile for New Baneshwar + Search Console (SRS §10.4); (7) Phase 2 course additions are already specced (Plumbing, Welding, Housekeeping, Childcare — SRS §14).

## 8. Source locations

- Website source (git repo): `/mnt/agents/output/app/` (master = delivered version `a246e7b`)
- Design documents (12 files): `/mnt/agents/output/design/`
- Research brief + all content data: `/mnt/agents/output/info.md`
