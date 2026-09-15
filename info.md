# Research & Content Brief — technical.skillshikshya.com

This brief consolidates: (1) the completed SEO/competitor research report, (2) the SRS page-by-page spec, (3) all real content data extracted from the existing prototype screenshots, (4) the design system tokens. Build the FULL site from this — it is the single source of truth.

---

## 0. Brand & Business Context

**SkillShikshya Technical** — hands-on technical & vocational training institute, New Baneshwar, Kathmandu, Nepal. CTEVT-affiliated (Reg. No. 2018-KTM-0421), NSTB Partner, Ministry of Labour & Employment accredited. Operating since 2018. Outcome = a job or self-employment (not portfolio projects). Distinct from SkillShikshya's IT-course vertical.

**Three non-negotiable trust markers visible above the fold on every course page** (every Nepal competitor leads with these):
1. CTEVT affiliation
2. NSTB Skill Test alignment (Level 1 & 2)
3. Placement support

**Key stats:** 2,000+ graduates · 90%+ placement rate · 10 trade courses · 7+ countries hired · Since 2018.

**Contact:** New Baneshwar, Kathmandu (Opposite Civil Hospital) · Phone 01-4000000 / 9800-000-000 · hello@skillshikshya.com · Sun–Fri 9am–5pm.

**Employer & agency partners:** Vrit Technology, Gulf Manpower Pvt., Israel G2G Agency, Himalayan Java, Al-Khobar Contracting.

---

## 1. Site Architecture (full page inventory — build ALL of these)

- `/` — Homepage
- `/courses/` — All Courses hub (category browser + filter pills)
- `/courses/[slug]/` — Course Detail template ×10 courses:
  - Beauty & Wellness: `nail-art-training`, `makeup-beautician-course`, `hair-styling-course`, `barber-training`
  - Construction & Electrical: `electrician-training`, `carpentry-training`
  - Hospitality & Culinary: `barista-training`, `baking-pastry-course`, `bartending-course`
  - Care Services: `elderly-caregiver-training`
- `/foreign-employment-preparation/` — the single biggest keyword opportunity; dedicated hub
- `/skill-test-and-certification/` — CTEVT & NSTB explainer (trust page)
- `/corporate-and-group-training/` — B2B, proposal form
- `/success-stories/` — testimonials grouped by trade category
- `/graduate-registry/` — Verified Graduate Registry lookup tool (certificate ID verification)
- `/blog/` — index + 4 full sample posts:
  - `how-to-get-nstb-skill-test-certificate-nepal`
  - `top-10-skills-in-demand-for-foreign-employment-nepal`
  - `electrician-vs-plumber-which-trade-pays-better-nepal`
  - `best-career-options-after-see-without-plus-two`
- `/about/`
- `/contact-and-counseling/` — primary conversion page

**Global/persistent elements (every page):** sticky WhatsApp FAB bottom-right; top nav (Courses · Foreign Employment · Certification · Success Stories · Corporate Training · About · phone · "Free Counseling" CTA); footer with course category links, site nav, contact block, CTEVT-registered-centre badge line; dark CTA banner before footer.

---

## 2. Full Course Data (use exactly — from prototype)

| Course | Slug | Category | Duration | Fee (NPR) | Badge | Description |
|---|---|---|---|---|---|---|
| Nail Art Training | nail-art-training | Beauty & Wellness | 6 Weeks | 8,000 | Popular | Covers gel extensions, acrylic shapes, 3D nail art designs, overlays, and fill-ins. |
| Makeup & Beautician | makeup-beautician-course | Beauty & Wellness | 3 Months | 15,000 | Abroad Ready | Comprehensive bridal makeup, skin treatments, hair styling, and salon safety. |
| Hair Styling Course | hair-styling-course | Beauty & Wellness | 2 Months | 10,000 | — | Professional hair cutting techniques, color treatments, perming, and straightening. |
| Barber Training | barber-training | Beauty & Wellness | 2 Months | 10,000 | — | Classic and modern men's hair grooming, beard trimming, styling, and hygiene standards. |
| Electrician Training | electrician-training | Construction & Electrical | 3 Months | 15,000 | Highly Popular | Domestic house wiring, safety protocols, industrial panels, and motor repair basics. |
| Carpentry Training | carpentry-training | Construction & Electrical | 3 Months | 14,000 | — | Traditional and modular wood construction, power tools, safety, and blue-print designs. |
| Barista Training | barista-training | Hospitality & Culinary | 1 Month | 9,000 | High Demand | Espresso extraction, latte art styles, coffee grinding, machine cleaning, and service soft skills. |
| Baking & Pastry | baking-pastry-course | Hospitality & Culinary | 2 Months | 12,000 | — | Commercial breadmaking, cakes, basic cookies, pastries, desserts, and kitchen safety. |
| Bartending Course | bartending-course | Hospitality & Culinary | 1 Month | 9,000 | — | Mixology principles, cocktail preparation, bar equipment management, speed-pouring, and customer service. |
| Elderly Caregiver | elderly-caregiver-training | Care Services | 3 Months | 25,000 | Israel/Japan Ready | Elderly health monitoring, mobility support, first aid/CPR, hygiene, and caregiver soft skills. |

Category intros:
- Beauty & Wellness: "Gain practical training in salon work, advanced makeup, and styling. Built for local self-employment, beauty clinic roles, or starting your own salon business." (4 courses · from Rs 8,000)
- Construction & Electrical: "Our highest demand trade category for foreign employment. Focuses on practical house wiring, motor repair, and industrial electrical work mapped to Level 1 & 2 exams." (2 courses · from Rs 14,000)
- Hospitality & Culinary: "Learn coffee craft, baking, and beverage chemistry. Prepares graduates for barista or kitchen jobs in popular cafes and resorts in Nepal or overseas." (3 courses · from Rs 9,000)
- Care Services: "Gain essential skills in nursing care, elderly care, and basic first aid. Highly recommended for students preparing for G2G programs to Israel, UK, or Japan." (1 course · Rs 25,000)

**Upcoming batches (August 2026):** Electrician Training — starts Aug 1, 2026 · 3 months · morning & evening shifts · Only 8 seats left. Makeup & Beautician — starts Aug 5, 2026 · 3 months · day and evening batches · Only 5 seats left. Elderly Caregiver — starts Aug 10, 2026 · 3 months · G2G Israel/Japan pathway included · Only 6 seats left.

---

## 3. Homepage section order (from SRS §7.1 — keep everything the prototype does right)

1. Hero — "Learn a skill. Get certified. Get hired." + subcopy ("Hands-on training in electrical work, beauty, hospitality and care services — with CTEVT & NSTB-recognized certification. 90%+ placement rate since 2018.") + trust pills (CTEVT Affiliated · NSTB Level 1 & 2 · 2,000+ Placed · Since 2018) + inline "Get Free Career Counseling" card form (full name, phone, course of interest select, "Request Free Counseling" button, "We respond within 1 hour on working days", badge "Next Batch Starts: August 1, 2026 — Limited seats!") + CTAs "Find your course" / "Browse all 10 courses" + stat row (2,000+ graduates · 90%+ placement · 10 trade courses · 7+ countries hired) + "Officially accredited by" strip (CTEVT — Council for Technical Education · NSTB — National Skill Testing Board · Ministry of Labour & Employment)
2. Upcoming Batch Dates banner (dark) — "Upcoming Batch Dates — August 2026", 3 batch cards with seats-left warning bars, "Reserve Your Seat" button
3. "Pick your trade field" — 4 icon-led category tiles with course counts + from-price
4. "What you can earn after training" — salary table (see §4)
5. "Built around getting hired, not just attending class" — 4 numbered blocks: 01 Active Trade Instructors (currently working electricians, chefs, beauticians — not retired academics) · 02 80% Practical Labs (real tools, real workshop hours, real café simulators) · 03 NSTB Exam Prep (curriculum maps directly to the NSTB practical exam required for foreign employment visas) · 04 90%+ Placement Rate (employer network of 30+ companies and manpower agencies)
6. Employer & Agency Partners logo row
7. Course-finder quiz — "Find the perfect course in 60 seconds" — 3-step interactive quiz (career goal → timeframe → interests) that recommends a course and deep-links to it. Q1 options: Work Abroad (Gulf, Japan, Europe) / Get a job locally in Nepal / Start my own business / salon / cafe
8. Instructors — "Your instructors — active trade professionals": Er. Suraj Khadka (Electrical Engineering, 14 yrs exp — licensed electrical engineer, wired 200+ commercial & residential projects in Kathmandu Valley, NSTB Level 2 examiner) · Sunita Maharjan (Beauty & Cosmetics, 10 yrs exp — award-winning salon owner, Glow Studio Lazimpat; CIBTAC UK and CIDESCO certified; 800+ students trained) · Barista Suman Lama (Coffee Science & Hospitality, 8 yrs exp — SCA-certified Barista Instructor, former head barista at Himalayan Java, specialty coffee consultant for 6 Kathmandu cafés)
9. Verified Graduate Registry — lookup tool (Certificate ID → verified graduate profile). Sample IDs: SS-2026-001 Ramesh Tamang (Electrician, Saudi Arabia) · SS-2026-002 Sabina Gurung (Beautician, KTM Salon Owner) · SS-2026-003 Anish Shrestha (Barista, Himalayan Java) · SS-2026-004 Pooja Rai (Caregiver, Israel G2G)
10. "What our graduates say" — 3 testimonial cards with 5 stars (see §5)
11. Fees & Payment Options — 3 cards: Full Upfront Payment (5% OFF, covers all lab materials) · 50/50 Installment (MOST POPULAR — pay 50% at enrollment, 50% after week 4, no interest, no paperwork, no credit check) · Scholarship/Waiver (government-sponsored or NGO-matched training slots, up to FREE, limited seats, income assessment required)
12. Foreign-employment CTA banner (dark green) — "Planning to work abroad? Get NSTB certified before you apply for skilled jobs in the Gulf, Malaysia, Croatia, or Japan." + "See Foreign Employment Prep" / "Talk to a counselor"
13. Footer

---

## 4. Salary table (homepage "What you can earn after training")

Disclaimer: "These salary ranges are based on actual employer data and graduate reports from our Batch 2024–2026 graduates. Local estimates are for Kathmandu Valley."

| Trade | Local (Nepal) | Gulf (Qatar/UAE) | Europe (Croatia/Romania) | Japan G2G |
|---|---|---|---|---|
| Electrician | Rs 25,000–45,000/mo | QAR 1,200–1,800/mo | €1,400–2,200/mo | — |
| Beautician | Rs 20,000–40,000/mo | AED 1,500–2,500/mo | — | — |
| Caregiver | Rs 18,000–30,000/mo | — | — | ¥200,000–260,000/mo |
| Barista | Rs 18,000–28,000/mo | AED 1,200–2,000/mo | — | — |

---

## 5. Testimonials (Success Stories page + homepage carousel)

Construction & Electrical:
- "After finishing electrician training here, I passed my skill test and now work in Saudi Arabia as a wiring tech. The hands-on workshop hours made all the difference." — Ramesh Tamang, Electrician Training (Saudi Arabia)
- "I built three houses' wiring on my own within six months of finishing the course. I'm now a local residential wiring contractor in Lalitpur." — Suresh Rai, Electrician Training (Lalitpur)
- "The carpentry workshop hours made the biggest difference — real practice on power tools, not just boring classroom theory slides." — Bikash Thapa, Carpentry Training (Kathmandu)

Beauty & Wellness:
- "I always wanted my own beauty studio. This advanced beautician course gave me the confidence and the CTEVT certificate to register my business." — Sabina Gurung, Rose Beauty Salon Owner (Kathmandu)
- "Nail art felt like a hobby before — now it's a real income for me. I run home-visit nail extensions services and make a solid monthly living." — Puja Maharjan, Nail Art Training (Kathmandu)
- "I do bridal hair styling and coloring treatments for three major salons in my neighborhood. Fully booked every wedding season!" — Nirmala K.C., Hair Stylist (Kathmandu)

Hospitality & Culinary:
- "I learned baking and pastry operations here. Today, I supply artisanal sourdough bread and custom birthday cakes to three cafes in Kathmandu." — Anish Shrestha, Baking & Pastry Graduate (Kathmandu)
- "Passed my barista job interview the week after finishing the course. I'm currently working at a popular coffee chain in Koteshwor." — Sandesh Lama, Barista Graduate (Kathmandu)

Care Services:
- "The care training prepared me well for working with elderly families in Israel. The certificate was officially processed by the G2G agency." — Kamala Adhikari, Caregiver (Israel G2G Scheme)

Homepage 3-card versions: Ramesh Tamang ("…now work in Saudi Arabia earning 4× what I would have locally"), Sabina Gurung ("The beautician course changed my life. I opened my own salon 3 months after graduating and now have 12 regular clients per day."), Anish Shrestha ("The barista course was intense and practical. The mock café sessions were exactly like working in a real coffee shop.") — all 5 stars.

---

## 6. Page-by-page specs (condensed from SRS §7 — follow exactly)

### /courses/ hub
- Hero: "Skill-focused Training Courses" + "Every course is heavily hands-on, CTEVT affiliated, and maps directly to National Skill Testing Board (NSTB) level certifications. Choose your career path below."
- Client-side filter pills: Show All Courses / Beauty & Wellness / Construction & Electrical / Hospitality & Culinary / Care Services
- Category sections with eyebrow "— CATEGORY", intro copy, course cards (gradient image header w/ badge, title, description, duration + fee row, "View Course Details" link)

### Course detail template (/courses/[slug]/) — repeat for all 10
H1: "[Course Name] Course in Nepal". Sections in order:
1. Trust bar above fold (icon row): CTEVT Affiliated · NSTB Level mapping · Duration · Certificate included · Placement support
2. Overview (150–200 words, keyword-rich)
3. Who this is for — 3 tracks: local job seeker / self-employment / foreign-employment prep
4. Curriculum breakdown by week/module (write realistic 4–8 module breakdown per course)
5. Duration & fee — real numbers from §2, payment options recap
6. Eligibility — "No formal education requirement" or "SEE passed preferred"
7. Career outcomes — local salary range (from §4) + abroad placement note
8. Certificate & Skill Test info — which NSTB level it maps to
9. FAQ block (5 questions — the standard pattern: duration / fee / qualification / certificate recognized for foreign employment / salary after course)
10. Sticky sidebar inquiry form (desktop) + WhatsApp button priority on mobile; gated "Download Brochure" (name/phone/email capture → success state)
11. Related courses (same category + cross-category abroad-ready)
Breadcrumbs: Home / Courses / [Category] / [Course]

### /foreign-employment-preparation/
- Hero: "Get Skill-Test Ready for Work Abroad" + "Planning to apply for skilled jobs in the Gulf, Malaysia, Croatia, Romania, or Japan? Learn how our NSTB skill test training gives you a critical competitive advantage." + "Book Free Counseling Session"
- "How the Skill Certification Process Works" — 4 numbered steps: 01 Enroll in Trade Training (complete 390 hours of practical trade training in our Baneshwar workshop labs) · 02 NSTB Skill Prep (practice with mock testing formats designed by National Skill Testing Board assessors) · 03 Pass the Skill Test (earn your Level 1 or Level 2 NSTB qualification card) · 04 Apply with Confidence (present a verified government credential to manpower agencies and embassy visa officers)
- "Why the NSTB Card Matters" — wage callout: "The NSTB card is the primary proof of trade competency recognized by foreign governments and manpower companies. Having this card makes you eligible for higher-tier skilled wages, which can be 50% to 100% higher than general helper wages." + "Gulf & European Demands" card: "Countries like Romania, Poland, Croatia, Saudi Arabia, and UAE have established visa requirements verifying skill certifications. Having an NSTB Level 1/2 qualification is the fastest way to pass these checks."
- "Our Abroad-Ready Courses" grid — Electrician (Highly Popular), Carpentry, Elderly Caregiver (Israel/Japan), Makeup & Beautician
- "Key Markets for Certified Grads" — Gulf States (Saudi Arabia, Qatar, UAE) · East Europe (Croatia, Romania, Poland) · Israel Caregiver (G2G schemes, specialized home nursing) · Japan SSW (Specified Skilled Worker)
- FAQ + CTA banner

### /skill-test-and-certification/
- Hero: "Understanding CTEVT & NSTB Systems" + "These two acronyms are essential for technical and vocational training credentials in Nepal. Learn what they mean and how they affect your career prospects in Nepal or abroad."
- Two cards: CTEVT Affiliation ("The Council for Technical Education and Vocational Training (CTEVT) is the national government body regulating vocational training in Nepal…") + The NSTB Skill Test ("The National Skill Testing Board (NSTB) conducts physical, practical exams to certify individual trade workers…")
- "CTEVT & NSTB Benefits at a Glance" — National Database / Government Verified / Manpower Approved / Lifetime Credential
- "Common Certification FAQs" accordion: Do I get a certificate on course completion? / What is the difference between CTEVT and NSTB? / Is the NSTB exam compulsory? / Where is the NSTB exam conducted?
- CTA: "Confused about visa certificate requirements? Let our counselors explain exactly which certificate (CTEVT or NSTB) you need based on your target country." + "Talk to a counselor for free"

### /corporate-and-group-training/
- Hero: "B2B & Group Vocational Training" + "Upskill your restaurant crew in specialty barista work, your construction team in advanced electrical wiring, or your care home staff in modern caregiver practices."
- "Institutions, Businesses, and NGOs" — Hotels & Cafes (specialty espresso extraction, sensory training, service soft skills) · Construction Firms (National Electric Code wiring, safety, equipment operation) · NGOs & Agencies (tailored vocational batches for community empowerment projects) · Care Providers (professional caregiver cohorts, G2G syllabus standard)
- "How to Set Up a Custom Batch" — 4 steps: Identify Skill Gap / Custom Curriculum / Practical Training / Certification & Audit
- "Request Corporate Training Proposal" form: Organization Name, Contact Person Name, Contact Phone Number, Skill Area of Interest (select), Approximate Cohort Size, "Submit Request for Proposal" — "Our manager will reply within 1 business day."

### /success-stories/
- Hero: "Real Graduates, Real Placements" + subcopy; testimonial cards grouped by category (data in §5); CTA banner "Want to be our next success story? Schedule a quick, free call with our career counseling office today." + "Request Counseling Callback"

### /graduate-registry/
- "Verified Graduate Registry" — explanation for employers/manpower agencies; lookup by Certificate ID; sample IDs listed; result card shows name, trade, graduation status, NSTB level, placement (client-side mock against the 4 sample records + graceful "not found" state)

### /blog/ + 4 posts
Blog index: filterable by category, cards with title/excerpt/date/read-time. Posts (write full, real, useful articles 800–1200 words each, with H2/H3 structure, FAQ block, and inline CTAs to relevant course pages):
1. "How to Get an NSTB Skill Test Certificate in Nepal" (step-by-step: eligibility → training hours → application → exam day → certificate)
2. "Top 10 Skills in Demand for Foreign Employment from Nepal" (electrician, caregiver, welder, plumber, barista, carpenter… with destination mapping)
3. "Electrician vs Plumber: Which Trade Pays Better in Nepal?" (salary table comparison, abroad demand, training cost/duration)
4. "Best Career Options After SEE Without +2" (vocational pathway framing, course recommendations, timelines)

### /about/
- Hero + mission; story since 2018; affiliation & accreditation badges (CTEVT Reg. No. 2018-KTM-0421, NSTB Partner, Ministry of Labour & Employment); team/instructor profiles; facility/location info; stats band.

### /contact-and-counseling/
- Hero: "Connect with Our Career Counselors" + "Have questions about fee structures, upcoming batch dates, or G2G caregiver exam registration? Reach out for a free, zero-obligation callback."
- "Request Callback" form: Full name, Phone number, Course of interest (select incl. "Not sure yet — help me decide"), Preferred contact time (Morning 9–12 etc.), "Request Free Callback"
- "Training Location & Details" — Office phone 01-4000000 · Email hello@skillshikshya.com · Location New Baneshwar, KTM · Working days Sun–Fri 9am–5pm · "Chat instantly on WhatsApp" green button · map placeholder card "SkillShikshya Technical Center, Opposite Civil Hospital, New Baneshwar, Kathmandu"

---

## 7. SEO spec (implement in code)

- Unique `<title>` + meta description per page, primary keyword first. Use a small SEO helper (set document.title + meta tags per route).
- Title patterns: Homepage "SkillShikshya Technical — Vocational Training Institute in Kathmandu, Nepal | CTEVT & NSTB Certified"; Course pages "[Course] Course in Nepal — CTEVT Certified Training | SkillShikshya Technical"; etc.
- JSON-LD schema per page type: Organization+LocalBusiness+WebSite (home), Course+FAQPage+BreadcrumbList (course details), ItemList+BreadcrumbList (courses hub), FAQPage+BreadcrumbList (certification, foreign employment), BlogPosting (posts), ContactPage+LocalBusiness (contact), AboutPage+Organization (about), Review (success stories).
- Semantic HTML: one H1 per page, proper H2/H3 hierarchy, breadcrumb nav, descriptive alt text (e.g. "electrician student practicing house wiring, Kathmandu").
- Internal linking rule: every course page links to its category hub section, the certification page, the foreign-employment hub (where relevant), and 2–3 related courses.

### Keyword map (primary per page)
- Home: vocational training institute Nepal / technical training Kathmandu
- Courses hub: vocational courses Nepal / skill training courses Kathmandu
- Electrician: electrician training in Nepal / electrician course in Kathmandu (long-tail: house wiring course Kathmandu, electrician course for Gulf job)
- Carpentry: carpentry training in Nepal (furniture making course Kathmandu, carpentry training for foreign employment)
- Makeup & Beautician: beautician course in Nepal / makeup course in Kathmandu (bridal makeup course Kathmandu, salon business course Nepal)
- Nail Art: nail art course in Nepal (gel nail extension training Nepal, nail art course for beginners)
- Hair Styling: hair styling course in Nepal (hair coloring course Kathmandu) · Barber: barber training in Nepal
- Barista: barista training in Kathmandu / barista course Nepal (espresso latte art course Kathmandu, barista training for Gulf hotel job)
- Baking & Pastry: baking and pastry course in Kathmandu (cake making classes Nepal, pastry chef training Nepal)
- Bartending: bartending course in Nepal (mixology training Kathmandu)
- Elderly Caregiver: elderly care training in Nepal / caregiver course in Nepal (caregiver course for Israel job Nepal, caregiver training G2G Nepal)
- Foreign employment hub: NSTB skill test Nepal / skill test certificate for foreign employment Nepal (skill test for Qatar/Malaysia/Saudi visa, Japan SSW skill test Nepal, Korea EPS)
- Certification: CTEVT NSTB certification Nepal (difference between CTEVT and NSTB, NSTB skill test fee)
- Corporate: corporate vocational training Nepal (group skill training company Nepal, NGO vocational training partner Nepal)
- Blog posts: as titled.

---

## 8. Design system (from prototype — match closely)

**Colors:** deep forest green `#0E3B2E` (header/footer/dark sections) · brand green `#1C6B4C` (primary buttons, links, active states) · amber `#F2A93B` (secondary CTAs, badges "Popular"/"Highly Popular", highlight underlines) · mint tint `#EAF3EC` (alternate section bg) · white cards · near-black-green text `#16231C` · muted `#5B6660`. WhatsApp green `#25D366` for the FAB/chat button.

**Typography:** Headings — bold slightly-rounded geometric sans (Sora or Poppins, heavy weights, tight tracking). Body — Inter 16px/1.6. Eyebrow micro-labels — monospace, uppercase, letter-spaced, small (e.g. "— WHERE TO START", "— CAREER OUTCOMES", "CATEGORY") in muted/amber.

**Signature components (formalize & reuse):** trust badge pill (CTEVT/NSTB/ISO with icon) · course card (dark-green diagonal-stripe gradient image header, amber badge chip top-right, title, description, duration+fee row, text link) · numbered step card (amber number, bold title, description, soft border) · stat block (big number + small caps label, divider-separated) · FAQ accordion · testimonial card (quote, 5 amber stars, name/trade/location footer) · sticky CTA sidebar (course detail, desktop) · full-width dark CTA banner with amber button before footer · sticky WhatsApp FAB bottom-right · batch card (dark green, category eyebrow, title, start/duration lines, amber "only N seats left" warning bar) · form inputs (white, soft border, rounded-xl, label above).

**Layout patterns:** max-w-6xl/7xl centered containers, generous vertical rhythm (py-16/24), alternating white / mint-tint sections, dark-green banner sections with subtle diagonal stripe texture, rounded-2xl cards with soft borders and shadows.

**Responsive:** mobile-first; 375/768/1024 breakpoints; course grids 1/2/3-4 cols; sticky sidebar desktop-only (mobile: WhatsApp FAB + in-flow form).

---

## 9. Functional requirements (mock but functional client-side)

- Counseling/inquiry forms: multi-step feel, validation, success state ("We'll call you back within one business day").
- Course-finder quiz: 3 questions → recommended course card with link.
- Graduate Registry: client-side lookup against the 4 sample records; not-found state with guidance.
- Courses filter pills: client-side filtering.
- FAQ accordions: fully rendered in DOM (crawlable), expand/collapse.
- Batch seats-left bars: data-driven from a courses/batches data file (src/data/), not hardcoded in JSX — so the dev team can later wire to CMS.
- WhatsApp FAB: links to https://wa.me/9779800000000 with pre-filled text.
- All course data, testimonials, instructors, blog posts live in `src/data/*.ts` files (single source of truth for future CMS migration).

## 10. Assets to generate (image generation tool)

1. `hero-workshop.png` — wide hero image: bright modern vocational training workshop in Kathmandu, students practicing electrical wiring and carpentry, warm natural light, green/amber accents, photorealistic
2. `course-electrician.png`, `course-carpentry.png`, `course-beautician.png`, `course-nailart.png`, `course-hairstyling.png`, `course-barber.png`, `course-barista.png`, `course-baking.png`, `course-bartending.png`, `course-caregiver.png` — 4:3 card images per course (hands-on training scenes, consistent warm photoreal style)
3. `instructor-suraj.png`, `instructor-sunita.png`, `instructor-suman.png` — portrait photos of Nepali trade instructors (professional, friendly, workshop/salon/café backdrop)
4. `about-campus.png` — training center exterior/classroom in New Baneshwar Kathmandu
5. `foreign-employment.png` — Nepali skilled worker at airport with toolkit, hopeful departure mood
6. `blog-nstb.png`, `blog-foreign-skills.png`, `blog-electrician-plumber.png`, `blog-after-see.png` — blog cover images
7. `category-beauty.png`, `category-construction.png`, `category-hospitality.png`, `category-care.png` — category tile images
8. `og-image.png` — 1200×630 brand share image
