## Vegas Improv Power (VIP) — Redesign MVP

This repository contains a Next.js 15 app (TypeScript, App Router, Tailwind CSS v4) with shadcn/ui initialized. We are currently in the planning phase to build a vibrant, professional homepage that embodies VIP’s "Functional Improv®" approach and the tagline "Improv for Being a Human®".

### Status
- Planning only. No implementation has begun yet.
- Private design docs placed in `.docs/` (ignored by git) for local reference.

### Key Paths
- Public assets: `public/`
  - Logos: `public/logos/2025-web-logo-header-main-transparent.png` (for light bgs), `public/logos/2022-web-logo-header-white.png` (for dark bgs)
- Private docs (not committed): `.docs/`
  - `/.docs/DESIGN-GUIDE.md`
  - `/.docs/HOMEPAGE-OUTLINE.md`

### Getting Started
Run the development server:
```bash
npm run dev
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
- Private design references live in `/.docs/` and are intentionally ignored by git.

### Deployment (Preparation)
This repo is configured to be pushed to GitHub. Public assets live under `public/`. Private working docs live under `/.docs/` and are already listed in `.gitignore`.

We will integrate CI and deployment in a later phase.
