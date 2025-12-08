# 🎨 Frontend Mentor Challenges

A focused collection of Frontend Mentor challenges to master modern HTML, CSS, and Tailwind fundamentals - the foundation layer of full-stack development.

<div align="center">

![Status](https://img.shields.io/badge/Status-In_Progress-yellow?style=for-the-badge)
![Projects](https://img.shields.io/badge/Projects-2%2F3-blue?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

</div>

---

## 🎯 Project Scope & Intent

As a **full-stack developer**, this repository represents a **deliberate focus** on frontend fundamentals - specifically HTML, CSS, and Tailwind CSS. While my broader tech stack includes React (frontend) and Java (backend), this collection intentionally isolates foundational styling and markup skills.

### Why This Matters

In production environments, clean HTML/CSS is crucial:
- **Component Libraries** (React, Vue) still require deep CSS knowledge
- **Design Systems** demand strong fundamentals
- **Performance** starts with efficient markup and styling
- **Accessibility** is foundational, not framework-dependent
- **Maintainability** requires understanding the core web platform

This is **not** a full portfolio - it's a targeted skill development project for the presentation layer.

---

## 🌐 Live Demos
[Digitalbank-Landing-Page](https://digitalbank-landing-page-yasir-akbal.netlify.app/)  
[E-Commerce Product Page](https://e-commerce-product-page-yasir-akbal.netlify.app)

---

## 🎓 Learning Objectives

### Core Focus Areas
- ✅ **Semantic HTML5** - Proper markup structure and document flow
- ✅ **Modern CSS3** - Grid, Flexbox, Custom Properties, advanced selectors
- 🎨 **Tailwind CSS** - Utility-first methodology and production optimization
- 📱 **Responsive Architecture** - Mobile-first, fluid design systems
- ♿ **Accessibility Engineering** - WCAG AA compliance, ARIA patterns
- 🎨 **UI/UX Principles** - Visual hierarchy, interaction patterns, usability

### Intentional Constraints
- **No JavaScript frameworks** - Pure HTML/CSS to master fundamentals
- **No backend integration** - Focus on presentation layer only
- **Static implementations** - Foundation for future dynamic applications

---

## 📂 Projects

### ✅ 1. [Digitalbank Landing Page](./digitalbank-landing-page)
**Status:** Complete | **Complexity:** Intermediate | **Stack:** HTML5, CSS3, Vanilla JS (minimal)

Enterprise-grade landing page demonstrating modern CSS architecture and accessibility patterns.

**Technical Highlights:**
- ♿ **WCAG AA Compliant** - Full keyboard navigation, ARIA landmarks, screen reader optimization
- 🎨 **CSS Architecture** - Custom properties for theming, BEM-inspired naming, modular structure
- 🌓 **Theme System** - Dark mode using `prefers-color-scheme` media query
- 📱 **Responsive Design** - 4 breakpoint system, fluid typography, container queries
- ⚡ **Performance** - 95+ Lighthouse score
- 🎯 **Touch Targets** - AAA compliance (44px minimum)

**Engineering Decisions:**
- Mobile-first cascade for optimal delivery
- CSS custom properties for maintainable theming
- Pseudo-elements for interactive card overlays (avoiding unnecessary DOM nodes)
- Reduced motion support for accessibility

**Metrics:**
- Lighthouse: Accessibility 20/21
- Lines of CSS: ~900 (well-organized, commented)
- Accessibility: 100% keyboard navigable, full ARIA support

---

### ✅ 2. [E-commerce Product Page](./ecommerce-product-page)
**Status:** Complete | **Complexity:** Intermediate | **Stack:** HTML5, Tailwind CSS

Modern e-commerce product page showcasing Tailwind CSS utility-first architecture and component patterns.

**Technical Highlights:**

- 🎨 Tailwind v4 Migration - Latest CSS-first configuration with @import, @theme, @source
- ♿ Accessibility First - Skip links, ARIA labels, keyboard navigation, live regions
- 📱 Mobile-First Responsive - Breakpoint-driven layout with lg: utilities for desktop
- 🎯 Custom Design System - Theme variables for colors and typography via @theme directive
- ⚡ Component Layer - Reusable .thumbnail, .focus-outline, .nav-item-hover classes

**Engineering Decisions:**

- Tailwind v4 CSS-native configuration for better DX and performance
- Custom component layer for repeated patterns (thumbnails, focus states)
- Semantic HTML with proper landmarks (<header>, <main>, <nav>, <figure>)
- Quantity selector with aria-live="polite" for screen reader feedback

**Design Patterns:**

- Mobile: Stacked layout with image carousel controls
- Desktop: Two-column grid (image gallery + product details)
- Interactive thumbnail gallery for desktop (hidden on mobile)
- Flexible quantity controls with accessible button labels

**Tailwind Techniques:**

- @layer components for extracting repeated utility patterns
- CSS custom properties via @theme for design tokens
- Responsive utilities (lg:flex, lg:w-1/2) for layout shifts
- Utility composition (e.g., flex items-center justify-between)
- focus: variants for keyboard accessibility
- hover: and transition-* for smooth interactions

---

### 📋 3. [Project TBD]
**Status:** Planned | **Complexity:** Advanced | **Stack:** HTML5, Tailwind CSS

Advanced layout challenge to be determined.

---
