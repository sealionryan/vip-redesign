# Vegas Improv Power — Style Guide (Relume/Webflow Oriented)

## Brand Essence
A modern, premium, and approachable improv company aesthetic that balances **professional refinement** with **creative warmth**.
The design should feel **light and airy like Apple**, yet carry **playful energy** and **depth** through subtle textures, gradients, and atmospheric color details inspired by Stripe.
Every element should feel **intentional, uncluttered, and inviting**, with space for the content to breathe.

---

## Color System

### Brand Colors
- **Purple**: `--vip-purple-700` (brand base)
- **Orange/Peach**: `--vip-orange-400` (brand base)
- **White**: `#f2f2f2`
- **Black**: `#1f1f1f`

### Color Shades (Use OKLCH for even distribution)
OKLCH shade scale implemented (50-950) for purple and orange:
- **50, 75, 100, 200, 300, 400, 500, 600, 700, 800, 900, 925, 950**
  - 50–100: Very light backgrounds
  - 200–400: Light UI elements
  - 700: Brand purple, 400: Brand orange
  - 600–800: Darker variations
  - 900–950: Text and dark backgrounds

### Application Patterns
- **Primary sections**: White or Purple-50/75 backgrounds with high-contrast text
- **CTAs/Buttons**: Orange-400 (brand) background with white text for high visibility
- **Footer**: Purple-900/950 background with white text
- **Cards**: White (#f2f2f2) with soft shadows and/or subtle gradients
  - Optional micro-glass for callouts (blur 12–16, 1px white border at 12–16% opacity)
  - Allow section split-bands and blurred color blobs per `.prd/DESIGN-GUIDE.md`

### New Background Treatments
- **Blurred Color Highlights:** Large, super-soft blobs in brand colors behind hero areas, feature blocks, or CTAs (opacity 8–15%, heavy Gaussian blur)
- **Subtle Gradients:** Replace flat blocks with two-tone gradients of the same hue (e.g., Purple-500 → Purple-400) or brand color + soft neutral
- **Noise/Grain Overlay:** Ultra-fine texture at low opacity for depth
- **Motif Patterns:** Low-opacity improv-inspired shapes (lines, dots, wave forms) applied sparingly to create character

---

## Typography

### Fonts
- **Headlines:** Satoshi (variable font)
  - H1 & H2: Bold/Heavy weight
  - H3 & H4: Medium weight
  - H5 & H6: Regular weight
- **Body Text:** Karma (serif, regular weight) — now available in `/public/fonts/Karma-webfonts/` (woff/woff2)

### Hierarchy
- Clear, decisive size scaling between headings
- Large hero headlines (H1 ~3–4rem)
- Comfortable line height (~1.5–1.7) for body text
- Maintain visual contrast between headline and body font styles

---

## Visual Elements

### Logo Usage
- **Light backgrounds:** Purple or full-color logo
- **Dark backgrounds:** White logo
- Keep sizing consistent across nav and footer

### Cards & Containers
- Rounded corners (consistent radius, 12–16px)
- Multiple soft shadows for depth
- White or very light gradients for background fill
- Glassmorphic accents **only** for special areas (highlighted info, callouts)

### Buttons
- **Primary:** Orange-400 (brand) with white text, hover to orange-500
- **Secondary:** White background with Purple-800 text, subtle shadow
- Gentle lift and shadow deepen on hover

---

## Image Strategy

### Hero Section
- Large featured image or collage
- Option for blurred brand-colored background shapes behind hero content
- Maintain movement and human connection

### Content Distribution
- **Top of page:** Strong imagery + gradients/blurred highlights
- **Middle:** Balanced text and imagery with modular cards
- **Bottom:** Content-focused, lighter visual weight

### Image Guidelines
- Candid, high-energy moments (rights cleared). AI placeholders ok pre‑final.
- Abstract or atmospheric fillers for variety
- Avoid stock-photo stiffness
- Keep tones consistent with brand colors

---

## Layout Patterns

### Sections
- **Hero:** Bold headline, subtle gradient background, blurred color highlights, clear CTAs
- **Services:** 3-column grid on desktop, stacked on mobile
- **Testimonials:** Carousel or 2–3 column grid
- **Offerings Split:** Two feature blocks (Classes + Corporate) with contrasting bg band
- **Blog Highlights:** 3 cards tied to Webflow CMS
- **FAQ:** Accordion (Webflow CMS or static)
- **Footer:** Dark purple with structured link groups

### Spacing
- Base spacing unit: 8px, scaled generously for large sections (e.g., 96px top/bottom)
- More negative space around key elements to maintain airy feel

---

## Animation Guidelines

### Key Animations
- **Page load:** Fade in with slight upward motion
- **Hover states:** Gentle lift and shadow emphasis
- **Background blobs:** Slow, subtle drift or parallax
- **Hero transitions:** Smooth fades or directional light sweeps
  - Respect reduced motion (turn off parallax)

### Principles
- Animation supports content, never distracts
- Consistent duration: 200–300ms, ease-out
- Respect reduced motion preferences

---

## Component Patterns

### Navigation
- Light background with purple text or dark background with white text
- Slight transparency with blur on scroll
- Active state: underline or orange highlight

### Hero Section
- Large Satoshi Bold headline
- Layered backgrounds: gradient + blurred blob + optional pattern
- Orange primary CTA and secondary outlined CTA

### Service Cards
- White or light gradient background
- Hover lift and soft shadow
- Clear title → short description → action hierarchy

### Footer
- Dark purple background
- White text and logo
- Organized columns for nav, contact, and signup

---

## Webflow + Relume Notes (MVP)
- Use Relume Style Guide page to set tokens (colors, type, radii, spacing).
- Preferred components for homepage: Navbar 1, Hero 26/29, Features 15, Testimonials 8, Features Split 6, Logos 4, Blog Cards 5, FAQ Accordion 2, CTA 7, Footer 3.
- See `/.prd/DESIGN-GUIDE.md` for step-by-step assembly and CMS bindings.

---

## Visual Personality
Imagine walking into a **beautiful, modern creative space** — light-filled, well-designed, full of energy, yet calm and uncluttered.
This is a space where ideas flow easily, conversations spark, and everyone feels welcome.
The look should feel premium without pretension, playful without chaos, and full of subtle visual details that reward a second glance.