# Mockup Guide

**Generated:** 2026-04-03
**Design System:** Trust & Authority + Minimal
**Target:** https://hartonodanrekan.com/

---

## Strategic Approach

**Primary Goal:** Generate consultation requests from Indonesian businesses needing legal services.

**Key Insight:** Law firms sell trust and expertise. The website must immediately answer: "Who are these lawyers? Can I trust them with my legal matter?"

**Design Decision:** Lead with the legal team — clients want to know who will be handling their case before reading about services.

---

## Generated Files

| File | Description |
|------|-------------|
| `index.html` | Homepage mockup (self-contained, ~750 lines) |

---

## Design Decisions

### Page Structure (Strategic Order)

1. **Hero** — Firm name, value proposition, immediate CTA
2. **Team Section** — 3 featured lawyers with photos, names, titles, specializations
3. **Practice Areas** — What the firm does
4. **Why Choose Us** — Differentiators and trust signals
5. **Publications** — Demonstrates expertise
6. **CTA** — Final conversion push
7. **Footer** — Contact info and navigation

### Color System

| Token | Hex | Usage |
|-------|-----|-------|
| Primary | `#1E3A5F` | Navy — authority, trust |
| Accent | `#C9A227` | Gold — premium, credibility |
| Background | `#FFFFFF` | Clean, professional |
| Text | `#1A202C` | Strong readability |

### Typography

- **Headings:** Georgia/serif — traditional, authoritative
- **Body:** System sans-serif — clean, fast, accessible

### Layout

- **Container:** 1200px max-width
- **Section spacing:** 80px vertical
- **Grid:** Responsive 1→2→3→4 columns

---

## Components

| Component | Description |
|-----------|-------------|
| Header | Sticky, logo + nav + CTA |
| Hero | Badge, headline, subtitle, dual CTAs, stats |
| Team Card | Photo, name, title, specialization, link |
| Service Card | Icon, title, description |
| Pub Card | Image, date, title, excerpt |
| CTA Section | Headline, text, button, contact info |
| Footer | Brand, links, contact, legal |

---

## Accessibility

- Skip link
- Semantic HTML (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`)
- ARIA labels on interactive elements
- Single H1 per page
- Focus-visible states
- Reduced motion support
- Color contrast 4.5:1+

---

## Responsive Breakpoints

- **Desktop:** 1024px+ (4-col grid)
- **Tablet:** 768-1023px (2-col grid)
- **Mobile:** <768px (1-col, hamburger nav)

---

## Key Improvements from Original Site

| Original Problem | Redesign Solution |
|-----------------|-------------------|
| No people shown | Team section with 3 featured lawyers |
| Generic "Contact Us" | "Schedule Consultation" — specific action |
| No trust signals | Testimonials removed, team/proof emphasized |
| Services buried | Practice areas prominent after hero |
| No About section | "Why Choose Us" with differentiators |

---

## How to View

```bash
open /home/henry/Desktop/projects/website-redesign-workflow/outputs/12-mockup/index.html
```

Or simply open the file in any browser.

---

## How to Deploy

Static HTML — no server required.

- **Direct:** Rename to `index.html` and serve
- **GitHub Pages:** Push to `gh-pages` branch
- **Netlify/Vercel:** Drag and drop folder
- **Local:** Double-click to open

---

## For Developers

1. **No build step** — self-contained HTML
2. **No external deps** — inline SVG icons, system fonts
3. **CSS organized** — reset → variables → base → layout → components → responsive
4. **Images** — Replace gradient placeholders with actual lawyer photos
5. **Forms** — Connect CTA email to Formspree, Netlify Forms, or backend
6. **Additional pages** — Create `/team.html`, `/services.html`, `/contact.html` with consistent styles

---

## Next Steps

1. Replace placeholder avatars with actual lawyer photos
2. Add LinkedIn/social links to team cards
3. Create dedicated Team page with all attorneys
4. Add real testimonials (with client permission)
5. Implement contact form
6. Add cookie consent banner
7. Add favicon and OG meta tags
