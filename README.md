# TwoSixMitch - Personal Website

My personal website built with Astro, showcasing my app development work and blog.

## Quick Start

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run preview  # Preview production build
```

## Structure

```
src/
├── assets/              # Images and static assets
├── components/          # Header, Footer, SEO
├── layouts/             # Base layout
├── pages/               # Main pages and blog
└── config.js           # Site configuration
```

## Adding New Blog Posts

1. Create new `.astro` file in `src/pages/blog/`
2. Use existing posts as templates
3. Add to `blogPosts` arrays in:
   - `src/pages/blog/index.astro`
   - `src/pages/index.astro`

## Deployment

Push to `main` branch → automatically deploys to GitHub Pages at `https://twosixmitch.github.io`

---

*Personal website - built with Astro + Tailwind CSS*
