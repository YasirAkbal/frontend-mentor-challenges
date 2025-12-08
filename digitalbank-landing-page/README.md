# 🏦 Digitalbank Landing Page

> Frontend Mentor Challenge - Intermediate Level

<img width="900" height="450" alt="Image" src="https://github.com/user-attachments/assets/94ceb9b8-af3f-4ef6-86eb-17b6dd4ec3a8" />

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies](#technologies)
- [What I Learned](#what-i-learned)

---

## 🎯 Overview

### The Challenge

Users should be able to:
- ✅ View optimal layout depending on device screen size
- ✅ See hover states for interactive elements
- ✅ Navigate using keyboard only
- ✅ Experience dark mode support

### Screenshot

<img width="450" height="225" alt="Image" src="https://github.com/user-attachments/assets/94ceb9b8-af3f-4ef6-86eb-17b6dd4ec3a8" />
<img width="450" height="225" alt="Image" src="https://github.com/user-attachments/assets/5508a295-4d51-4cd8-9977-3a0704d44062" />
<img width="240" height="400" alt="Image" src="https://github.com/user-attachments/assets/29ecb954-e7e7-4c7f-b3a3-a6f9e30e2a96" />

---

## ✨ Features

### Accessibility (WCAG AA Compliant)
- ♿ Skip navigation link
- ⌨️ Full keyboard navigation
- 🎯 44px minimum touch targets
- 🔊 Screen reader friendly
- 👁️ Focus indicators on all interactive elements
- 🎬 Reduced motion support

### Responsive Design
- 📱 Mobile-first approach
- 💻 4 responsive breakpoints
- 🔄 Fluid typography and spacing

### Modern CSS
- 🎨 CSS Custom Properties
- 📐 CSS Grid & Flexbox
- 🌓 Dark mode with `prefers-color-scheme`

---

## 🛠️ Technologies

- HTML5 (Semantic markup)
- CSS3 (Grid, Flexbox, Custom Properties)
- Vanilla JavaScript
- No frameworks or build tools

---

## 🎓 What I Learned

### CSS Techniques
```css
/* CSS Custom Properties for theming */
:root {
    --clr-primary: hsl(233, 26%, 24%);
    --clr-green-500: hsl(136, 64%, 51%);
}

/* AAA Touch Target compliance */
a, button {
    min-height: 44px;
}

/* Reduced motion support */
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.01ms !important;
    }
}
```

### Accessibility Patterns
```html
<!-- Skip link for keyboard users -->
<a href="#main-content" class="skip-link">Skip to main content</a>

<!-- ARIA landmarks -->
<section aria-labelledby="intro-heading">
    <h1 id="intro-heading">Next generation digital banking</h1>
</section>
```

### Smart Solutions
```css
/* Clickable card without wrapping everything in <a> */
.card a::after {
    content: '';
    position: absolute;
    inset: 0;
}
```

---

## 🚀 Setup
```bash
# Clone the repo
git clone https://github.com/YasirAkbal/frontend-mentor-challenges.git

# Navigate to project
cd frontend-mentor-challenges/digitalbank-landing-page

# Open in browser
open index.html
```

No build process needed! Just open `index.html` in your browser.

---
