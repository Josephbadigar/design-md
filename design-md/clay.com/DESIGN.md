---
version: alpha
name: Clay
description: "Dark interface measured from clay.com: Roobertvf type, vivid yellow accents, flat surfaces and 12px corners."
colors:
  background: "#035D44"
  surface: "#035D44"
  on-surface: "#FEFDFB"
  on-background: "#FEFDFB"
  on-surface-variant: "#000000"
  on-surface-muted: "#001433"
  on-surface-subtle: "#1B1A18"
  outline: "#7B797426"
  primary: "#CBD810"
  on-primary: "#000000"
  inverse-surface: "#F4F3F0"
  secondary: "#46022F"
  warning: "#808000"
typography:
  headline-display:
    fontFamily: Roobertvf
    fontSize: 88px
    fontWeight: 575
    lineHeight: 1
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Roobertvf
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.04em
  headline-md:
    fontFamily: Roobertvf
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Roobertvf
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.3
  title-lg:
    fontFamily: Roobertvf
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.3
  body-md:
    fontFamily: Roobertvf
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Roobertvf
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.01em
  body-sm:
    fontFamily: Roobertvf
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.1
  caption:
    fontFamily: Roobertvf
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.3
  label-lg:
    fontFamily: Roobertvf
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: Roobertvf
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Roobertvf
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: 0.12em
  headline-display-mobile:
    fontFamily: Roobertvf
    fontSize: 41.5px
    fontWeight: 575
    lineHeight: 1
    letterSpacing: -0.04em
  headline-md-mobile:
    fontFamily: Roobertvf
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Roobertvf
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.04em
rounded:
  sm: 12px
  md: 18px
  lg: 24px
spacing:
  xs: 2.08px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 64px
  gutter: 16px
  section: 64px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 9px 18px
    height: 47px
  button-secondary:
    backgroundColor: "#FFFFFF"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 9px 18px
    height: 47px
  button-tertiary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "#FFFFFF"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
    height: 39px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    rounded: 0px
    padding: 6.4px
  input-field:
    backgroundColor: "#FFFFFF"
    textColor: "{colors.on-surface-subtle}"
    typography: "{typography.body-md}"
    rounded: 20px
    padding: 11.2px 16px 16px 16px
  card:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 16px 20px
  link:
    textColor: "#55534E"
---

# Clay Design System

## Overview

Clay describes itself as: “Infrastructure to get any data, run agentic workflows, and launch GTM plays.” The interface is dark, built on **Deep Teal (#035D44)** with **Snow (#FEFDFB)** text, and **Vivid Yellow (#CBD810)** as the main accent.

Type is set in **Roobertvf**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 12px.

Measured from [clay.com](https://www.clay.com/) on November 5, 2026 at 1440×900 and 390×844 from 374 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Deep Teal (#035D44):** Page background, seen 1 time. Token `background`.
- **Snow (#FEFDFB):** Primary text and headings, seen 2 times. Token `on-surface`, CSS `--loam---web-library_terra-swatches---oat--oat-100`.
- **Near Black (#000000):** Secondary text, seen 46 times. Token `on-surface-variant`.
- **Deep Blue (#001433):** Muted text and metadata, seen 5 times. Token `on-surface-muted`, CSS `--loam---web-library_terra-swatches---blueberry--blueberry-500`.
- **Charcoal (#1B1A18):** Subtle text and placeholders, seen 6 times. Token `on-surface-subtle`.
- **Warm Slate 15% (#7B797426):** Borders and dividers, seen 26 times. Token `outline`.
- **Vivid Yellow (#CBD810):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Mist (#F4F3F0):** High-contrast fills, seen 38 times. Token `inverse-surface`.
- **Deep Pink (#46022F):** Accent in text, fills and borders, seen 5 times. Token `secondary`.
- **Dark Yellow (#808000):** Warnings and highlights, seen 2 times. Token `warning`.

## Typography

**Roobertvf** carries the whole interface. Fallback stack: `Roobertvf, Arial, sans-serif`. Other loaded fonts: Roobert, Space Mono, Phosphor.

- **headline-display:** Roobertvf 88px at weight 575, line height 1, tracking -0.04em (41.5px on mobile). Page title (h1).
- **headline-lg:** Roobertvf 48px at weight 500, line height 1, tracking -0.04em (32px on mobile). Section headings (h2).
- **headline-md:** Roobertvf 44px at weight 500, line height 1.1, tracking -0.02em (32px on mobile). Sub-section headings.
- **headline-sm:** Roobertvf 24px at weight 400, line height 1.3. Card and feature titles.
- **title-lg:** Roobertvf 20px at weight 400, line height 1.3. Small titles.
- **body-md:** Roobertvf 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Roobertvf 18px at weight 500, line height 1.5, tracking -0.01em. Lead paragraphs.
- **body-sm:** Roobertvf 14px at weight 400, line height 1.1. Secondary and small text.
- **caption:** Roobertvf 12px at weight 400, line height 1.3. Captions and fine print.
- **label-lg:** Roobertvf 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** Roobertvf 14px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Roobertvf 12px at weight 600, line height 1.1, tracking 0.12em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (73% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2.08px, sm 8px, md 16px, lg 20px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 767px, 768px, 991px, 1280px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgba(255, 255, 255, 0.05) 0px 0px 0px 1px inset`

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **sm (12px):** 216 elements.
- **md (18px):** 132 elements.
- **lg (24px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get a demo”):** #CBD810 fill, #000000 text, 18px/500, 12px radius, padding 9px 18px.
- **button-secondary (“Start free trial”):** #FFFFFF fill, #000000 text, 18px/500, 12px radius, padding 9px 18px.
- **button-tertiary (“Start free trial”):** #000000 fill, #FFFFFF text, 13.92px/500, 12px radius, padding 8px 16px.
- **button-ghost (“⌘ K”):** transparent fill, #000000 text, 12.8px/400, padding 6.4px.
- **input-field (“Find companies with 30+ sales re”):** #FFFFFF fill, #1B1A18 text, 16px/400, 20px radius, padding 11.2px 16px 16px 16px.
- **card:** #FEFDFB fill, #000000 text, 16px/400, 18px radius, padding 16px 20px, border 1px solid #FFFFFF.
- **link:** transparent fill, #55534E text, padding 0px.

## Do's and Don'ts

- Do use #035D44 for the page.
- Do keep text in 4 levels: #FEFDFB, #000000, #001433, #1B1A18.
- Do reserve #CBD810 for primary actions and key highlights.
- Do set headlines in Roobertvf with tight tracking (-0.04em).
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do use 12px corners on most elements; larger surfaces also use 18px and 24px.
- Don't use #000000 for body text; it reaches 2.65:1 on #035D44. Keep it for large text or metadata.
- Don't use #001433 for body text; it reaches 2.31:1 on #035D44. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond Roobertvf.
- Don't use #CBD810 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.1s, 0.3s, 0.15s, 0.25s.

- **Easing:** `ease-out`, `cubic-bezier(0.075, 0.82, 0.165, 1)`, `linear`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/clay.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
