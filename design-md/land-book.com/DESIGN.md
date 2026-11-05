---
version: alpha
name: Land-book
description: "Light interface measured from land-book.com: Inter type, dark teal accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#F7F6F5"
  surface: "#F7F6F5"
  on-surface: "#2B2A2A"
  on-background: "#2B2A2A"
  on-surface-strong: "#1D1C1C"
  on-surface-variant: "#4A4949"
  on-surface-muted: "#62615F"
  surface-container-low: "#F0EFED"
  surface-container: "#FFFFFF"
  overlay: "#FFFFFF80"
  outline: "#E1E0DD86"
  outline-variant: "#DDDCD980"
  primary: "#017C6E"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 24.5px
    fontWeight: 600
    lineHeight: 1.15
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Inter
    fontSize: 10.5px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
rounded:
  sm: 4.57px
  md: 13.71px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 36px
  gutter: 16px
  margin: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 7.61px 12px
    height: 32px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 7.61px 12px
    height: 32px
  button-ghost:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 7.61px 12px
    height: 32px
  button-ghost-hover:
    textColor: "{colors.on-surface}"
  input-field:
    backgroundColor: "{colors.overlay}"
    textColor: "#000000B3"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 7.61px 36px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 32px 16px 16px 16px
  link:
    textColor: "{colors.on-surface-strong}"
---

# Land-book Design System

## Overview

Land-book describes itself as: “Find the best hand-picked website design inspiration. We're a curated website design gallery for Creatives, updated daily.” The interface is light, built on **Snow (#F7F6F5)** with **Graphite (#2B2A2A)** text, and **Dark Teal (#017C6E)** as the main accent.

Type is set in **Inter**. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [land-book.com](https://land-book.com/) on November 4, 2026 at 1440×900 and 390×844 from 229 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Snow (#F7F6F5):** Page background, seen 2 times. Token `background`.
- **Graphite (#2B2A2A):** Primary text and headings, seen 50 times. Token `on-surface`.
- **Charcoal (#1D1C1C):** Headings and emphasis, seen 18 times. Token `on-surface-strong`.
- **Graphite (#4A4949):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Slate (#62615F):** Muted text and metadata, seen 14 times. Token `on-surface-muted`, CSS `--bs-gray-600`.
- **Mist (#F0EFED):** Raised areas one step from the page, seen 20 times. Token `surface-container-low`, CSS `--bs-gray-100`.
- **White (#FFFFFF):** Cards and panels, seen 3 times. Token `surface-container`, CSS `--bg-elevated`.
- **White 50% (#FFFFFF80):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Silver 53% (#E1E0DD86):** Borders and dividers, seen 6 times. Token `outline`.
- **Silver 50% (#DDDCD980):** Secondary dividers, seen 6 times. Token `outline-variant`, CSS `--border-muted`.
- **Dark Teal (#017C6E):** Primary buttons and calls to action, seen 5 times. Token `primary`, CSS `--bs-success`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, system-ui, -apple-system, Helvetica Neue`.

- **headline-display:** Inter 24.5px at weight 600, line height 1.15. Page title (h1).
- **body-md:** Inter 14px at weight 400, line height 1.5. Body text.
- **body-sm:** Inter 10.5px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Inter 14px at weight 500, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (83% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 32px, xl 36px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Page margin:** 16px on each side of full-width sections.
- **Breakpoints:** 575.98px, 576px, 767.98px, 768px, 991.98px, 992px, 1199.98px, 1200px, 1399.98px, 1400px, 1799.98px, 1800px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#F0EFED → #FFFFFF):

- `rgba(0, 0, 0, 0.08) 0px -1px 0px 0px inset, rgba(151, 145, 130, 0.25) 0px 0px 0px 1px inset`
- `rgba(255, 255, 255, 0.5) 0px 0px 4px 1px inset, rgba(55, 10, 255, 0.08) 0px 1px 2px 0px inset, rgba(255, 255, 255, 0.2) 0px 2px 5px 0px inset`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0.15) 0px -1px 0px 0px inset, rgba(0, 0, 0, 0.01) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.01) 0px 1px 3px 0px, rgba(19, 31, 51, 0.03) 0px 1px 1px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 124 elements.
- **md (13.71px):** 48 elements.
- **sm (4.57px):** 32 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #017C6E fill, #FFFFFF text, 14px/500, 800px radius, padding 7.61px 12px, shadow `rgba(0, 0, 0, 0.15) 0px -1px 0px 0px inset, rgba(0, 0, 0, 0.01) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.01) 0px 1px 3px 0px, rgba(19, 31, 51, 0.03) 0px 1px 1px 0px`.
- **button-outline (“Landing”):** #F0EFED fill, #1D1C1C text, 14px/500, 800px radius, padding 7.61px 12px.
- **button-ghost (“Get Pro”):** #FFFFFF fill, #1D1C1C text, 14px/500, 800px radius, padding 7.61px 12px, shadow `rgba(0, 0, 0, 0.08) 0px -1px 0px 0px inset, rgba(151, 145, 130, 0.25) 0px 0px 0px 1px inset`.
- **button-ghost-hover:** background #FFFFFF, text #2B2A2A on hover.
- **input-field:** #FFFFFF80 fill, #000000B3 text, 14px/400, 800px radius, padding 7.61px 36px, shadow `rgba(255, 255, 255, 0.5) 0px 0px 4px 1px inset, rgba(55, 10, 255, 0.08) 0px 1px 2px 0px inset, rgba(255, 255, 255, 0.2) 0px 2px 5px 0px inset`.
- **card:** #F0EFED fill, #017C6E text, 14px/400, 13.712px radius, padding 32px 16px 16px 16px.
- **link:** transparent fill, #1D1C1C text, padding 0px.

## Do's and Don'ts

- Do use #F7F6F5 for the page and lift surfaces in small steps: #F0EFED, #FFFFFF.
- Do keep text in 4 levels: #2B2A2A, #1D1C1C, #4A4949, #62615F.
- Do reserve #017C6E for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 32px).
- Do make buttons and chips fully rounded (9999px); most other elements use 13.71px corners.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Inter.
- Don't use #017C6E for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.08s, 0.005s, 0.2s, 0.3s. Longer ambient animations run 1s, 0.7s, 36s.

- **Easing:** `ease-out`, `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/land-book.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
