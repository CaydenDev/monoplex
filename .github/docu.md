# Monoplex CSS Framework Documentation
Version 1.1.3

## Overview

Monoplex is a sophisticated dark-themed CSS framework that provides a comprehensive set of tools for building modern web interfaces. This documentation provides detailed information about all features, components, and utilities available in the framework.

## Design System

### Color System

Monoplex uses a carefully crafted color system with semantic variables:

```css
:root {
  /* Base Colors */
  --monoplex-bg: #0a0a0a;
  --monoplex-surface: #121212;
  --monoplex-surface-2: #181818;
  --monoplex-text: #a0a0a0;
  --monoplex-text-muted: #707070;

  /* Theme Colors */
  --monoplex-primary: #445566;
  --monoplex-secondary: #554466;
  --monoplex-accent: #446655;
  --monoplex-muted: #333333;

  /* Color Variations */
  --monoplex-primary-light: #556677;
  --monoplex-primary-dark: #334455;
  --monoplex-secondary-light: #665577;
  --monoplex-secondary-dark: #443355;
  --monoplex-accent-light: #557766;
  --monoplex-accent-dark: #335544;
}
```

### Typography

#### Font Families
```css
--monoplex-font-sans: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
--monoplex-font-mono: 'Fira Code', Consolas, Monaco, 'Andale Mono', 'Ubuntu Mono', monospace;
```

#### Size Scale
```css
--monoplex-size-1: 0.25rem;  /* 4px */
--monoplex-size-2: 0.5rem;   /* 8px */
--monoplex-size-3: 0.75rem;  /* 12px */
--monoplex-size-4: 1rem;     /* 16px */
--monoplex-size-5: 1.5rem;   /* 24px */
--monoplex-size-6: 2rem;     /* 32px */
--monoplex-size-8: 3rem;     /* 48px */
--monoplex-size-10: 4rem;    /* 64px */
--monoplex-size-12: 6rem;    /* 96px */
```

## Components

### Buttons

#### Basic Button
```html
<button class="btn">Click me</button>
```

#### Button Variants
```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-secondary">Secondary</button>
<button class="btn btn-accent">Accent</button>
<button class="btn btn-outline">Outline</button>
```

#### Special Effect Buttons
```html
<!-- Magnetic Button -->
<button class="btn-magnetic">
  Magnetic Button
</button>

<!-- Liquid Button -->
<button class="btn-liquid">
  <span>Liquid Effect</span>
</button>

<!-- Cyber Button -->
<button class="plex-hover-button">
  Cyber Effect
</button>
```

### Cards

#### Basic Card
```html
<div class="card">
  <h3 class="card-title">Card Title</h3>
  <div class="card-body">
    Card content goes here
  </div>
</div>
```

#### Special Effect Cards
```html
<!-- Glass Card -->
<div class="glass-card">
  Glass effect card content
</div>

<!-- Cyber Card -->
<div class="cyber-card">
  Cyberpunk style card
</div>

<!-- Holographic Card -->
<div class="card-holographic">
  Holographic effect card
</div>
```

### Forms

#### Basic Input
```html
<div class="form-group">
  <label class="form-label">Input Label</label>
  <input type="text" class="form-control">
</div>
```

#### Animated Input
```html
<div class="form-group">
  <input type="text" class="input-animated" placeholder=" ">
  <label>Floating Label</label>
</div>
```

#### Switch
```html
<label class="switch">
  <input type="checkbox">
  <span class="slider"></span>
</label>
```

## Layout Utilities

### Flexbox
```html
<!-- Basic Flex Container -->
<div class="flex">
  <div>Item 1</div>
  <div>Item 2</div>
</div>

<!-- Common Flex Patterns -->
<div class="flex items-center justify-between">
  <div>Aligned Center</div>
  <div>Space Between</div>
</div>

<div class="flex-col items-center">
  <div>Column Layout</div>
  <div>Centered Items</div>
</div>
```

### Grid
```html
<!-- Basic Grid -->
<div class="grid grid-cols-3 gap-4">
  <div>Grid Item 1</div>
  <div>Grid Item 2</div>
  <div>Grid Item 3</div>
</div>

<!-- Responsive Grid -->
<div class="grid sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
  <!-- Grid items -->
</div>
```

## Special Effects

### Text Effects
```html
<!-- Gradient Text -->
<span class="text-gradient">Gradient Text</span>

<!-- Neon Text -->
<span class="text-neon">Neon Glow</span>

<!-- Glitch Text -->
<span class="text-glitch">Glitch Effect</span>
```

### Background Effects
```html
<!-- Glass Effect -->
<div class="glass">
  Glassmorphism background
</div>

<!-- Matrix Effect -->
<div class="matrix-bg">
  Matrix rain effect
</div>

<!-- Quantum Dots -->
<div class="quantum-dots">
  Quantum dot pattern
</div>
```

## Animations

### Built-in Animations
```html
<div class="animate-fade-in">Fade In</div>
<div class="animate-slide-in">Slide In</div>
<div class="animate-pulse">Pulse Effect</div>
<div class="animate-shimmer">Shimmer Effect</div>
```

### Custom Animation Variables
```css
--monoplex-ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
--monoplex-ease-smooth: cubic-bezier(0.4, 0, 0.2, 1);
--monoplex-ease-spring: cubic-bezier(0.175, 0.885, 0.32, 1.275);
```

## Responsive Design

### Breakpoints
```css
/* Small (sm) */
@media (min-width: 640px) {
  .sm\:class-name { /* styles */ }
}

/* Medium (md) */
@media (min-width: 768px) {
  .md\:class-name { /* styles */ }
}

/* Large (lg) */
@media (min-width: 1024px) {
  .lg\:class-name { /* styles */ }
}
```

### Responsive Utilities
```html
<div class="hidden sm:block">
  <!-- Visible only on small screens and up -->
</div>

<div class="sm:flex md:grid lg:block">
  <!-- Different layouts at different breakpoints -->
</div>
```

## Best Practices

### Performance Tips
1. Use the built-in utility classes instead of writing custom CSS
2. Leverage the CSS custom properties for theming
3. Use the responsive utilities for adaptive layouts
4. Minimize the use of heavy effects on mobile devices

### Accessibility
1. Maintain proper color contrast using the provided color system
2. Use semantic HTML elements with framework classes
3. Ensure interactive elements are keyboard accessible
4. Test with screen readers

## Browser Support

Monoplex is tested and supported in:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

Note: Some advanced effects may have limited support in older browsers.

