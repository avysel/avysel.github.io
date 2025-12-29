# Nexus Prism Design System

## Overview

Nexus Prism is a modern, tech-focused design system created for professional GitHub Pages sites. It combines sleek aesthetics with cutting-edge visual effects, featuring glassmorphism, subtle gradients, and smooth animations. The system uses Bootstrap 5.3.3 only for structure and responsive layout, with all visual styles completely customized.

## Design Principles

1. **Modern Tech Aesthetic** : Glassmorphism, subtle gradients, smooth shadows
2. **Professional Palette** : Tech-inspired colors (blues, purples, cyans)
3. **Clean Typography** : Modern, readable fonts with optimal spacing
4. **Smooth Interactions** : Fluid animations and transitions
5. **Unique Identity** : No visual resemblance to default Bootstrap
6. **Accessibility** : WCAG 2.1 AA compliance

## Color Palette

### Primary Colors - Tech Inspired

```css
--color-primary: #6366F1;        /* Indigo - primary tech color */
--color-primary-dark: #4F46E5;  /* Dark indigo - hover states */
--color-primary-light: #818CF8;  /* Light indigo - variants */

--color-secondary: #8B5CF6;     /* Purple - secondary tech color */
--color-accent: #06B6D4;         /* Cyan - accents, highlights */
--color-success: #10B981;        /* Emerald - success states */
--color-warning: #F59E0B;        /* Amber - warnings */
--color-error: #EF4444;          /* Red - errors */
--color-info: #3B82F6;           /* Blue - information */
```

### Neutral Colors - Professional Grays

```css
--color-bg-primary: #0F172A;     /* Slate 900 - dark background */
--color-bg-secondary: #1E293B;   /* Slate 800 - secondary background */
--color-bg-tertiary: #334155;    /* Slate 700 - tertiary background */
--color-bg-light: #F8FAFC;       /* Slate 50 - light background */
--color-bg-glass: rgba(15, 23, 42, 0.7); /* Glass effect background */

--color-text-primary: #F1F5F9;   /* Slate 100 - primary text */
--color-text-secondary: #CBD5E1; /* Slate 300 - secondary text */
--color-text-muted: #94A3B8;     /* Slate 400 - muted text */
--color-text-inverse: #0F172A;   /* Dark text on light background */

--color-border: #334155;         /* Slate 700 - borders */
--color-border-light: #475569;   /* Slate 600 - light borders */
--color-border-glow: rgba(99, 102, 241, 0.5); /* Glowing border effect */
```

## Typography

### Font Families

```css
--font-primary: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
--font-mono: 'JetBrains Mono', 'Fira Code', 'SF Mono', Monaco, monospace;
```

### Typographic Hierarchy

```css
/* Headings */
--font-size-h1: 3rem;            /* 48px */
--font-size-h2: 2.25rem;        /* 36px */
--font-size-h3: 1.875rem;       /* 30px */
--font-size-h4: 1.5rem;         /* 24px */
--font-size-h5: 1.25rem;        /* 20px */
--font-size-h6: 1.125rem;       /* 18px */

/* Body text */
--font-size-base: 1rem;         /* 16px */
--font-size-sm: 0.875rem;       /* 14px */
--font-size-xs: 0.75rem;        /* 12px */
--font-size-lg: 1.125rem;       /* 18px */
--font-size-xl: 1.25rem;        /* 20px */

/* Weights */
--font-weight-light: 300;
--font-weight-normal: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;

/* Line heights */
--line-height-tight: 1.25;
--line-height-normal: 1.5;
--line-height-relaxed: 1.75;
```

### Usage Examples

- **H1** : Main page title (3rem, semibold)
- **H2** : Main sections (2.25rem, semibold)
- **H3** : Subsections (1.875rem, medium)
- **H4-H6** : Card titles, lists (1.5rem - 1.125rem, medium)
- **Body** : Regular text (1rem, normal, line-height: 1.75)
- **Small** : Metadata, dates (0.875rem, normal)

## Spacing

### Spacing System

```css
--spacing-xs: 0.25rem;      /* 4px */
--spacing-sm: 0.5rem;       /* 8px */
--spacing-md: 1rem;         /* 16px */
--spacing-lg: 1.5rem;       /* 24px */
--spacing-xl: 2rem;         /* 32px */
--spacing-2xl: 3rem;        /* 48px */
--spacing-3xl: 4rem;        /* 64px */
--spacing-4xl: 6rem;        /* 96px */
```

### Usage

- **xs** : Minimal internal spacing (icons, badges)
- **sm** : Spacing between close elements
- **md** : Standard spacing (card padding)
- **lg** : Spacing between sections
- **xl** : Spacing between major sections
- **2xl-4xl** : Spacing between major blocks

## Borders and Radius

### Border Radius - Modern Rounded

```css
--border-radius-sm: 0.375rem;   /* 6px */
--border-radius-md: 0.5rem;     /* 8px */
--border-radius-lg: 0.75rem;    /* 12px */
--border-radius-xl: 1rem;       /* 16px */
--border-radius-2xl: 1.5rem;    /* 24px */
--border-radius-full: 9999px;    /* Full circle */
```

### Border Widths

```css
--border-width: 1px;
--border-width-thick: 2px;
```

## Shadows

### Modern Soft Shadows

```css
--shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
--shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
--shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
--shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
--shadow-2xl: 0 25px 50px -12px rgba(0, 0, 0, 0.25);

/* Glow effects */
--shadow-glow-primary: 0 0 20px rgba(99, 102, 241, 0.4);
--shadow-glow-accent: 0 0 20px rgba(6, 182, 212, 0.4);
```

## Components

All components use custom visual styles with a unique tech-modern identity.

### Buttons

**Custom Styles** :
- Gradient backgrounds with subtle transitions
- Soft shadows with glow effects on hover
- Smooth animations: `translateY(-2px)` on hover
- Modern border-radius
- Glassmorphism effects for outline variants

**Available Variants** :
- `btn-primary` : Indigo gradient with glow
- `btn-secondary` : Purple gradient
- `btn-outline-primary` : Glassmorphism outline style
- `btn-success` : Emerald gradient
- `btn-danger` : Red gradient

### Cards

**Custom Styles** :
- Glassmorphism background with backdrop blur
- Subtle borders with glow effects
- Modern border-radius (12px)
- Hover effect: `translateY(-4px)` with enhanced shadow
- Gradient overlays for headers

### Badges

**Custom Styles** :
- Rounded pill shape
- Gradient backgrounds
- Soft shadows
- Glow effects for primary badges
- Modern typography

### Alerts

**Custom Styles** :
- Glassmorphism backgrounds
- Left border accent (4px)
- Soft shadows
- Smooth fade-in animations
- Modern border-radius

### Navigation

**Custom Styles** :
- Glassmorphism navbar
- Smooth hover transitions
- Active state with gradient background
- Subtle glow effects
- Modern spacing

### Links

**Custom Styles** :
- Gradient text on hover
- Smooth underline animation
- Medium font weight
- Tech color scheme

## Layout

### Container

```css
--container-max-width: 1280px;
--container-padding: var(--spacing-xl);
```

### Grid System

Uses Bootstrap 5.3 grid system (12 columns) for structure:
- Classes: `row`, `col`, `col-{breakpoint}-{size}`
- Breakpoints: xs, sm, md, lg, xl, xxl
- Gaps: `g-*`, `gx-*`, `gy-*` for spacing

### Sections

- Vertical spacing: `--spacing-2xl` between sections
- Horizontal padding: `--spacing-xl` on mobile, `--spacing-2xl` on desktop
- Glassmorphism backgrounds with backdrop blur

## Animations and Transitions

```css
--transition-fast: 150ms cubic-bezier(0.4, 0, 0.2, 1);
--transition-base: 200ms cubic-bezier(0.4, 0, 0.2, 1);
--transition-slow: 300ms cubic-bezier(0.4, 0, 0.2, 1);
```

**Common Uses** :
- Hover states: `--transition-base`
- Interactive elements: `--transition-fast`
- Complex animations: `--transition-slow`

## Glassmorphism Effects

```css
/* Glass background */
background: rgba(15, 23, 42, 0.7);
backdrop-filter: blur(10px);
-webkit-backdrop-filter: blur(10px);
border: 1px solid rgba(255, 255, 255, 0.1);
```

## Interactive States

### Focus

- Outline: 2px solid `--color-primary`
- Glow effect: `--shadow-glow-primary`
- Smooth transition

### Disabled

- Opacity: 0.5
- Cursor: not-allowed
- Pointer-events: none

### Loading

- Animated spinner with gradient
- Reduced opacity on content
- Cursor: wait

## Accessibility

### Contrast

- All texts respect a minimum contrast ratio of 4.5:1
- Text on dark backgrounds: minimum ratio of 7:1

### Keyboard Navigation

- All interactive elements are keyboard accessible
- Visible and clear focus with glow effects
- Logical tab order

### ARIA

- Appropriate use of ARIA attributes
- Labels for icons
- Semantic landmarks (header, nav, main, footer)

## Responsive Design

### Breakpoints

```css
--bs-breakpoint-xs: 0;
--bs-breakpoint-sm: 576px;
--bs-breakpoint-md: 768px;
--bs-breakpoint-lg: 992px;
--bs-breakpoint-xl: 1200px;
--bs-breakpoint-xxl: 1400px;
```

### Strategy

- **Mobile First** : Design optimized for mobile, then progressive enhancement
- **Flexible Grid** : Bootstrap 5.3 grid that adapts automatically
- **Responsive Images** : Bootstrap `img-fluid` class for adaptive images
- **Fluid Typography** : Use of `clamp()` for font sizes (modern CSS)
- **Responsive Utilities** : Bootstrap classes with breakpoints

## Implementation

### CSS Custom Properties

All values are defined as CSS variables in `:root` for easy maintenance and customization.

### Component Structure

Components use semantic HTML with Bootstrap utility classes for structure, but all visual styles are completely custom.

### Recommended CDN

```html
<!-- Bootstrap 5.3.3 CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- Bootstrap Icons 1.11.3 -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.css">

<!-- Bootstrap 5.3.3 JavaScript Bundle -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

