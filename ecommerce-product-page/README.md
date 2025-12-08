# 👟 E-commerce Product Page
> Frontend Mentor Challenge - Intermediate Level

<img width="950" height="450" alt="Image" src="https://github.com/user-attachments/assets/d375a56d-2cca-457b-890f-a422e6ae642f" />
<img width="240" height="430" alt="Image" src="https://github.com/user-attachments/assets/8df3aae6-67f7-48a8-bf51-4a5f5799d182" />

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies](#technologies)
- [What I Learned](#what-i-learned)

---

## 🎯 Overview

### The Challenge

Users should be able to:
- ✅ View optimal layout for different device screen sizes
- ✅ See hover and focus states for all interactive elements
- ✅ Navigate the entire interface using keyboard only
- ✅ Switch between product images using thumbnail gallery
- ✅ Add items to cart with quantity selection
- ✅ Experience smooth transitions and animations

---

## ✨ Features

### Accessibility (WCAG AA Compliant)
- ♿ **Skip to content link** - Keyboard users can bypass navigation
- ⌨️ **Full keyboard navigation** - All interactive elements are keyboard accessible
- 🎯 **ARIA labels** - Descriptive labels for screen readers on all controls
- 🔊 **Semantic HTML** - Proper heading hierarchy and landmark regions
- 👁️ **Focus indicators** - Clear visual feedback with custom orange outline
- 🎬 **Reduced motion support** - Respects `prefers-reduced-motion` preference
- 📢 **Live regions** - Quantity changes announced to screen readers with `aria-live`

### Responsive Design
- 📱 **Mobile-first approach** - Optimized for small screens, enhanced for larger
- 💻 **Fluid layouts** - Flexbox and responsive units for smooth scaling
- 🖼️ **Adaptive image gallery** - Carousel on mobile, thumbnails on desktop

### Modern Tailwind CSS
- 🎨 **Custom theme configuration** - Brand colors defined in CSS `@theme` layer
- 🔧 **Component classes** - Reusable `.thumbnail`, `.focus-outline`, `.nav-item-hover`
- ⚡ **Utility-first approach** - Rapid development with Tailwind utilities
- 🎭 **Hover & transition effects** - Smooth scale, color, and shadow transitions
- 🌈 **Color system** - HSL-based palette for consistent theming

---

## 🛠️ Technologies

- **HTML5** - Semantic markup with ARIA enhancements
- **Tailwind CSS v4** - Utility-first CSS framework with custom theme
- **CSS3** - Custom properties, transitions, media queries
- **JavaScript** - (Static version, no interactivity yet)

---

## 🎓 What I Learned

### Tailwind CSS v4 Theme Configuration

```css
@theme {
  /* Custom color palette */
  --color-orange: hsl(26, 100%, 55%);
  --color-blue-dark-grayish: hsl(219, 9%, 45%);
  
  /* Custom font family */
  --font-family-kumbh: "Kumbh Sans", sans-serif;
}
```

**Why this matters:** Tailwind v4's `@theme` directive provides type-safe, autocomplete-friendly custom tokens that integrate seamlessly with utility classes.

### Component Layer for Reusable Patterns

```css
@layer components {
  .thumbnail {
    @apply rounded-xl flex-1 min-w-0 object-cover h-auto 
           shadow hover:scale-105 hover:shadow-lg 
           transition-all duration-200 cursor-pointer;
  }
  
  .focus-outline {
    @apply focus:outline focus:outline-2 
           focus:outline-orange focus:outline-offset-2;
  }
}
```

**Why this matters:** Extracting repeated utility combinations into component classes improves maintainability while preserving Tailwind's utility-first philosophy.

### Accessibility Best Practices

```html
<!-- Skip link for keyboard users -->
<a href="#main-content" 
   class="sr-only focus:not-sr-only focus:absolute focus:top-4 focus:left-4">
  Skip to main content
</a>

<!-- ARIA labels for icon buttons -->
<button aria-label="Decrease quantity" aria-controls="quantity">
  <img src="./images/icon-minus.svg" alt="Minus Icon" />
</button>

<!-- Live region for dynamic content -->
<span id="quantity" aria-live="polite">0</span>
```

**Why this matters:** Screen reader users and keyboard navigators rely on proper semantic HTML and ARIA attributes for equal access to functionality.

### Responsive Layout with Tailwind

```html
<!-- Mobile: stacked layout, Desktop: side-by-side with max-width -->
<main class="lg:flex lg:gap-32 lg:items-center lg:justify-center">
  <figure class="lg:w-1/2 lg:max-w-[500px]">
    <!-- Product images -->
  </figure>
  <section class="lg:w-1/2 lg:max-w-[500px]">
    <!-- Product details -->
  </section>
</main>
```

**Why this matters:** Mobile-first responsive design ensures optimal experience across all device sizes without unnecessary code for smaller screens.

### Reduced Motion Support

```css
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

**Why this matters:** Users with vestibular disorders or motion sensitivity can disable animations system-wide, and our CSS respects that preference.

### Hover State Enhancements

```html
<!-- Scale + shadow on hover for thumbnails -->
<img class="hover:scale-105 hover:shadow-lg transition-all duration-200" />

<!-- Color change on hover for buttons -->
<button class="hover:bg-orange/80 hover:shadow-lg hover:scale-105 
               transition-all duration-200">
  Add to cart
</button>
```

**Why this matters:** Visual feedback on hover improves perceived responsiveness and guides users toward interactive elements.

---

## 🚀 Setup

```bash
# Clone the repository
git clone https://github.com/YasirAkbal/frontend-mentor-challenges.git

# Navigate to project directory
cd frontend-mentor-challenges/ecommerce-product-page

# Open in browser
open index.html
```

No build process required! The HTML file directly references compiled Tailwind CSS.

---

## 📊 Key Metrics

### Accessibility
- ✅ 100% keyboard navigable
- ✅ WCAG AA compliant color contrast
- ✅ Semantic HTML with ARIA enhancements
- ✅ Skip navigation link
- ✅ Focus indicators on all interactive elements
- ✅ Reduced motion support

### Responsive Design
- ✅ Mobile-first approach
- ✅ 2 breakpoints (mobile, desktop lg+)
- ✅ Fluid typography and spacing
- ✅ Touch-friendly tap targets

### Code Quality
- ✅ Clean, semantic HTML5
- ✅ Organized Tailwind utilities
- ✅ Reusable component classes
- ✅ Custom theme configuration
