---
version: alpha
name: Stack Overflow
description: "Light interface measured from stackoverflow.com: system-ui type, blue accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0C0D0E"
  on-background: "#0C0D0E"
  on-surface-variant: "#3B4045"
  on-surface-muted: "#636B74"
  surface-container-low: "#EDF5FD"
  surface-container: "#F1F2F3"
  surface-container-high: "#E3E6E8"
  outline: "#F1F2F3"
  outline-variant: "#BABFC5"
  primary: "#1B75D0"
  on-primary: "#FFFFFF"
  secondary: "#E7700D"
typography:
  headline-display:
    fontFamily: system-ui
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.3
  body-md:
    fontFamily: system-ui
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.31
  body-lg:
    fontFamily: system-ui
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.31
  body-sm:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.31
  caption:
    fontFamily: system-ui
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.31
  label-lg:
    fontFamily: system-ui
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.3
  label-md:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.31
  label-sm:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 700
    lineHeight: 1.85
rounded:
  sm: 4px
  md: 6px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 56px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 8px 10.4px
    height: 33px
  button-primary-hover:
    backgroundColor: "#155CA2"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 4px
    height: 24px
  button-outline-hover:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
  button-ghost:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px
    height: 33px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 7.8px 9.1px 7.8px 32px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Stack Overflow Design System

## Overview

The interface is light, built on **White (#FFFFFF)** with **Charcoal (#0C0D0E)** text, and **Blue (#1B75D0)** as the main accent.

Type is set in **system-ui**. Headlines run large; body text is 17px. The surface language is flat. Corners are mostly 4px.

Measured from [stackoverflow.com](https://stackoverflow.com/questions) on November 4, 2026 at 1440×900 and 390×844 from 377 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 17 times. Token `background`.
- **Charcoal (#0C0D0E):** Primary text and headings, seen 21 times. Token `on-surface`.
- **Cool Graphite (#3B4045):** Secondary text, seen 59 times. Token `on-surface-variant`.
- **Cool Slate (#636B74):** Muted text and metadata, seen 44 times. Token `on-surface-muted`.
- **Cool Snow (#EDF5FD):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Mist (#F1F2F3):** Cards and panels, seen 32 times. Token `surface-container`.
- **Mist (#E3E6E8):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Mist (#F1F2F3):** Borders and dividers, seen 31 times. Token `outline`.
- **Cool Silver (#BABFC5):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Blue (#1B75D0):** Primary buttons and calls to action, seen 19 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Orange (#E7700D):** Accent, seen 1 time. Token `secondary`.

## Typography

**system-ui** carries the whole interface. Fallback stack: `-apple-system, BlinkMacSystemFont, Segoe UI Adjusted, Segoe UI`.

- **headline-display:** system-ui 15px at weight 400, line height 1.3. Page title (h1).
- **body-md:** system-ui 17px at weight 400, line height 1.31. Body text.
- **body-lg:** system-ui 19px at weight 400, line height 1.31. Lead paragraphs.
- **body-sm:** system-ui 13px at weight 400, line height 1.31. Secondary and small text.
- **caption:** system-ui 11px at weight 400, line height 1.31. Captions and fine print.
- **label-lg:** system-ui 15px at weight 700, line height 1.3. Large buttons and tabs.
- **label-md:** system-ui 13px at weight 700, line height 1.31. Buttons, navigation and labels.
- **label-sm:** system-ui 12px at weight 700, line height 1.85. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 52% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 56px.
- **Breakpoints:** 607px, 640px, 640.1px, 771px, 816px, 816.1px, 947px, 980px, 980.1px, 1100px, 1111px, 1264px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#EDF5FD → #F1F2F3 → #E3E6E8) and #F1F2F3 borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 212 elements.
- **md (6px):** 26 elements.
- **full (9999px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #1B75D0 fill, #FFFFFF text, 13px/400, 6px radius, padding 8px 10.4px.
- **button-primary-hover:** background #155CA2, text #FFFFFF on hover.
- **button-outline (“python”):** #F1F2F3 fill, #3B4045 text, 12px/700, 4px radius, padding 0px 4px, border 1px solid #F1F2F3.
- **button-outline-hover:** background #E3E6E8, text #0C0D0E on hover.
- **button-ghost (“Questions”):** #F1F2F3 fill, #0C0D0E text, 13px/700, 6px 0px 0px 6px radius, padding 8px.
- **input-field (“Search…”):** #FFFFFF fill, #3B4045 text, 13px/400, 6px radius, padding 7.8px 9.1px 7.8px 32px, border 1px solid #BABFC5.
- **card:** #FFFFFF fill, #1B75D0 text, 13px/400, 4px radius, padding 0px.
- **link:** transparent fill, #3B4045 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #EDF5FD, #F1F2F3, #E3E6E8.
- Do keep text in 3 levels: #0C0D0E, #3B4045, #636B74.
- Do reserve #1B75D0 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 6px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond system-ui.
- Don't use #1B75D0 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s.

- **Easing:** `cubic-bezier(0.165, 0.84, 0.44, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/stackoverflow.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
