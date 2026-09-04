---
name: Kinetic Green Corporate
colors:
  surface: '#f7faf8'
  surface-dim: '#d8dbd9'
  surface-bright: '#f7faf8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f4f2'
  surface-container: '#eceeed'
  surface-container-high: '#e6e9e7'
  surface-container-highest: '#e0e3e1'
  on-surface: '#181c1c'
  on-surface-variant: '#3f4947'
  inverse-surface: '#2d3130'
  inverse-on-surface: '#eef1f0'
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
  secondary-container: '#c0e7e3'
  on-secondary-container: '#456966'
  tertiary: '#673119'
  on-tertiary: '#ffffff'
  tertiary-container: '#83472e'
  on-tertiary-container: '#ffbfa6'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#a4f1e7'
  primary-fixed-dim: '#88d4cb'
  on-primary-fixed: '#00201d'
  on-primary-fixed-variant: '#00504a'
  secondary-fixed: '#c3eae6'
  secondary-fixed-dim: '#a7ceca'
  on-secondary-fixed: '#00201e'
  on-secondary-fixed-variant: '#284d4a'
  tertiary-fixed: '#ffdbce'
  tertiary-fixed-dim: '#ffb599'
  on-tertiary-fixed: '#370e00'
  on-tertiary-fixed-variant: '#6f371f'
  background: '#f7faf8'
  on-background: '#181c1c'
  surface-variant: '#e0e3e1'
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
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
---

## Brand & Style

The design system is engineered for high-performance fleet management and sustainable technology sectors. The brand personality is rooted in "Controlled Energy"—a balance between the rapid pace of real-time data and the professional stability required for enterprise operations. 

The aesthetic follows a **Modern Corporate** direction with a focus on data density and functional clarity. It avoids unnecessary decoration, instead using precision-engineered spacing and a cool-toned palette to evoke a sense of reliability and environmental consciousness. The UI should feel fast, responsive, and authoritative, providing users with the confidence to manage complex logistics at scale.

## Colors

The palette is anchored by "Deep Kinetic Green" (#00625b), a color that signals both growth and professional maturity. 

- **Primary:** Used for key actions, active states, and brand identification.
- **Secondary:** Employed for deep-background navigation elements and heavy-duty UI framing.
- **Surface:** A cool, mint-tinted off-white (#f7faf8) that reduces eye strain during long-duration monitoring compared to pure white.
- **Data Visualization:** Use the primary green for "Optimal" states, but maintain standard semantic colors (Red/Amber) for critical alerts to ensure safety compliance in fleet monitoring.

## Typography

Typography is prioritized for legibility in information-dense environments. 

1. **Interface Text:** Use **Inter** for all standard UI elements. It provides excellent x-height for readability in small sizes (tables/sidebars).
2. **Technical Data:** Use **JetBrains Mono** for numerical values, timestamps, GPS coordinates, and vehicle IDs. The monospaced nature ensures that shifting values do not cause layout jumps in real-time dashboards.
3. **Hierarchy:** Use `label-caps` for table headers and section titles to differentiate them from actionable content.

## Layout & Spacing

This design system utilizes a **4px baseline grid** to achieve high data density without clutter. 

- **Grid System:** A 12-column fluid grid for desktop dashboards, collapsing to a single column for mobile monitoring.
- **Density:** Dashboard widgets should use `sm` (8px) internal padding to maximize the "above-the-fold" information. 
- **Alignment:** All data points in a vertical list must align to the 4px grid to maintain visual rhythm during rapid scrolling.
- **Breakpoints:** 
  - Mobile: < 600px
  - Tablet: 600px - 1024px
  - Desktop: > 1024px (Standard view for dispatchers)

## Elevation & Depth

To maintain a "Professional/Modern" feel, depth is communicated through **Tonal Layering** and **Thin Outlines** rather than heavy shadows.

- **Level 0 (Surface):** The background (#f7faf8).
- **Level 1 (Card):** White background with a 1px border (#e0e7e3). No shadow.
- **Level 2 (Hover/Active):** White background with a very soft, tight shadow (Blur: 4px, Y: 2px, Opacity: 0.05, Color: #1e4340) and the primary border color.
- **Level 3 (Modals):** White background with a diffused shadow to indicate focus and separation from the monitoring grid.

## Shapes

The shape language is **Soft**, striking a balance between the "hard" nature of heavy machinery and the "soft" nature of modern software.

- **Components:** Standard buttons, input fields, and small cards use a **4px (0.25rem)** corner radius.
- **Containers:** Dashboard widgets and larger sections use an **8px (0.5rem)** radius.
- **Interactive Indicators:** Active states in sidebars or segmented controls use the 4px radius for a crisp, precise appearance.

## Components

### Buttons
- **Primary:** Solid #00625b with white text. 4px radius. High contrast for critical actions (e.g., "Deploy Fleet").
- **Secondary:** Outline #00625b or tonal fill.
- **Status Buttons:** Used in tables; small height (28px), JetBrains Mono text.

### Input Fields
- Understated style: 1px border (#ced9d2) on #ffffff background. 
- Focus state: 2px border #00625b.
- Labels are always persistent; do not use floating labels to ensure clarity in dense forms.

### Data Cards & Widgets
- White fill, 1px border (#e0e7e3).
- Headers should have a subtle bottom border to separate titles from metrics.
- Sparklines (mini-graphs) should use the primary green with a subtle fill gradient.

### Status Chips
- Pill-shaped but with the same 4px soft corner logic. 
- Use low-saturation backgrounds with high-saturation text (e.g., Light Red background with Deep Red text) for "Vehicle Offline" or "Low Battery" alerts.

### Navigation
- Sidebar: Secondary color (#1e4340) background with low-opacity white icons. 
- Active state: Left-edge accent line in primary green (#00625b).