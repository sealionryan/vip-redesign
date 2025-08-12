# TASKS — VEGAS IMPROV POWER HOMEPAGE (PLANNING PHASE)

> Measure twice, cut once. This list outlines tasks/subtasks for the homepage MVP. We will start implementation after confirming this plan.

## 1. Project Prep (Done / Verify)
- Confirm tech stack: Next.js 15, Tailwind v4, shadcn/ui
- Ensure `.docs/`, `.prd/`, `.serena/`, and `.old/` are ignored in `.gitignore`
- Verify public assets: `public/logos/` light/dark logos
- Ensure `README.md`, `PRD.md`, `TASKS.md` exist and are accurate

## 2. Design Inputs (Private References) ✓
- Review (skip any in /.docs/ subfolder, they are old, only use if needed for prior research) `/.docs/DESIGN-GUIDE.md` (historic) and `/.prd/DESIGN-GUIDE.md` (Webflow build) ✓
- Review `/.prd/HOMEPAGE-OUTLINE.md` ✓
- Extract tokens: colors, spacing, radii, motion ✓
- Fonts: Satoshi (variable font available in `public/fonts/`) + Karma (woff/woff2 available in `public/fonts/Karma-webfonts/`) ✓
- AI wireframe prototype created and validated ✓

## 3. IA & Content (MVP)
- Finalize section order and copy placeholders per PRD
- Identify CTAs and routes: `/classes`, `/corporate` (or anchors)

## 4. Component Plan
- Layout primitives: `Container`, `Section`, `SectionHeading`
- Header/Nav with logo variants and sticky behavior
- Hero block (H1 headline, subcopy, dual CTAs, imagery placeholder)
- Differentiators list (H2, subcopy, 3 cards with 16:9 thumbnail placeholder, excerpt, link to read more)
- Testimonials (H2, three cards, circular reviewer thumbnail, five yellow stars, review excerpt, circular review-site logo (Google, Yelp), and review date)
- Feature cards (H2, Improv Classes, Corporate Workshops)
- Clients logo strip (H2, placeholder logo strip)
- Blog highlights (H2, Webflow CMS-bound, 16:9 thumbnail image placeholders, article title, excerpt, link to read more)
- FAQs (Webflow CMS-bound or static shortlist per page)
- Footer with dark purple theme and white logo variant

## 5. Visual System (MVP)
- Color tokens in `globals.css` aligned with guide (Tailwind v4 inline tokens)
- Button variants (primary, secondary) using shadcn Button
- Card styles with glassmorphism (shadows, blur)
- Motion guidelines (200–300ms ease-out; reduced motion respect)

## 6. Implementation Tasks (to start after plan approval)
- Scaffold `src/components/` with planned components
- Implement responsive layout and sections per PRD
- Wire dual CTAs and anchor/route targets
- Integrate accessible navigation and focus states
- Add placeholder content/images as specified (rights-cleared or AI placeholders)

## 7. Accessibility & Performance (MVP)
- Semantic structure and ARIA where needed
- Contrast checks for purple/orange usages
- Responsive image sizes; lazy-load non-critical media

## 8. SEO (MVP)
- Metadata (title/description)
- Basic Open Graph/Twitter tags
- Alt text for imagery

## 9. QA Checklist
- Responsive pass: mobile, tablet, desktop
- Keyboard navigation and focus order
- Lighthouse pass (Perf >85, A11y >95, BP >95, SEO >90)

## 10. Phase 2 (Post-MVP) — Outline Only
- Unit tests for critical components and nav flows
- Analytics events for CTA clicks
- Content system for testimonials/blog highlights
- OKCLH shade generation and full theme tokens


