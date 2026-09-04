---
name: Kinetic Desktop
colors:
  surface: '#f7faf8'
  surface-dim: '#d7dbd9'
  surface-bright: '#f7faf8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f4f2'
  surface-container: '#eceeed'
  surface-container-high: '#e6e9e7'
  surface-container-highest: '#e0e3e1'
  on-surface: '#181c1c'
  on-surface-variant: '#3f4947'
  inverse-surface: '#2d3130'
  inverse-on-surface: '#eef1ef'
  outline: '#6f7977'
  outline-variant: '#bec9c6'
  surface-tint: '#126a62'
  primary: '#004843'
  on-primary: '#ffffff'
  primary-container: '#00625b'
  on-primary-container: '#8fdbd1'
  inverse-primary: '#88d4cb'
  secondary: '#406561'
  on-secondary: '#ffffff'
  secondary-container: '#c0e8e2'
  on-secondary-container: '#446965'
  tertiary: '#663119'
  on-tertiary: '#ffffff'
  tertiary-container: '#83472d'
  on-tertiary-container: '#ffbfa5'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#a4f1e7'
  primary-fixed-dim: '#88d4cb'
  on-primary-fixed: '#00201d'
  on-primary-fixed-variant: '#00504a'
  secondary-fixed: '#c2eae5'
  secondary-fixed-dim: '#a7cec9'
  on-secondary-fixed: '#00201e'
  on-secondary-fixed-variant: '#284d49'
  tertiary-fixed: '#ffdbce'
  tertiary-fixed-dim: '#ffb598'
  on-tertiary-fixed: '#370e00'
  on-tertiary-fixed-variant: '#6f371f'
  background: '#f7faf8'
  on-background: '#181c1c'
  surface-variant: '#e0e3e1'
  sidebar-bg: '#1e4340'
  on-sidebar: '#eef1f0'
  border-subtle: '#e0e7e3'
  success: '#126a62'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
  data-mono-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.06em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  sidebar-width: 280px
  margin: 32px
  gutter: 24px
  widget-padding: 16px
  compact-padding: 8px
  base-unit: 4px
---

## Brand & Style

The design system is a high-density, professional adaptation of a sustainable technology identity, specifically refined for complex desktop-class data management. The brand personality is "Industrial Precision"—a synthesis of the rugged reliability required for fleet operations and the sophisticated technicality of modern software.

The aesthetic utilizes **Minimalism** with a **Bento-Box** layout structure to organize vast amounts of information into digestible, modular segments. By prioritizing whitespace within modules and using a cold, mint-tinted neutral palette, the design system minimizes cognitive load while maintaining an authoritative presence. It avoids decorative flourishes in favor of functional clarity, ensuring the UI remains performant and focused for long-duration enterprise use.

## Colors

The palette is centered around **Persian Green (#00625b)**, which serves as the anchor for primary actions and brand recognition. 

- **Primary & Tints:** Persian Green is used for active states, primary buttons, and critical data highlights.
- **Surface Strategy:** The system uses a multi-tiered neutral approach. The main background is a cool-tinted off-white to reduce glare, while container surfaces use subtle shifts in lightness to create visual separation without heavy borders.
- **Sidebar:** A specific dark-green variant is reserved for the fixed navigation to provide a strong structural frame and clear hierarchy between "where I am" and "what I am doing."
- **Data Visualization:** Maintain the primary green for healthy metrics, but utilize the high-contrast `error` red for critical system alerts.

## Typography

Typography is optimized for a technical, data-dense desktop environment. 

1. **Inter** is the workhorse for the interface, providing high legibility for menus, forms, and descriptive text. 
2. **JetBrains Mono** is strictly reserved for quantitative data—GPS coordinates, timestamps, and fleet IDs—to prevent layout shifts when data refreshes in real-time.
3. **Hierarchy:** `label-caps` should be used for metadata and table headers to create a distinct visual layer that separates "framework" from "content." 
4. **Density:** In high-density widgets, prefer `body-sm` and `data-mono-sm` to maximize information visibility without sacrificing readability.

## Layout & Spacing

This design system uses a **Fixed-Fluid Hybrid** layout model.

- **Sidebar:** A fixed 280px left navigation provides persistent access to global tools.
- **Main Content:** A 12-column fluid grid with 32px outer margins and 24px gutters. 
- **Bento Dashboard:** Content is organized into cards (widgets) that span varying column counts (e.g., 3, 4, 6, or 12). 
- **Vertical Rhythm:** A strict 4px baseline grid ensures that even in high-density tables, text and iconography feel aligned and intentional. 
- **Density Controls:** Use `widget-padding` for standard content and `compact-padding` for data-heavy monitoring tools.

## Elevation & Depth

Visual hierarchy is primarily driven by **Tonal Layering** and **Subtle Outlines** to keep the interface feeling light and responsive.

- **Surface Levels:** The background uses the neutral surface color. Dashboard widgets are elevated using a white background and a 1px `border-subtle` (#e0e7e3).
- **Interactive Depth:** On hover, widgets or actionable cards should transition to a 1px border using the primary green and a very soft, low-opacity shadow (Blur: 8px, Offset-Y: 4px, Color: 5% alpha primary green).
- **Modals & Overlays:** Use a more pronounced diffused shadow to separate critical interrupts from the grid, ensuring the background remains visible but clearly inactive.

## Shapes

The shape language is **Soft (0.25rem)**, reflecting a professional and engineered precision.

- **Small Components:** Buttons, inputs, and tags use the 4px base radius.
- **Containers:** Large dashboard widgets and bento-cards use `rounded-lg` (8px) to soften the overall grid structure.
- **Consistency:** Avoid pill shapes for buttons to maintain the "Corporate Modern" aesthetic; reserve pill shapes only for status chips to distinguish them from actionable buttons.

## Components

### Navigation Sidebar
The 280px sidebar uses the `sidebar-bg`. Navigation items should have a 16px horizontal padding. The active state is indicated by a 4px primary green vertical bar on the extreme left edge and a subtle tonal shift in the item background.

### Bento Widgets
Cards must have a consistent 1px `border-subtle`. Headers within widgets should use `label-caps` for the title and a bottom border to separate the header from the data area.

### Buttons
- **Primary:** Persian Green fill, white text, 4px radius.
- **Ghost:** Primary color text, no background. Used for secondary actions within dense tables.
- **Data-Action:** Small-height (32px) buttons using `data-mono` for numerical actions.

### Input Fields
Standardized on a "Compact" height (36px for desktop). Use a persistent top-aligned label in `label-caps` style. Background should be white with a 1px `border-subtle`, changing to a 2px Persian Green border on focus.

### Status Chips
Pill-shaped with a 0.125rem radius. Use the "Low-Saturation Background / High-Saturation Text" formula:
- **Active:** Light green background / Deep green text.
- **Warning:** Pale amber background / Dark amber text.
- **Critical:** Light red background / Deep red text.