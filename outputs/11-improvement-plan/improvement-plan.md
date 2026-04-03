# Website Redesign Improvement Plan

**Target:** https://hartonodanrekan.com/
**Date:** 2026-04-03
**Based on:** Steps 01-10 analysis

---

## Executive Summary

Hartono & Rekan is an Indonesian law firm with outdated WordPress/Elementor site (jQuery 1.12.4, WordPress 5.4.6). The site demonstrates legal expertise through articles but fails at basic conversion optimization. The redesign should prioritize: clear contact CTAs, professional design aligned with modern law firm standards, technology modernization, and trust-building through social proof.

---

## Category: Design

### 1. Typography System

**Current Issue:** No consistent typography system, mixed font usage through Elementor

**Recommended Change:**
- Base font: 18px, line-height 1.6
- Headlines: System font stack (SF Pro, Inter, -apple-system)
- H1: 48-56px, weight 700
- H2: 32-36px, weight 600
- H3: 24px, weight 600
- Body: 18px, weight 400
- Letter-spacing: -0.02em on headlines, 0 on body

**Reference Example:** Apple, Ogilvy use system fonts with similar sizing

**Priority:** P1 | **Effort:** Medium | **Impact:** Medium

---

### 2. Color Palette

**Current Issue:** No defined color system, Elementor default blues

**Recommended Change:**
- Primary Background: #ffffff
- Secondary Background: #f8f8f8
- Primary Text: #1a1a1a
- Secondary Text: #666666
- Brand Accent: #0x4A90D9 (professional blue)
- CTA Color: #0x4A90D9 with #0x3A7BC8 hover
- Subtle borders: #e5e5e5

**Reference Example:** Minimal white-based palettes with strategic color accents (Ogilvy, Clio)

**Priority:** P1 | **Effort:** Low | **Impact:** Medium

---

### 3. Layout & Spacing

**Current Issue:** Inconsistent spacing, Elementor defaults

**Recommended Change:**
- Container max-width: 1200px
- Section padding: 80px vertical (desktop), 48px (mobile)
- Component gaps: 24-32px
- Card padding: 24-32px
- Grid: 12-column, 24px gap

**Reference Example:** Ogilvy's generous whitespace, 80-120px section padding

**Priority:** P1 | **Effort:** Medium | **Impact:** High

---

### 4. Homepage Hero

**Current Issue:** No clear hero section, value proposition unclear

**Recommended Change:**
- Full-width hero with gradient/image
- Large headline: "H 法律n & Rekan — Legal Excellence in Indonesia"
- Subheadline with services summary
- Primary CTA: "Schedule Consultation" button
- Secondary CTA: "View Our Services" text link

**Reference Example:** Ogilvy hero pattern, Clio's clear value proposition

**Priority:** P0 | **Effort:** Medium | **Impact:** High

---

### 5. Visual Effects & Motion

**Current Issue:** No animations, static Elementor pages

**Recommended Change:**
- Fade-in on scroll: opacity 0→1, translateY 20px→0, 400ms ease-out
- Hover transitions: 200ms ease
- Button hover: slight scale (1.02) + shadow
- Sticky header: background opacity transition on scroll

**Reference Example:** Subtle Ogilvy animations, Apple scroll effects

**Priority:** P2 | **Effort:** Medium | **Impact:** Low

---

## Category: Content

### 6. Value Proposition

**Current Issue:** No clear value proposition, homepage unclear about services

**Recommended Change:**
- Hero tagline: "Trusted Legal Counsel for Indonesian Businesses"
- Services bullets: Corporate Law, Dispute Resolution, Human Trafficking Law, Property Law
- Differentiator: "Serving clients since [year], combined [X] years experience"

**Reference Example:** Pew Research's clear mission statement, Clio's immediate clarity

**Priority:** P0 | **Effort:** Low | **Impact:** High

---

### 7. Contact CTAs

**Current Issue:** No prominent CTAs, contact info only in footer

**Recommended Change:**
- Header: "Schedule Consultation" button (always visible)
- Hero: Primary CTA
- Mid-page: "Need Legal Advice? Contact Us" section
- Footer: Contact form link
- Phrasing: "Schedule Consultation" not "Contact Us"

**Reference Example:** Clio's multiple CTA strategy, "Schedule a Consultation" phrasing

**Priority:** P0 | **Effort:** Low | **Impact:** High

---

### 8. Social Proof

**Current Issue:** No testimonials, client logos, or case studies

**Recommended Change:**
- Add "What Clients Say" section with 2-3 testimonials
- Include client logos (with permission) or "Trusted by [X] Indonesian businesses"
- Add case study snippets with measurable outcomes
- Credentials/affiliations displayed near CTAs

**Reference Example:** Clio trust signals, testimonial patterns

**Priority:** P1 | **Effort:** Medium | **Impact:** High

---

### 9. Article Structure

**Current Issue:** Articles lack author, date, read time, related content

**Recommended Change:**
- Add author bio box at article end
- Display publication date prominently
- Add estimated read time (e.g., "5 min read")
- Add "Related Articles" section
- Add social sharing buttons

**Reference Example:** Pew Research article structure, clear bylines

**Priority:** P1 | **Effort:** Medium | **Impact:** Medium

---

### 10. About Page Content

**Current Issue:** No About page, firm history/mission unclear

**Recommended Change:**
- Create dedicated About page with:
  - Firm history and founding story
  - Mission and values
  - Areas of practice
  - Office locations and contact info
  - Professional affiliations

**Reference Example:** Professional law firm about pages

**Priority:** P1 | **Effort:** Medium | **Impact:** Medium

---

## Category: UX

### 11. Navigation Structure

**Current Issue:** Navigation unclear, no logical grouping

**Recommended Change:**
- Primary nav: Home, About, Services, Publications, Contact
- Dropdown for Services sub-items
- Mobile: Hamburger menu with full overlay
- Sticky header on scroll
- Current page indicator

**Reference Example:** Clio's mega-menu, Ogilvy sticky nav

**Priority:** P0 | **Effort:** Medium | **Impact:** High

---

### 12. Contact Form

**Current Issue:** No dedicated contact page or inquiry form

**Recommended Change:**
- Create /contact page
- Form fields: Name, Email, Phone (optional), Message, Service Interest (dropdown)
- Inline validation
- Success page with "We'll contact you within 24 hours"
- Contact info: Phone, Email, Office address with map

**Reference Example:** Clio's minimal friction form, clear next steps

**Priority:** P0 | **Effort:** Medium | **Impact:** High

---

### 13. Team/Associates Page

**Current Issue:** Associates slider exists but is inadequate, not linked

**Recommended Change:**
- Create proper /team page
- Photo, name, title, specializations for each associate
- LinkedIn/social links
- Contact option per associate
- Office location information

**Reference Example:** Professional team pages, partner bios

**Priority:** P1 | **Effort:** Medium | **Impact:** Medium

---

## Category: Technical

### 14. Technology Stack Modernization

**Current Issue:** jQuery 1.12.4 (2016), WordPress 5.4.6 (2020), Elementor version issues

**Recommended Change:**
- Upgrade WordPress to latest stable
- Replace jQuery with vanilla JS or modern framework
- Update Elementor to latest version
- Audit and remove unused plugins
- Consider headless WordPress or static site for better performance

**Reference Example:** Apple/Stripe minimal JS approach

**Priority:** P0 | **Effort:** High | **Impact:** High

---

### 15. Performance Optimization

**Current Issue:** Heavy pages (174KB homepage), no lazy loading evident, large images

**Recommended Change:**
- Convert images to WebP format
- Implement lazy loading for below-fold images
- Minify CSS and JavaScript
- Enable browser caching headers
- Target: <500KB total page weight

**Reference Example:** Apple 248KB pages, Stripe performance

**Priority:** P1 | **Effort:** Medium | **Impact:** High

---

### 16. Accessibility Enhancements

**Current Issue:** Multiple H1 on homepage, room for improvement

**Recommended Change:**
- Single H1 per page (firm name on most pages)
- Add skip to main content link
- Ensure all form fields have labels
- Color contrast >4.5:1 ratio
- Add aria-labels to icon-only buttons
- Test with screen reader

**Reference Example:** Apple/Stripe accessibility implementations

**Priority:** P1 | **Effort:** Low | **Impact:** High

---

### 17. SEO Improvements

**Current Issue:** Meta descriptions present but could be optimized, no structured data

**Recommended Change:**
- Add LocalBusiness JSON-LD schema
- Add Organization schema
- Optimize meta descriptions per page
- Ensure single H1 per page
- Create XML sitemap
- Add alt text to all images (already good)

**Reference Example:** Structured data best practices

**Priority:** P1 | **Effort:** Low | **Impact:** Medium

---

### 18. Mobile Responsiveness

**Current Issue:** Viewport meta present but mobile experience unclear

**Recommended Change:**
- Mobile-first CSS approach
- Hamburger menu for mobile nav
- Touch-friendly tap targets (44x44px minimum)
- Responsive images with srcset
- Test on actual mobile devices

**Reference Example:** Apple mobile-first approach

**Priority:** P0 | **Effort:** Medium | **Impact:** High

---

## Implementation Dependencies

Some improvements enable others:

1. **P0 Foundation (Do First)**
   - Hero + Value Proposition (#4, #6)
   - Contact CTA placement (#7)
   - Navigation structure (#11)
   - Contact form page (#12)
   - Technology upgrade (#14)

2. **P1 Enhancement (Do Second)**
   - Typography + Colors (#1, #2)
   - Social proof section (#8)
   - Team page (#13)
   - Accessibility fixes (#16)
   - Performance (#15)
   - Article structure (#9)
   - About page (#10)

3. **P2 Polish (Do Last)**
   - SEO improvements (#17)
   - Motion/animations (#5)
   - Mobile polish (#18)
