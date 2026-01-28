# Kazend Website

Landing page for Kazend, a CRM platform for real estate agents.

## Tech Stack

- **Astro 5.x** - Static site generator
- **Tailwind CSS v4** - Using `@tailwindcss/vite` plugin
- **TypeScript** - Type-safe development

## Design System

### Colors (defined in `src/styles/global.css`)

| Name | Value | Usage |
|------|-------|-------|
| `charcoal` | `#0a0a0a` | Primary background |
| `warm-black` | `#121210` | Secondary background |
| `cream` | `#f5f0e8` | Primary text |
| `gold` | `#c9a66b` | Accent color |
| `gold-light` | `#e8d4b0` | Light accent |
| `gold-dark` | `#a68544` | Dark accent |
| `stone` | `#2a2825` | Borders, cards |
| `muted` | `#8a8680` | Secondary text |

### Typography

- **Display font**: Syne (headings, `.font-display`)
- **Body font**: Outfit (body text, default)

### Animation Classes

- `.animate-fade-up` - Fade in with upward movement
- `.animate-fade-in` - Simple fade in
- `.animate-slide-in` - Slide in from left
- `.animate-line-grow` - Line expansion effect
- `.animate-float` - Floating animation
- `.animate-pulse-glow` - Pulsing glow effect
- `.delay-100` through `.delay-800` - Animation delays

### Utility Classes

- `.noise-bg` - Adds noise texture overlay
- `.geo-lines` - Geometric grid pattern
- `.text-gradient-gold` - Gold gradient text effect
- `.glow-border` - Subtle glowing border
- `.corner-accent` - Decorative corner borders
- `.feature-card` - Card with hover effects
- `.social-link` - Social link hover style

## Project Structure

```
src/
├── components/
│   ├── Header.astro      # Site header with logo
│   ├── Footer.astro      # Site footer
│   └── FeatureCard.astro # Feature card component
├── layouts/
│   └── Layout.astro      # Base layout (meta, fonts, global styles)
├── pages/
│   └── index.astro       # Landing page
└── styles/
    └── global.css        # Theme, animations, utility classes
```

## Commands

```bash
pnpm install    # Install dependencies
pnpm run dev    # Start dev server
pnpm run build  # Production build
pnpm run preview # Preview production build
```

## Coding Conventions

- Use Astro components (`.astro`) for all UI
- Apply Tailwind utility classes directly in templates
- Use theme colors via Tailwind: `bg-charcoal`, `text-gold`, etc.
- Keep components small and focused
- Use the `Layout.astro` wrapper for all pages
