---
version: alpha
name: Rust
description: "Dark interface measured from rust-lang.org: Alfa Slab One type with Fira Sans, dark teal accents, flat surfaces and 4px corners."
colors:
  background: "#0B7261"
  surface: "#0B7261"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#2A3439"
  outline: "#A72145"
  outline-variant: "#2E2459"
  primary: "#0B7261"
  on-primary: "#FFFFFF"
  secondary: "#4299BF"
  warning: "#FFC832"
typography:
  headline-display:
    fontFamily: Alfa Slab One
    fontSize: 96px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: 0.01em
  headline-lg:
    fontFamily: Fira Sans
    fontSize: 36px
    fontWeight: 800
    lineHeight: 1.25
    letterSpacing: 0.028em
  headline-md:
    fontFamily: Fira Sans
    fontSize: 27px
    fontWeight: 600
    lineHeight: 1.3
  body-md:
    fontFamily: Fira Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.6
  body-lg:
    fontFamily: Fira Sans
    fontSize: 21.5px
    fontWeight: 600
    lineHeight: 1.6
  body-sm:
    fontFamily: Fira Sans
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.15
  label-md:
    fontFamily: Fira Sans
    fontSize: 14.5px
    fontWeight: 600
    lineHeight: 1.6
    letterSpacing: 0.083em
  headline-display-mobile:
    fontFamily: Alfa Slab One
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: 0.025em
  headline-lg-mobile:
    fontFamily: Fira Sans
    fontSize: 30px
    fontWeight: 800
    lineHeight: 1.25
    letterSpacing: 0.033em
  headline-md-mobile:
    fontFamily: Fira Sans
    fontSize: 22.5px
    fontWeight: 600
    lineHeight: 1.3
rounded:
  md: 4px
spacing:
  xs: 2px
  sm: 6px
  md: 12px
  lg: 30px
  xl: 60px
  section: 60px
  container: 1152px
components:
  button-outline:
    backgroundColor: "{colors.outline}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px 30px
    height: 41px
  button-secondary:
    backgroundColor: "{colors.warning}"
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-md}"
    rounded: "{rounded.md}"
    padding: 20px
    height: 85px
  input-field:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 2px 6px
  link:
    textColor: "{colors.warning}"
---

# Rust Design System

## Overview

Rust describes itself as: “A language empowering everyone to build reliable and efficient software.” The interface is dark, built on **Dark Teal (#0B7261)** with **Near Black (#000000)** text, and **Dark Teal (#0B7261)** as the main accent.

Type is set in **Alfa Slab One** and **Fira Sans**. Headlines run large; body text is 18px. The surface language is flat. Corners are mostly 4px.

Measured from [rust-lang.org](https://rust-lang.org/) on October 21, 2026 at 1440×900 and 390×844 from 115 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Dark Teal (#0B7261):** Page background, seen 1 time. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 12 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 37 times. Token `on-surface-strong`.
- **Cool Graphite (#2A3439):** Secondary text, seen 13 times. Token `on-surface-variant`.
- **Pink (#A72145):** Borders and dividers, seen 4 times. Token `outline`.
- **Dark Indigo (#2E2459):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Dark Teal (#0B7261):** Brand color on large areas, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Cyan (#4299BF):** Accent, seen 1 time. Token `secondary`.
- **Vivid Amber (#FFC832):** Warnings and highlights, seen 16 times. Token `warning`.

## Typography

**Alfa Slab One** and **Fira Sans** share the interface. Fallback stack: `Alfa Slab One, serif`.

- **headline-display:** Alfa Slab One 96px at weight 300, line height 1.2, tracking 0.01em (40px on mobile). Page title (h1).
- **headline-lg:** Fira Sans 36px at weight 800, line height 1.25, tracking 0.028em (30px on mobile). Section headings (h2).
- **headline-md:** Fira Sans 27px at weight 600, line height 1.3 (22.5px on mobile). Sub-section headings.
- **body-md:** Fira Sans 18px at weight 400, line height 1.6. Body text.
- **body-lg:** Fira Sans 21.5px at weight 600, line height 1.6. Lead paragraphs.
- **body-sm:** Fira Sans 15px at weight 400, line height 1.15. Secondary and small text.
- **label-md:** Fira Sans 14.5px at weight 600, line height 1.6, tracking 0.083em. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 47% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 12px, lg 30px, xl 60px.
- **Sections:** 60px vertical padding between major sections.
- **Container:** content is capped at 1152px.
- **Breakpoints:** 545px, 550px, 769px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #A72145 borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 40 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“BUILDING TOOLS”):** #A72145 fill, #FFFFFF text, 14.4px/600, 4px radius, padding 8px 30px, border 1px solid #A72145.
- **button-secondary (“GET STARTED”):** #FFC832 fill, #000000 text, 27px/600, 4px radius, padding 20px, border 1px solid #FFC832.
- **input-field:** #FFFFFF fill, #2A3439 text, 15px/400, padding 2px 6px, border 1px solid #2A3439.
- **link:** transparent fill, #FFC832 text, padding 0px.

## Do's and Don'ts

- Do use #0B7261 for the page.
- Do keep text in 3 levels: #000000, #FFFFFF, #2A3439.
- Do use #0B7261 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (6px, 12px, 30px).
- Do use 4px corners on most elements.
- Don't use #000000 for body text; it reaches 3.6:1 on #0B7261. Keep it for large text or metadata.
- Don't use #2A3439 for body text; it reaches 2.2:1 on #0B7261. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Alfa Slab One and Fira Sans.
- Don't use #0B7261 for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/rust-lang.org/), the free DESIGN.md generator.
