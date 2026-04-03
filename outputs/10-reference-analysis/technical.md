# Reference Analysis: Technical Perspective

**References Analyzed:** Apple, Stripe
**Screenshots:** outputs/06-reference-screenshots/technical/

## Key Technical Patterns

### 1. Page Performance

**Apple (apple.com):**
- Total page weight: 248 KB (HTML only, images separate)
- Minimal external scripts: 12
- CSS likely inline or minimal external files
- Image lazy loading
- Optimized image formats (WebP with fallbacks)

**Stripe (stripe.com):**
- Total page weight: 563 KB (heavy but acceptable for features)
- Minimal blocking resources
- Code splitting for JavaScript
- Preconnect and prefetch headers
- Critical CSS inlined

**Performance Best Practices:**
- Target: <200 KB initial HTML + CSS
- Images: WebP format, lazy loading, srcset for responsive
- Scripts: Defer non-critical JS, minimal dependencies
- Fonts: System fonts or self-hosted, preload critical
- Time to Interactive: <3 seconds on 3G

### 2. Accessibility Implementations

**Both Apple and Stripe excel at:**

**Semantic HTML:**
```html
<header role="banner">
  <nav role="navigation" aria-label="Main">
  <main role="main">
  <footer role="contentinfo">
  <article>
  <section>
```

**ARIA Attributes:**
- aria-label for icon-only buttons
- aria-expanded for menus
- aria-current for active nav
- aria-hidden for decorative elements
- role attributes where semantic HTML insufficient

**Keyboard Navigation:**
- Visible focus indicators (outline on focus)
- Skip to main content link
- Logical tab order
- Escape key closes modals

**Additional A11y:**
- Color contrast ratios >4.5:1
- Form labels explicitly associated
- Error messages linked to fields via aria-describedby
- Alt text on all images

### 3. Mobile Responsiveness

**Effective Patterns:**
- Mobile-first CSS approach
- Breakpoints: 768px (tablet), 1024px (desktop)
- Flexible images: max-width: 100%
- Hamburger menus on mobile
- Touch-friendly tap targets (min 44x44px)
- Viewport meta tag set correctly

### 4. SEO Structure

**Critical Elements:**
- Single <h1> per page
- Logical heading hierarchy (h1 → h2 → h3)
- Meta title and description
- Canonical URLs
- Structured data (JSON-LD) for Organization, LocalBusiness
- XML sitemap
- robots.txt allowing crawlers
- Mobile-friendly (Google requirement)

### 5. Code Organization

**Apple Patterns:**
- Custom CSS properties for theming
- BEM-like class naming
- Minimal specificity conflicts
- CSS Grid and Flexbox for layout
- No inline styles (except dynamic)

**Stripe Patterns:**
- Component-based architecture
- Utility classes for spacing
- Consistent naming conventions
- Separated concerns (HTML/CSS/JS)

## Recommendations for Redesign

1. **Performance**
   - Target <500 KB total page weight
   - Use WebP images with lazy loading
   - Minimize JavaScript (avoid jQuery if possible)
   - System font stack to avoid font loading

2. **Accessibility**
   - Single H1 per page
   - Add skip to content link
   - All images require alt text
   - Form labels explicitly associated
   - Color contrast >4.5:1
   - Focus indicators visible

3. **SEO**
   - Add LocalBusiness structured data
   - Ensure single H1 on all pages
   - Add meta descriptions if missing
   - Create XML sitemap

4. **Code Quality**
   - CSS custom properties for colors/spacing
   - Semantic HTML5 elements
   - No inline styles
   - Mobile-first responsive approach
