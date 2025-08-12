# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Context

This is the Vegas Improv Power (VIP) homepage redesign **prototyping and wireframing environment**. Use this Next.js application to rapidly build mockups, test UI patterns, and explore design concepts that will inform the final website build.

The project embodies VIP's "Functional Improv®" approach with the tagline "Improv for Being a Human®". Focus on visual experimentation and user experience testing rather than production-ready code.

## Development Commands

**Always use `pnpm` (not `npm`):**
- `pnpm dev` — Start development server (localhost:3000)
- `pnpm build` — Build production application
- `pnpm start` — Start production server
- `pnpm lint` — Run ESLint

## Project Architecture

This is a Next.js 15 application using the App Router architecture.

### Tech Stack
- Framework: Next.js 15 (App Router)
- Styling: Tailwind CSS v4 with CSS variables
- UI Components: shadcn/ui (new-york)
- Icons: Lucide React
- TypeScript: strict

### Project Structure
- `src/app/` — App Router pages/layouts
- `src/lib/` — Shared utilities (includes `cn` helper)
- `src/components/` — Reusable components (shadcn in `src/components/ui/`)
- `public/` — Static assets (logos, fonts)
- `PRD.md` — Product Requirements Document
- `TASKS.md` — Development tasks and progress
- `/.docs/`, `/.prd/` — Private design docs (git-ignored)

### Key Asset Paths
- **Logos:**
  - Light backgrounds: `public/logos/2025-web-logo-header-main-transparent.png`
  - Dark backgrounds: `public/logos/2022-web-logo-header-white.png`
- **Fonts:**
  - Headlines: `public/fonts/Satoshi-Variable.ttf` (and Italic variant)
  - Body: `public/fonts/Karma-webfonts/` (woff/woff2 files)

### Key Configuration Files
- `components.json` — shadcn/ui configuration
- `src/app/globals.css` — Tailwind v4 inline theme + dark mode
- `tsconfig.json` — TypeScript config with `@/*` alias

### Component Selection Process

**IMPORTANT: Always use the shadcn-ui MCP server for component work:**
- `mcp__shadcn-ui__list_components` - Browse all available components
- `mcp__shadcn-ui__get_component_demo` - See usage examples before implementation
- `mcp__shadcn-ui__get_component` - Get source code for installation
- Use these tools for any shadcn/ui planning, selection, or implementation

### Recommended Components for Prototyping
- **Card** - testimonials, service offerings, blog highlights
- **Form** - contact forms, newsletter signups
- **Dialog/Sheet** - modals, mobile navigation drawers
- **Accordion** - FAQ sections, collapsible content
- **Badge** - tags, categories, status indicators
- **Tabs** - content organization, section switching
- **Avatar** - team members, testimonial authors
- **Button** - CTAs (already configured with brand colors)

### Styling System
- Tailwind v4 with inline theme tokens (OKLCH-ready)
- Custom dark variant: `@custom-variant dark (&:is(.dark *))`
- shadcn/ui uses CSS variables
- `cn()` combines `clsx` + `tailwind-merge`

### Fonts
- Headlines: Satoshi Variable
- Body: Karma (woff/woff2 in `public/fonts/Karma-webfonts/`)
- Geist may remain as dev fallback; final site uses Satoshi + Karma

### Design Docs
- Public style guide: `public/STYLE-GUIDE.md`
- Private guides: `/.docs/` (historic) and `/.prd/DESIGN-GUIDE.md` (Webflow + Relume build). Both are git-ignored.

### Development Approach
- **Focus**: Design exploration and visual experimentation
- **Goal**: Create wireframes and prototypes to inform final Webflow build
- **Philosophy**: Prioritize learning what works visually over production constraints
- Use shadcn/ui components liberally to accelerate prototyping

### Conventions
- Prefer `pnpm` over `npm`
- Keep hidden folders ignored: `.docs/`, `.prd/`, `.serena/`, `.old/`
- Follow code style rules: meaningful names, early returns, explicit types on exported APIs

### Final Deployment Context
- **Current Phase:** Prototyping and wireframing
- **Final Deployment:** Live site will be built separately in Webflow using Relume components
- **Purpose:** This repo serves as design exploration workspace - insights feed into Webflow build
- **Documentation:** Private design guides in `/.docs/` and `/.prd/` contain Webflow-specific instructions