# Aether Brutal Design System

## Overview

Aether Brutal is a bold, tech-focused design system that combines the vibrant tech color palette of Aether Prism (on light backgrounds) with the geometric, hard-edged aesthetic of Neo Brutalist design. It features thick borders, offset shadows, and a light tech-inspired color scheme, creating a unique visual identity that's both modern and impactful. The system uses Bootstrap 5.3.3 only for structure and responsive layout, with all visual styles completely customized.

## Design Principles

1. **Brutalist Geometry** : Sharp edges, no border-radius, thick borders
2. **Light Tech Color Palette** : Indigo, purple, cyan on light backgrounds
3. **Bold Typography** : High contrast, readable fonts with strong hierarchy
4. **Offset Shadows** : Classic brutalist black offset shadows for depth
5. **Unique Identity** : No visual resemblance to default Bootstrap
6. **Accessibility** : WCAG 2.1 AA compliance despite bold style

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

### Neutral Colors - Light Professional Backgrounds

```css
--color-bg-primary: #FFFFFF;     /* White - primary background */
--color-bg-secondary: #F8FAFC;   /* Slate 50 - secondary background */
--color-bg-tertiary: #F1F5F9;    /* Slate 100 - tertiary background */
--color-bg-dark: #0F172A;        /* Slate 900 - dark accents */

--color-text-primary: #0F172A;   /* Slate 900 - primary text */
--color-text-secondary: #475569;  /* Slate 600 - secondary text */
--color-text-muted: #94A3B8;     /* Slate 400 - muted text */
--color-text-inverse: #FFFFFF;   /* White text on dark background */

--color-border: #E2E8F0;         /* Slate 200 - borders */
--color-border-light: #CBD5E1;   /* Slate 300 - light borders */
--color-border-dark: #000000;    /* Black - thick brutalist borders */
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
--font-size-h1: 3.5rem;      /* 56px */
--font-size-h2: 2.75rem;     /* 44px */
--font-size-h3: 2.25rem;     /* 36px */
--font-size-h4: 1.75rem;     /* 28px */
--font-size-h5: 1.5rem;      /* 24px */
--font-size-h6: 1.25rem;     /* 20px */

/* Body text */
--font-size-base: 1.125rem;  /* 18px */
--font-size-sm: 1rem;         /* 16px */
--font-size-xs: 0.875rem;     /* 14px */
--font-size-lg: 1.25rem;      /* 20px */
--font-size-xl: 1.5rem;      /* 24px */

/* Weights */
--font-weight-light: 300;
--font-weight-normal: 400;
--font-weight-medium: 600;
--font-weight-semibold: 700;
--font-weight-bold: 800;

/* Line heights */
--line-height-tight: 1.2;
--line-height-normal: 1.5;
--line-height-relaxed: 1.8;
```

### Usage Examples

- **H1** : Main page title (3.5rem, bold)
- **H2** : Main sections (2.75rem, bold)
- **H3** : Subsections (2.25rem, semibold)
- **H4-H6** : Card titles, lists (1.75rem - 1.25rem, semibold)
- **Body** : Regular text (1.125rem, normal, line-height: 1.8)
- **Small** : Metadata, dates (1rem, normal)

## Spacing

### Spacing System (generous spacing)

```css
--spacing-xs: 0.5rem;      /* 8px */
--spacing-sm: 1rem;        /* 16px */
--spacing-md: 1.5rem;      /* 24px */
--spacing-lg: 2.5rem;      /* 40px */
--spacing-xl: 4rem;        /* 64px */
--spacing-2xl: 6rem;       /* 96px */
--spacing-3xl: 8rem;       /* 128px */
--spacing-4xl: 12rem;      /* 192px */
```

### Usage

- **xs** : Minimal internal spacing (icons, badges)
- **sm** : Spacing between close elements
- **md** : Standard spacing (card padding)
- **lg** : Spacing between sections
- **xl** : Spacing between major sections
- **2xl-4xl** : Spacing between major blocks

## Borders - Brutalist Style

**No border-radius** - Geometric shapes only:

```css
--border-radius: 0;  /* No rounding - square/rectangular shapes */

--border-width: 3px;           /* Standard border */
--border-width-thick: 5px;     /* Thick border */
--border-width-extra: 8px;      /* Extra thick border (headers) */
```

All borders use `--color-border-dark` (black) for maximum contrast and brutalist aesthetic.

## Shadows - Brutalist Offset Style

Black offset shadows (classic brutalist style):

```css
--shadow-brutal-sm: 4px 4px 0 0 var(--color-border-dark);   /* Small shadow */
--shadow-brutal: 8px 8px 0 0 var(--color-border-dark);      /* Standard shadow */
--shadow-brutal-lg: 12px 12px 0 0 var(--color-border-dark); /* Large shadow */
```

Shadows are always black and offset to bottom-right, creating a brutalist 3D effect.

## Components

All components use custom visual styles with a unique brutalist-tech identity on light backgrounds.

### Buttons

**Custom Styles** :
- Thick black borders (5px)
- Offset shadows
- Hover animation: `translate(4px, 4px)` removing shadow
- Bold weight, uppercase text (optional)
- Tech-inspired solid colors (indigo, purple, cyan)

**Available Variants** :
- `btn-primary` : Indigo with black border
- `btn-secondary` : Purple with black border
- `btn-accent` : Cyan with black border
- `btn-outline-primary` : Outlined style with tech colors
- `btn-success` : Emerald gradient
- `btn-danger` : Red error

### Cards

**Custom Styles** :
- Thick black borders (5px)
- Offset shadows
- Geometric shapes (no border-radius)
- Light tech backgrounds (white, slate 50/100)
- Hover effect: `translate(-4px, -4px)` with larger shadow
- Tech color accent borders (optional)

### Badges

**Custom Styles** :
- Rectangular shapes (no border-radius)
- Thick black borders
- Offset shadows
- Bold weight, uppercase text
- Tech-inspired solid colors

### Alerts

**Custom Styles** :
- Thick black borders (5px)
- Tech color backgrounds (indigo, purple, cyan variants)
- Offset shadows
- Bold typography
- No border-radius

### Navigation

**Custom Styles** :
- Thick black borders
- Offset shadows
- Light tech background
- Hover effect with tech color background change
- Bold links, semibold weight
- Fast transitions

### Links

**Custom Styles** :
- Underlined with thick line (2-3px)
- Tech primary color (indigo)
- Hover: darker color, thicker underline
- Medium font weight

## Layout

### Container

```css
--container-max-width: 1400px;
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
- Thick borders and offset shadows
- Light tech backgrounds

## Animations and Transitions

```css
--transition-fast: 100ms cubic-bezier(0.4, 0, 0.2, 1);
--transition-base: 150ms cubic-bezier(0.4, 0, 0.2, 1);
--transition-slow: 200ms cubic-bezier(0.4, 0, 0.2, 1);
```

**Common Uses** :
- Hover states: `--transition-base`
- Interactive elements: `--transition-fast`
- Complex animations: `--transition-slow`

## Interactive States

### Focus

- Outline: 3px solid `--color-primary` (indigo)
- No border-radius
- Fast transition

### Disabled

- Opacity: 0.5
- Cursor: not-allowed
- Pointer-events: none

### Loading

- Animated spinner with tech colors
- Reduced opacity on content
- Cursor: wait

## Accessibility

### Contrast

- All texts respect a minimum contrast ratio of 4.5:1
- Text on light backgrounds: dark text for maximum readability
- Tech colors on light backgrounds maintain excellent contrast

### Keyboard Navigation

- All interactive elements are keyboard accessible
- Visible and clear focus with tech color outline
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

## Color Combinations

### Recommended Pairings

- **Primary (Indigo) + Accent (Cyan)** : High contrast, tech-forward
- **Secondary (Purple) + Primary (Indigo)** : Harmonious tech palette
- **Light Background + Tech Colors** : Maximum impact and readability
- **White Background + Dark Text** : For optimal contrast

### Usage Guidelines

- Use light backgrounds (white, slate 50/100) as primary surfaces
- Apply tech colors (indigo, purple, cyan) for accents and interactive elements
- Maintain high contrast for readability
- Use black borders consistently for brutalist aesthetic

