## Vegas Improv Power (VIP) — Redesign MVP

This repository contains a Next.js 15 app (TypeScript, App Router, Tailwind CSS v4) with shadcn/ui initialized. We are currently in the planning phase to build a vibrant, professional homepage that embodies VIP’s "Functional Improv®" approach and the tagline "Improv for Being a Human®".

### Status
- Planning/design completed. Webflow + Relume build guide is prepared.
- AI wireframe prototype created and tested successfully.
- Private design docs live in `.docs/` and `/.prd/` (both ignored by git).

### Key Paths
- Public assets: `public/`
  - Logos: `public/logos/2025-web-logo-header-main-transparent.png` (light), `public/logos/2022-web-logo-header-white.png` (dark)
  - Fonts: `public/fonts/` (Satoshi Variable) and `public/fonts/Karma-webfonts/` (woff/woff2)
- Private docs (not committed): `.docs/`, `.prd/`
  - `.docs/` holds historic and extended references
  - `.prd/DESIGN-GUIDE.md` is the Webflow + Relume build guide

### Getting Started
Run the development server:
```bash
pnpm dev
```
Then open http://localhost:3000

### Scripts
- `dev`: Run Next.js dev server
- `build`: Build the app
- `start`: Start the production server
- `lint`: Run ESLint

### Tech
- Next.js 15 (App Router, TypeScript)
- Tailwind CSS v4
- shadcn/ui (latest CLI)

### Docs
- PRD: `PRD.md`
- Tasks: `TASKS.md`
- Public style guide: `public/STYLE-GUIDE.md` (Relume/Webflow oriented)
- Private design references: `/.docs/` and build guide at `/.prd/DESIGN-GUIDE.md` (both ignored)

### Deployment (Preparation)
This repo is configured to be pushed to GitHub. Public assets live under `public/`. Private working docs live under `/.docs/` and `/.prd/` and are listed in `.gitignore`. Live site will be built in Webflow using Relume components with CMS for Blog and optional FAQ.

We will integrate CI and deployment in a later phase.
