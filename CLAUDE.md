# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands

```bash
npm run dev      # Start development server (Vite)
npm run build    # TypeScript check + production build
npm run lint     # Run ESLint
npm run preview  # Preview production build locally
```

## Architecture

This is a React + TypeScript Todo application using Vite as the build tool.

- **Entry point**: `src/main.tsx` renders `App` into `#root`
- **Main component**: `src/App.tsx` contains all Todo logic (state management with `useState`, CRUD operations)
- **Styling**: Component-scoped CSS files (`App.css`, `index.css`)

## Deployment

- Deployed to Vercel (auto-deploys on push to `main`)
- `vite.config.ts` - Do not add `base` path for Vercel deployment
