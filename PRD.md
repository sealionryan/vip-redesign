# VEGAS IMPROV POWER — HOMEPAGE PRD

## Overview
Create a vibrant, professional homepage that communicates VIP’s unique Functional Improv® approach. The homepage must speak to both individual learners and corporate clients through a warm, creative, yet professional visual language. Use the lens: “Improv for Being a Human®”.

This document defines scope, goals, audiences, content, UX, visual direction, SEO, accessibility, and success criteria for the MVP homepage only.

## Goals
- Clearly communicate VIP’s value proposition (Functional Improv®, “Improv for Being a Human®”).
- Drive two primary CTAs: Explore Improv Classes, Corporate Workshops.
- Present brand ethos: warmth, creativity, professional edge.
- Be mobile-first responsive and performant.

## Non-Goals (Phase 1)
- Deep content buildout for subpages beyond basic links.
- Complex CMS integration.
- Advanced analytics/experimentation.

## Audiences
- Individuals seeking improv classes for personal growth.
- Corporate clients seeking workshops for teams (communication, adaptability, collaboration).

## Content & IA (MVP)
Sections (order is approximate; finalized in implementation):
1. Header / Navbar
   - Logo (light/dark variants in `/public/logos`)
   - Nav links: Classes, Corporate Workshops, About, Contact (anchors or routes)
   - CTA: "Explore Classes"
2. Hero
   - Headline communicating Functional Improv® and tagline lens
   - Subcopy focusing on outcomes: communication, confidence, adaptability, connection
   - Two primary CTAs: Explore Improv Classes, Corporate Workshops
   - Visual: hero image(s) per design guide
3. Unique Approach
   - Short bullets on Functional Improv® and real-world application
4. Featured Offerings
   - Two feature cards: Improv Classes, Corporate Workshops (links to respective pages)
5. Testimonials (MVP placeholder copy)
6. Why Choose VIP
   - 3–4 differentiators
7. Past Clients (logo strip placeholder)
8. Blog Highlights (MVP placeholder)
9. Final CTA
10. Footer

## Visual & Brand
Reference private docs (not committed):
- `/.docs/DESIGN-GUIDE.md`
- `/.docs/HOMEPAGE-OUTLINE.md`

Key notes:
- Colors: Purple `#4e4489`, Orange `#FFA77A`, neutrals per guide
- Use OKCLH for shade generation (future)
- Buttons: primary orange on light backgrounds; white-on-purple for footer/dark sections
- Glassmorphism on cards, subtle depth and animation (200–300ms ease-out)
- Fonts: Satoshi (headlines), Karma (body) — to be validated for licensing and delivery

## Accessibility
- Semantics for navigation, hero, sections
- Color contrast for buttons and text on purple/orange backgrounds
- Keyboard navigation for interactive components
- Respect reduced motion preferences

## Performance
- Optimize hero imagery (responsive images, modern formats where possible)
- Lazy-load non-critical assets
- Keep CLS low; avoid layout shift from fonts/images

## SEO (MVP)
- Page title, meta description
- Open Graph/Twitter tags (basic)
- Descriptive alt text for imagery

## Tech Constraints
- Next.js 15 (App Router)
- Tailwind v4
- shadcn/ui components (as needed)
- Public assets under `/public/`
- Keep private working docs under `/.docs/` (ignored by git)

## Success Criteria
- Homepage renders responsively and matches brand direction
- Clear dual-CTA path for Individuals vs Corporate
- Lighthouse: Performance > 85, Accessibility > 95, Best Practices > 95, SEO > 90 (MVP target)

## Risks & Mitigations
- Custom fonts licensing: validate before use; fallback to system/Google fonts temporarily.
- Image availability: use placeholders aligned with guide; swap later.
- Scope creep beyond homepage: defer to Phase 2 tasks.

## Phase 2 (Post-MVP) — Outline Only
- Component test coverage for critical UI
- Analytics and event tracking
- Structured content for blog highlights and testimonials
- Theming tokens with OKCLH scale

