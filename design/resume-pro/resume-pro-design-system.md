# Resume Pro Design System

A professional, print-optimized design system specifically crafted for resumes and CVs. Prioritizes readability, information hierarchy, and flawless rendering across desktop, mobile, and print media (PDF and paper).

## Design Principles

1. **Readability First** : Clear typography, generous spacing, optimal contrast
2. **Information Hierarchy** : Visual structure that guides the eye to important information
3. **Print-Optimized** : Designed to look perfect when printed or exported to PDF
4. **Responsive** : Adapts seamlessly from desktop to mobile
5. **Professional** : Clean, modern, and timeless aesthetic
6. **Accessible** : High contrast, semantic HTML, screen reader friendly

## Color Palette

### Primary Colors

```css
--color-primary: #1a1a1a;        /* Deep black for text */
--color-secondary: #2c3e50;      /* Dark blue-gray for accents */
--color-accent: #3498db;         /* Professional blue for links */
--color-muted: #7f8c8d;          /* Gray for secondary text */
```

### Background Colors

```css
--color-bg-primary: #ffffff;     /* Pure white background */
--color-bg-secondary: #f8f9fa;   /* Light gray for sections */
--color-bg-accent: #ecf0f1;      /* Subtle accent background */
```

### Border Colors

```css
--color-border: #e0e0e0;          /* Light border */
--color-border-accent: #bdc3c7;  /* Medium border */
```

### Print Colors

All colors are optimized to work in grayscale and black & white printing. The design maintains excellent contrast when printed.

## Typography

### Font Families

```css
--font-primary: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Helvetica Neue', Arial, sans-serif;
--font-mono: 'Courier New', Courier, monospace;
```

**Rationale** : System fonts ensure fast loading, excellent readability, and perfect rendering in print.

### Font Sizes

```css
--font-size-xs: 0.75rem;    /* 12px - Small labels */
--font-size-sm: 0.875rem;   /* 14px - Secondary text */
--font-size-base: 1rem;     /* 16px - Body text */
--font-size-lg: 1.125rem;   /* 18px - Subheadings */
--font-size-xl: 1.25rem;    /* 20px - Section titles */
--font-size-2xl: 1.5rem;    /* 24px - Card titles */
--font-size-3xl: 1.875rem;  /* 30px - Page title */
--font-size-4xl: 2.25rem;   /* 36px - Main heading */
```

### Font Weights

```css
--font-weight-light: 300;
--font-weight-normal: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
```

### Line Heights

```css
--line-height-tight: 1.25;
--line-height-normal: 1.5;
--line-height-relaxed: 1.75;
```

### Typography Scale

- **H1 (Name)** : `2.25rem`, `bold`, `line-height: 1.2`
- **H2 (Title/Position)** : `1.5rem`, `semibold`, `line-height: 1.3`
- **H3 (Section Titles)** : `1.25rem`, `semibold`, `line-height: 1.4`
- **H4 (Subsection Titles)** : `1.125rem`, `medium`, `line-height: 1.4`
- **H5 (Item Titles)** : `1rem`, `semibold`, `line-height: 1.5`
- **H6 (Dates/Locations)** : `0.875rem`, `normal`, `color: muted`
- **Body** : `1rem`, `normal`, `line-height: 1.6`
- **Small** : `0.875rem`, `normal`, `line-height: 1.5`

## Spacing

### Spacing Scale

```css
--spacing-xs: 0.25rem;   /* 4px */
--spacing-sm: 0.5rem;    /* 8px */
--spacing-md: 0.75rem;   /* 12px */
--spacing-base: 1rem;    /* 16px */
--spacing-lg: 1.5rem;    /* 24px */
--spacing-xl: 2rem;      /* 32px */
--spacing-2xl: 3rem;     /* 48px */
--spacing-3xl: 4rem;     /* 64px */
```

### Usage Guidelines

- **Section spacing** : `--spacing-2xl` (48px) between major sections
- **Card padding** : `--spacing-xl` (32px) on desktop, `--spacing-lg` (24px) on mobile
- **Item spacing** : `--spacing-lg` (24px) between items within a section
- **Text spacing** : `--spacing-base` (16px) between paragraphs
- **Compact spacing** : `--spacing-md` (12px) for tight lists

## Layout

### Container

```css
--container-max-width: 210mm;    /* A4 width */
--container-padding: var(--spacing-xl);
```

**Rationale** : A4 width (210mm) ensures perfect fit when printing or exporting to PDF.

### Grid System

Uses Bootstrap 5.3 grid system (12 columns) for structure:
- Classes: `row`, `col`, `col-{breakpoint}-{size}`
- Breakpoints: xs, sm, md, lg, xl, xxl
- Gaps: `g-*`, `gx-*`, `gy-*` for spacing

### Layout Structure

**Desktop (≥992px)** :
- Two-column layout: Main content (8 cols) + Sidebar (4 cols)
- Maximum width: 210mm (A4 width)
- Generous margins for readability

**Tablet (768px - 991px)** :
- Single column layout
- Full width with padding

**Mobile (<768px)** :
- Single column layout
- Reduced padding for space efficiency

**Print** :
- Single column layout (sidebar content flows below)
- Optimized margins and spacing
- Page breaks controlled to avoid awkward splits

## Components

### Header

**Purpose** : Display name, title, and contact information prominently.

**Structure** :
- Name (H1) - Large, bold
- Title/Position (H2) - Medium, semibold
- Contact info (optional) - Small, muted

**Styles** :
- Dark background (`--color-secondary`) with white text
- Generous padding (`--spacing-2xl`)
- Clean, professional appearance

### Sections

**Purpose** : Organize content into logical groups.

**Structure** :
- Section title (H3) with bottom border
- Section content in cards or lists

**Styles** :
- Clear visual separation
- Consistent spacing
- Print-friendly borders

### Cards

**Purpose** : Group related content with clear boundaries.

**Custom Styles** :
- White background with subtle border
- Generous padding (`--spacing-xl`)
- Soft shadow (screen only, removed in print)
- Clean, minimal design
- No background animations or effects

### Experience Items

**Purpose** : Display work experience, education, or projects.

**Structure** :
- Title (H5) - Job title, degree, or project name
- Meta (H6) - Dates, location, company
- Description - Bullet points or paragraphs
- Technologies (optional) - Small, muted text

**Styles** :
- Clear hierarchy
- Generous spacing between items
- Horizontal rule separator
- Print-optimized spacing

### Skills Lists

**Purpose** : Display technical skills, languages, or competencies.

**Structure** :
- Category title (bold)
- Skills (comma-separated or bulleted)

**Styles** :
- Clean, scannable format
- Consistent spacing
- Easy to read in print

### Links

**Custom Styles** :
- Professional blue color (`--color-accent`)
- Underline on hover (screen only)
- Full URL displayed in print
- No color changes in print

### Dividers

**Purpose** : Separate content items.

**Styles** :
- Light horizontal rule (`<hr>`)
- Consistent spacing
- Subtle color

## Print Optimization

### Print Media Queries

```css
@media print {
    /* Remove shadows and effects */
    box-shadow: none !important;
    text-shadow: none !important;
    
    /* Optimize colors for print */
    color: #000 !important;
    background: #fff !important;
    
    /* Control page breaks */
    page-break-inside: avoid;
    page-break-after: auto;
    
    /* Optimize spacing */
    margin: 0;
    padding: var(--spacing-lg);
    
    /* Show URLs */
    a[href]:after {
        content: " (" attr(href) ")";
    }
    
    /* Hide non-essential elements */
    .no-print {
        display: none !important;
    }
}
```

### Print-Specific Features

1. **Page Breaks** : Sections avoid breaking across pages
2. **URL Display** : Links show full URLs in print
3. **Color Optimization** : All colors work in grayscale
4. **Spacing** : Optimized margins and padding for paper
5. **Font Sizes** : Slightly adjusted for print readability
6. **Backgrounds** : Removed or simplified for print

## Responsive Design

### Breakpoints

```css
--breakpoint-sm: 576px;
--breakpoint-md: 768px;
--breakpoint-lg: 992px;
--breakpoint-xl: 1200px;
--breakpoint-xxl: 1400px;
```

### Mobile Optimizations

- Single column layout
- Reduced padding
- Larger touch targets
- Optimized font sizes
- Stacked contact information

### Desktop Optimizations

- Two-column layout (main + sidebar)
- Generous spacing
- Optimal line length
- Sidebar for secondary information

## Accessibility

### Contrast Ratios

- Text on white: 16:1 (WCAG AAA)
- Text on dark: 12:1 (WCAG AAA)
- Links: 4.5:1 minimum (WCAG AA)

### Semantic HTML

- Proper heading hierarchy (H1 → H6)
- Semantic elements (`<section>`, `<article>`, `<nav>`)
- ARIA labels where appropriate
- Alt text for images

### Screen Readers

- Logical content order
- Descriptive link text
- Proper form labels
- Skip navigation links

## Best Practices

### Content Organization

1. **Header** : Name, title, contact info
2. **Profile/Summary** : Brief professional summary (optional)
3. **Experience** : Work history in reverse chronological order
4. **Education** : Degrees and certifications
5. **Skills** : Technical and soft skills
6. **Projects** : Notable projects (optional)
7. **Additional** : Languages, certifications, etc.

### Writing Guidelines

1. Use action verbs
2. Quantify achievements
3. Keep descriptions concise
4. Use bullet points for readability
5. Maintain consistent formatting

### Design Guidelines

1. Keep it simple and clean
2. Use consistent spacing
3. Maintain clear hierarchy
4. Avoid clutter
5. Test in print before finalizing

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Print functionality in all major browsers
- PDF export via browser print-to-PDF
- Mobile browsers (iOS Safari, Chrome Mobile)

## Usage

### Basic Structure

```html
<div class="container resume-container">
    <!-- Header -->
    <header class="resume-header">
        <h1>Your Name</h1>
        <h2>Your Title</h2>
    </header>
    
    <div class="row">
        <!-- Main Content -->
        <div class="col-lg-8">
            <section class="resume-section">
                <h3>Experience</h3>
                <!-- Experience items -->
            </section>
        </div>
        
        <!-- Sidebar -->
        <div class="col-lg-4">
            <section class="resume-section">
                <h3>Skills</h3>
                <!-- Skills content -->
            </section>
        </div>
    </div>
</div>
```

### Customization

The design system uses CSS custom properties (variables) for easy theming. Modify the color, spacing, or typography variables to match your brand while maintaining print compatibility.

