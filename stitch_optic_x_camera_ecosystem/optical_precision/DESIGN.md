---
name: Optical Precision
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#37393a'
  surface-container-lowest: '#0c0f0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#282a2b'
  surface-container-highest: '#333535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#c4c7c7'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c8c6c5'
  primary: '#c8c6c5'
  on-primary: '#313030'
  primary-container: '#121212'
  on-primary-container: '#7e7d7d'
  inverse-primary: '#5f5e5e'
  secondary: '#c8c6c5'
  on-secondary: '#303030'
  secondary-container: '#474747'
  on-secondary-container: '#b6b5b4'
  tertiary: '#00daf3'
  on-tertiary: '#00363d'
  tertiary-container: '#001519'
  on-tertiary-container: '#008a9a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c8c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474646'
  secondary-fixed: '#e4e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#474747'
  tertiary-fixed: '#9cf0ff'
  tertiary-fixed-dim: '#00daf3'
  on-tertiary-fixed: '#001f24'
  on-tertiary-fixed-variant: '#004f58'
  background: '#121414'
  on-background: '#e2e2e2'
  surface-variant: '#333535'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  body-base:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  data-mono:
    fontFamily: spaceGrotesk
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.05em
  label-caps:
    fontFamily: spaceGrotesk
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 16px
  margin: 32px
  container-max: 1440px
---

## Brand & Style
The brand personality of this design system is defined by "Technical Authority." It is designed to evoke the feeling of looking through a high-end electronic viewfinder (EVF). The aesthetic is a fusion of **Minimalism** and **Glassmorphism**, prioritizing clarity, precision, and high-performance utility.

The UI should feel like a professional instrument rather than a consumer app. This is achieved through a "Heads-Up Display" (HUD) approach, where information is layered over high-fidelity imagery using translucent surfaces and razor-thin strokes. The emotional response is one of confidence and clinical accuracy, mirroring the mechanical excellence of flagship mirrorless hardware.

## Colors
This design system utilizes a "Deep Field" dark mode palette to ensure that visual content remains the focal point while UI elements recede into the background.

- **Primary (Matte Black):** The foundation of the interface, providing a non-reflective, high-contrast base.
- **Secondary (Graphite):** Used for structural surfaces, defining the physical limits of containers and panels.
- **Tertiary (Cyan):** The "Active State" color, representing focus, recording status, and digital precision.
- **Accent (Amber):** Reserved for technical warnings, secondary data points, and "Standby" or "Manual" indicators.
- **Neutral (Pure White):** Used exclusively for high-contrast typography and critical iconography to ensure maximum legibility against dark backgrounds.

## Typography
The typography strategy centers on the contrast between editorial clarity and technical metadata. 

- **Headlines:** Use **Inter** with heavy weights and tight letter spacing to project authority and modernism.
- **Body Text:** **Inter** provides a neutral, highly readable foundation for long-form technical descriptions.
- **Technical Data:** **Space Grotesk** is utilized for all HUD elements, spec tables, and numerical data. Its geometric construction mimics the look of monospaced engineering displays, ensuring that changing digits (like shutter speeds or ISO) do not cause layout shifts. 
- **Labels:** Small-caps are used for secondary UI labels to maintain a compact, instrument-like feel.

## Layout & Spacing
The layout follows a **Fixed Grid** philosophy rooted in a 4px baseline unit. This "Optical Grid" ensures that all technical elements are perfectly aligned, mirroring the precision of a camera sensor's pixel array.

- **Grid:** A 12-column grid is used for marketing and comparison pages.
- **HUD Overlay:** For interactive video or image viewers, elements are anchored to the corners and mid-points of the viewport with a 32px safe-zone margin.
- **Rhythm:** Vertical spacing should be aggressive and mathematical, using multiples of 8px to separate distinct data clusters.

## Elevation & Depth
Depth in this design system is achieved through "Optical Layering" rather than traditional shadows.

- **Glassmorphism:** All overlay panels (menus, HUD controls) use a heavy backdrop blur (20px+) with a 15% opacity Graphite fill. This simulates the look of multi-coated lens elements.
- **Thin Borders:** Layers are separated by 1px solid borders in Graphite (#2C2C2C) or a 10% white stroke.
- **Z-Axis Hierarchy:** 
  - Level 0: Content/Media (Bottom).
  - Level 1: Primary UI Surface (Matte Black).
  - Level 2: HUD Overlays (Glassmorphic).
  - Level 3: Active Tooltips/Modals (Glassmorphic with Cyan border).

## Shapes
The shape language is "Precision Machined." Sharp corners are the default to maintain a professional, technical aesthetic. A very subtle **Soft (0.25rem)** roundedness is applied to buttons and interactive cards to suggest the ergonomic tactility of a camera body, but it should never reach a "pill" or "friendly" circularity. All data visualization bars and chart elements must remain perfectly sharp (0px radius) to emphasize mathematical accuracy.

## Components

### Buttons & Controls
Buttons use a "Ghost" style by default, with 1px Cyan or White borders. Hover states trigger a subtle Cyan outer glow (0px blur, 2px spread) to mimic an illuminated hardware button. Micro-interactions should be instantaneous (100ms) and snappy.

### Technical Spec Tables
Tables must use the `data-mono` type style. Rows should be separated by 1px Graphite lines. Alternate rows can use a 2% white tint for legibility in dense data sets. Key specs (e.g., "45MP", "8K/60p") should be highlighted in Pure White.

### Video Player & Overlays
The player is edge-to-edge. Tracking overlays (AF points) are rendered as thin Cyan squares. Histograms and waveform monitors use high-transparency glass backgrounds with no borders, appearing to float over the footage.

### Roadmap Charts
Interactive roadmaps use a horizontal timeline. Lenses or bodies are represented by vertical Graphite "blades" that expand on hover. Connections between ecosystem components are drawn with 1px Cyan lines.

### Comparison Grids
Comparison grids feature a "Sticky Header" for models. Differences between models should be highlighted with a subtle Amber left-border on the cell, indicating a technical variance.