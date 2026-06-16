---
name: Kinematic Blueprint
colors:
  surface: '#f6fafe'
  surface-dim: '#d6dade'
  surface-bright: '#f6fafe'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f0f4f8'
  surface-container: '#eaeef2'
  surface-container-high: '#e4e9ed'
  surface-container-highest: '#dfe3e7'
  on-surface: '#171c1f'
  on-surface-variant: '#434653'
  inverse-surface: '#2c3134'
  inverse-on-surface: '#edf1f5'
  outline: '#737784'
  outline-variant: '#c3c6d5'
  surface-tint: '#2559bd'
  primary: '#00327d'
  on-primary: '#ffffff'
  primary-container: '#0047ab'
  on-primary-container: '#a5bdff'
  inverse-primary: '#b1c5ff'
  secondary: '#5f5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e4e2e1'
  on-secondary-container: '#656464'
  tertiary: '#6b1800'
  on-tertiary: '#ffffff'
  tertiary-container: '#932400'
  on-tertiary-container: '#ffa992'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2ff'
  primary-fixed-dim: '#b1c5ff'
  on-primary-fixed: '#001946'
  on-primary-fixed-variant: '#00419e'
  secondary-fixed: '#e4e2e1'
  secondary-fixed-dim: '#c8c6c6'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#474747'
  tertiary-fixed: '#ffdbd1'
  tertiary-fixed-dim: '#ffb5a0'
  on-tertiary-fixed: '#3b0900'
  on-tertiary-fixed-variant: '#872000'
  background: '#f6fafe'
  on-background: '#171c1f'
  surface-variant: '#dfe3e7'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  title-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
  caption-mono:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
spacing:
  base_grid: 4px
  gutter: 24px
  margin_desktop: 64px
  margin_mobile: 20px
  component_padding: 16px
---

## Brand & Style
This design system is built for the high-precision world of mechanical engineering. It prioritizes clarity, structural integrity, and technical documentation aesthetics. The visual language is inspired by CAD interfaces and physical blueprints, emphasizing the "work behind the work."

The style is **Technical & Structured**, utilizing a systematic approach to layout. UI elements are treated as components of a schematic. Key stylistic signatures include:
- **Graph Paper Underlay:** A subtle 20px grid pattern in the background to ground all elements.
- **Schematic Detailing:** Use of "L" shaped crop marks at the outer corners of major sections and containers.
- **Drafting Lines:** Borders are thin (1px) and mimic technical drawing strokes, utilizing dashed lines for secondary information or "hidden" states.
- **Precision Markers:** Use of coordinate markers (e.g., [B-4]) and measurement callouts to denote section transitions.

## Colors
The palette is derived from classic engineering documentation.
- **Engineering Blue (#0047AB):** Used for primary structural elements, active states, and key headers to evoke the classic blueprint feel.
- **Charcoal (#333333):** The standard for text and heavy structural outlines, providing high-contrast legibility.
- **Off-White (#F0F4F8):** The "Blueprint Paper" base, providing a softer, more professional canvas than pure white.
- **Safety Orange (#FF4500):** A high-visibility accent used sparingly for warnings, critical call-to-actions, and "Revision" markers.

## Typography
The typography system balances the readability of a modern sans-serif with the functional "data-output" look of a monospaced typeface.

- **Inter:** Used for all prose and primary navigation. It provides a robust, professional foundation that maintains legibility even in dense technical descriptions.
- **JetBrains Mono:** Reserved for technical metadata, coordinates, skill tags, and "spec" callouts. It should always appear in uppercase when used for labels to mimic architectural lettering.

## Layout & Spacing
The layout follows a **Fixed Grid** model based on a 12-column desktop system. 

- **Alignment:** All elements must snap to a 4px base increment. 
- **Section Dividers:** Instead of standard padding, sections are separated by horizontal 1px lines that extend to the edge of the grid, often capped with a coordinate marker like `[01 // SEC]`.
- **Breakpoints:**
  - **Desktop (1200px+):** 12 columns, 24px gutters, 64px margins.
  - **Tablet (768px):** 6 columns, 16px gutters, 32px margins.
  - **Mobile (375px):** 2 columns, 12px gutters, 20px margins.

## Elevation & Depth
In this design system, depth is communicated through **Tonal Layers** and **Lines** rather than shadows. 
- **Flat Depth:** Use 1px borders to define containment. Do not use ambient shadows.
- **Layering:** To suggest z-index, use "Drawing Overlays." An elevated element (like a modal) should have a thicker 2px border and a background color of pure `#FFFFFF` to distinguish it from the off-white background.
- **Hidden Lines:** Elements "behind" or secondary to the main view should use dashed border strokes (`stroke-dasharray: 4 4`).

## Shapes
The shape language is strictly **Sharp (0px)**. All containers, buttons, and input fields must have square corners. This reinforces the "machined" and "engineered" aesthetic. Circular elements are only permitted for functional icons or status indicators.

## Components
- **Project Cards:** Feature a 1px charcoal border. The top right corner includes a "Part No." (e.g., P-2024-01) in JetBrains Mono. Images within cards should have a subtle blue tint or overlay.
- **Skill Tags:** Styled like industrial labels. White background, 1px charcoal border, with a small "Safety Orange" dot on the left side to indicate "Active" status. Text is always uppercase Monospace.
- **Buttons:** Rectangular with no radius. Primary buttons use a solid Engineering Blue background with white text. Secondary buttons use a ghost style (transparent background, 1px border). Hover states should trigger a "Crosshair" cursor.
- **Section Headers:** Accompanied by a horizontal line that spans the full container width. To the left of the title, a coordinate marker in brackets (e.g., [A-1]) provides a "map" feel to the portfolio.
- **Technical Specs:** Used within project pages to list materials, software, or tolerances. These should be formatted in a table-like structure with dashed horizontal separators.