# VEGAS IMPROV POWER — HOMEPAGE PRD (AI‑READY)

## Objectives
- Communicate Functional Improv® through the lens “Improv for Being a Human®”.
- Serve two paths equally: Individuals (classes) and Corporate (workshops).
- Establish a warm, creative, professional visual tone aligned to brand.
- MVP only; fast, responsive, accessible.

## Non‑Goals (Phase 1)
- Full buildout of subpages, CMS, analytics/A/B testing.
- Advanced animation sequences; OKCLH shade system (Phase 2).

## Assets & Paths
- Logos (public):
  - Light backgrounds: `public/logos/2025-web-logo-header-main-transparent.png`
  - Dark backgrounds: `public/logos/2022-web-logo-header-white.png`
- Fonts (public):
  - `public/fonts/Satoshi-Variable.ttf`, `public/fonts/Satoshi-VariableItalic.ttf`
  - Body font Karma: defer until licensing/packaging; use system fallback in MVP
- Private references (not committed):
  - `/.docs/DESIGN-GUIDE.md`
  - `/.docs/HOMEPAGE-OUTLINE.md`
  - Appendix (verbose specs): `/.docs/PRD-APPENDIX.md`

## Information Architecture (MVP)
1) Header / Nav
   - Logo swap by section background (light vs dark)
   - Nav: Classes, Corporate Workshops, About, Contact (anchors or routes)
   - CTA: “Explore Classes”
2) Hero
   - Headline (≤ 10 words) + tagline reference
   - Subcopy (≤ 20 words) articulating outcomes: communication, confidence, adaptability, connection
   - 2 CTAs (exact text): “Explore Improv Classes”, “Corporate Workshops”
   - 1 hero image (placeholder acceptable)
3) Unique Approach
   - 3–4 bullets on Functional Improv® as real‑world application
4) Featured Offerings
   - 2 cards: Improv Classes, Corporate Workshops
   - Each: short description + 3–4 bullets + CTA
5) Testimonials
   - 3 testimonials: quote (≤ 100 words), attribution
6) Why Choose VIP
   - 3–4 differentiators (icon + title + 1–2 lines)
7) Past Clients
   - 6 logo placeholders
8) Blog Highlights
   - 3 posts (title, short excerpt, date, link)
9) Final CTA
   - Repeat dual CTAs
10) Footer
   - Dark section with white logo

## Components & Variants
- Header/Nav: sticky; glass on scroll; light/dark logo; primary CTA button
- Button (shadcn/ui):
  - Primary: bg orange‑700, hover orange‑800, text white
  - Secondary: white/transparent background, purple‑800 border/text
- Card: white/glassmorphic, radius consistent, layered soft shadows, hover lift (‑4px)
- Section primitives: `Container`, `Section`, `SectionHeading`
- Media: responsive images with proper alt; lazy where non‑critical

## Style Tokens (MVP)
- Colors
  - Purple `#4e4489`, Orange `#FFA77A`, White `#f2f2f2`, Black `#1f1f1f`
  - Tailwind v4 inline tokens in `src/app/globals.css`
  - OKCLH shade scale: Phase 2
- Typography
  - Headlines: Satoshi (variable) — bold/medium weights per section
  - Body: system fallbacks (Phase 2: Karma)
- Spacing & Containers
  - Base: 8px scale; section padding ~64–96px desktop, 48–64px mobile
  - Max width: 1280px; container padding 24/32/40 (mobile/tablet/desktop)
- Breakpoints
  - Mobile 320–767, Tablet 768–1023, Desktop 1024–1439, Large ≥1440

## Interactions
- Animation: 200–300ms ease‑out; buttons/cards hover lift; subtle content fade‑in
- Reduced motion: respect `prefers-reduced-motion` (disable transitions/scroll effects)

## Accessibility (WCAG 2.1 AA)
- Semantic landmarks and headings; keyboard navigable
- Contrast: ≥ 4.5:1 text; visible focus
- Alt text for informative images; decorative images hidden from a11y tree

## SEO (MVP)
- Title, meta description
- Basic Open Graph/Twitter tags
- Descriptive alt text; clean headings hierarchy

## Performance Targets
- Lighthouse: Perf > 85, A11y > 95, Best Practices > 95, SEO > 90
- LCP < 2.5s, CLS < 0.1; lazy‑load non‑critical media

## Acceptance Checklist (Binary)
- [ ] Header/nav with logo swap and primary CTA
- [ ] Hero renders with headline (≤ 10 words), subcopy (≤ 20 words), 2 CTAs
- [ ] 2 offering cards each with 3–4 bullets and CTA
- [ ] Testimonials (3) and Differentiators (3–4) present
- [ ] Past clients (6 logos) and Blog highlights (3 posts)
- [ ] Final CTA section and dark footer with white logo
- [ ] Keyboard nav passes; visible focus; contrast meets targets
- [ ] Title/meta present; OG/Twitter placeholders
- [ ] LCP/CLS within targets on local test imagery

## Phase 2 (Post‑MVP) — Outline
- OKCLH shade system and design tokens expansion
- Analytics/events; test coverage for critical UI flows
- Rich content for testimonials/blog; advanced hero animation

Notes: verbose copy examples, animation sequences, and extended image specs live in `/.docs/PRD-APPENDIX.md` (local only).

