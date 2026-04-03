# Reference Analysis: Design Perspective

**References Analyzed:** Ogilvy, JD Supra
**Screenshots:** outputs/06-reference-screenshots/design/

## Key Design Patterns

### 1. Layout & Visual Hierarchy

**Ogilvy (ogilvy.com)**
- Full-viewport hero sections with bold typography
- Clear content sections with generous whitespace
- Card-based layouts for service/offering displays
- Grid-based portfolio/project showcases
- Sticky navigation that transforms on scroll

**JD Supra (jdsupra.com)**
- Clean, content-focused newspaper-style layout
- Strong vertical rhythm with consistent spacing
- Clear typographic hierarchy (large headlines, readable body)
- Minimal decorative elements, content is hero
- Left-aligned text for readability

### 2. Typography Systems

**Best Practices Observed:**
- Sans-serif primary fonts (Inter, SF Pro, etc.)
- Large headline sizes (48-72px on desktop)
- Consistent line-height (1.4-1.6 for body)
- Clear weight differentiation (300, 400, 600, 700)
- Ample letter-spacing on headlines

**CSS Patterns:**
```css
/* Ogilvy-style */
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
font-size: clamp(2rem, 5vw, 4rem);
font-weight: 600;
letter-spacing: -0.02em;
line-height: 1.1;

/* Body text */
font-size: 1.125rem;
line-height: 1.6;
```

### 3. Color Usage

**Common Patterns:**
- White/light gray backgrounds (#ffffff, #f5f5f5)
- Primary brand colors used sparingly (buttons, links)
- Dark text on light backgrounds for readability
- Accent colors for CTAs only
- Neutral grays for secondary text

**Recommended Palette Approach:**
- Background: #ffffff (primary), #f8f8f8 (sections)
- Text: #1a1a1a (primary), #666666 (secondary)
- Brand accent: #0056b3 or similar professional blue
- CTA: #0066cc with #004499 hover

### 4. Spacing & Rhythm

- Section padding: 80-120px vertical
- Container max-width: 1200-1400px
- Content gaps: 24-48px
- Component internal padding: 16-32px
- Grid gap: 24-32px

### 5. Imagery & Icons

- High-quality, contextual photography
- Minimal iconography (line icons preferred)
- Strategic use of whitespace around images
- Lazy loading for off-screen images

### 6. Motion & Effects

- Subtle fade-in on scroll (opacity + translateY)
- Smooth hover transitions (200-300ms)
- Transform scale on interactive elements (1.02-1.05)
- No jarring or distracting animations

## Recommendations for Redesign

1. **Hero Section** - Adopt Ogilvy-style full-viewport hero with bold headline
2. **Typography** - Use system font stack with large, bold headlines
3. **Color** - Keep minimal, white-dominant with strategic blue accents
4. **Spacing** - Generous whitespace between sections
5. **Motion** - Subtle scroll animations, quick hover transitions
