# Neobrutalist Design System

## Overview

This design system was created to modernize a GitHub Pages personal site with a **radically different visual identity**: a **neobrutalist style** with geometric shapes, vibrant colors, and thick borders. It uses Bootstrap 5.3.3 **only for structure and responsive**, all visual styles are completely customized.

## Design Principles

1. **Neobrutalist Style** : Geometric shapes, thick borders, offset shadows
2. **Vibrant Colors** : Contrasted and bold palette
3. **Bold Typography** : Uppercase, high weights, tight letter-spacing
4. **Unique Identity** : No visual resemblance to default Bootstrap
5. **Accessibility** : WCAG 2.1 AA compliance despite bold style

## Color Palette

### Primary Colors - Brutalist Style

```css
--color-primary: #FF6B6B;        /* Vibrant coral red - primary color */
--color-primary-dark: #EE5A52;  /* Dark red - hover states */
--color-primary-light: #FF8787;  /* Light red - variants */

--color-secondary: #4ECDC4;     /* Vibrant turquoise - secondary color */
--color-accent: #FFE66D;         /* Vibrant yellow - accents, highlights */
--color-warning: #FFA07A;        /* Salmon - warnings */
--color-error: #FF4757;          /* Vibrant red - errors */
--color-info: #74B9FF;           /* Vibrant blue - information */
```

### Neutral Colors - Warm Tones

```css
--color-bg-primary: #FFF8F0;     /* Warm cream - primary background */
--color-bg-secondary: #FFE5D9;   /* Light peach - secondary background */
--color-bg-tertiary: #FFD7C7;    /* Peach - tertiary background */
--color-bg-dark: #2D3436;        /* Dark gray - header, code */
--color-bg-dark-light: #636E72;  /* Medium gray */

--color-text-primary: #2D3436;   /* Very dark gray - primary text */
--color-text-secondary: #636E72; /* Medium gray - secondary text */
--color-text-muted: #B2BEC3;     /* Light gray - muted text */
--color-text-inverse: #FFFFFF;    /* White - text on dark background */

--color-border: #2D3436;         /* Very dark gray - borders */
--color-border-dark: #000000;    /* Black - thick borders */
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
--font-size-lg: 1.25rem;     /* 20px */
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

- **H1** : Main page title (3.5rem, bold, uppercase)
- **H2** : Main sections (2.75rem, bold, uppercase)
- **H3** : Subsections (2.25rem, bold, uppercase)
- **H4-H6** : Card titles, lists (1.75rem - 1.25rem, bold, uppercase)
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

All borders are in `--color-border-dark` (black) for maximum contrast.

## Shadows - Brutalist Offset Style

Black offset shadows (classic brutalist style):

```css
--shadow-brutal-sm: 4px 4px 0 0 var(--color-border-dark);   /* Small shadow */
--shadow-brutal: 8px 8px 0 0 var(--color-border-dark);      /* Standard shadow */
--shadow-brutal-lg: 12px 12px 0 0 var(--color-border-dark); /* Large shadow */
```

Shadows are always black and offset to bottom-right, creating a brutalist 3D effect.

## Components

All components use custom visual styles with a unique neobrutalist identity.

### Buttons

**Custom Styles** :
- Thick black borders (5px)
- Offset shadows
- Hover animation: `translate(4px, 4px)` removing shadow
- Uppercase text, bold weight
- Vibrant solid colors

**Available Variants** :
- `btn-primary` : Coral red with black border
- `btn-secondary` : Turquoise with black border
- `btn-outline-primary` : Outlined style
- `btn-success` : Yellow accent
- `btn-danger` : Red error

### Cards

**Custom Styles** :
- Thick black borders (5px)
- Offset shadows
- Geometric shapes (no border-radius)
- Hover effect: `translate(-4px, -4px)` with larger shadow
- Accent border overlay effect

### Badges

**Custom Styles** :
- Rectangular shapes (no border-radius)
- Thick black borders
- Offset shadows
- Uppercase text, bold weight
- Vibrant solid colors

### Alerts

**Custom Styles** :
- Thick black borders (5px)
- Vibrant solid backgrounds
- Offset shadows
- Bold typography
- No border-radius

### Navigation

**Custom Styles** :
- Thick black borders
- Offset shadows
- Hover effect with background color change
- Uppercase links, bold weight
- Fast transitions

### Links

**Custom Styles** :
- Underlined with thick line (2-3px)
- Primary color
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

- Outline: 3px solid `--color-primary`
- No border-radius
- Fast transition

### Disabled

- Opacity: 0.5
- Cursor: not-allowed
- Pointer-events: none

### Loading

- Animated spinner
- Reduced opacity on content
- Cursor: wait

## Accessibility

### Contrast

- All texts respect a minimum contrast ratio of 4.5:1
- Text on dark backgrounds: minimum ratio of 7:1

### Keyboard Navigation

- All interactive elements are keyboard accessible
- Visible and clear focus
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
- **Responsive Utilities** : Bootstrap classes with breakpoints (`d-md-none`, `text-lg-center`, etc.)

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

