# Project Overview

This is an Astro Nano portfolio and blog site built with Astro, Tailwind CSS, and TypeScript.

## Tech Stack
- **Framework**: Astro 5.0.5
- **Styling**: Tailwind CSS 3.4.1 with Typography plugin
- **Language**: TypeScript 5.4.2
- **Content**: MDX support for enhanced markdown
- **Linting**: ESLint with TypeScript and Astro plugins

## Project Structure
```
src/
├── components/     # Reusable UI components
├── content/        # Content collections
│   ├── blog/       # Blog posts
│   ├── projects/   # Project entries
│   └── work/       # Work experience
├── layouts/        # Page layouts
├── lib/            # Utility functions
├── pages/          # Route pages
├── styles/         # Global styles
├── consts.ts       # Global constants
└── types.ts        # TypeScript type definitions
```

## Key Commands
```bash
npm run dev          # Start dev server at localhost:4321
npm run build        # Build for production (runs astro check first)
npm run preview      # Preview production build
npm run lint         # Run ESLint
npm run lint:fix     # Auto-fix ESLint issues
```

## Important Notes
- The project uses Astro's content collections for blog, projects, and work sections
- All builds run `astro check` first to ensure type safety
- ESLint is configured for TypeScript and Astro files
- The site is optimized for performance (100/100 Lighthouse score)

## Development Workflow
1. Always run `npm run lint` before finalizing changes
2. Use `astro check` (via `npm run build`) to verify TypeScript types
3. Content is managed through markdown/MDX files in `src/content/`
4. Components follow a minimalist design pattern with Tailwind CSS

## Configuration Files
- `astro.config.mjs` - Astro configuration
- `tsconfig.json` - TypeScript configuration
- `package.json` - Dependencies and scripts
- `tailwind.config.js` - Tailwind CSS configuration (if present)