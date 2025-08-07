# TASKS — VEGAS IMPROV POWER HOMEPAGE (PLANNING PHASE)

> Measure twice, cut once. This list outlines tasks/subtasks for the homepage MVP. We will start implementation after confirming this plan.

## 1. Project Prep (Done / Verify)
- Confirm tech stack: Next.js 15, Tailwind v4, shadcn/ui
- Ensure `.docs/` is ignored in `.gitignore` (private working docs)
- Verify public assets: `public/logos/` light/dark logos
- Ensure `README.md`, `PRD.md`, `TASKS.md` exist and are accurate

## 2. Design Inputs (Private References)
- Review `/.docs/DESIGN-GUIDE.md`
- Review `/.docs/HOMEPAGE-OUTLINE.md`
- Extract tokens: colors, spacing, radii, motion
- Decide interim fonts vs final (licensing check)

## 3. IA & Content (MVP)
- Finalize section order and copy placeholders per PRD
- Identify CTAs and routes: `/classes`, `/corporate` (or anchors)

## 4. Component Plan
- Layout primitives: `Container`, `Section`, `SectionHeading`
- Header/Nav with logo variants and sticky behavior
- Hero block (headline, subcopy, dual CTAs, imagery placeholder)
- Feature cards (Classes, Corporate Workshops)
- Testimonials (MVP placeholder)
- Differentiators list
- Clients logo strip (placeholder)
- Blog highlights (MVP placeholder)
- Footer with dark theme and white logo variant

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
- Add placeholder content/images as specified

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

