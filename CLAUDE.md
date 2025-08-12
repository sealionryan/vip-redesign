# CLAUDE.md

Guidance for Claude Code when working with this repository.

## Development Commands

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

### Key Configuration Files
- `components.json` — shadcn/ui configuration
- `src/app/globals.css` — Tailwind v4 inline theme + dark mode
- `tsconfig.json` — TypeScript config with `@/*` alias

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

### Conventions
- Prefer `pnpm` over `npm`.
- Keep hidden folders ignored: `.docs/`, `.prd/`, `.serena/`, `.old/`.
- Follow code style rules: meaningful names, early returns, explicit types on exported APIs.

### Notes
- Webflow + Relume will implement the live site. This repo houses the Next.js MVP and design references. Keep docs synchronized when substantive changes are made.