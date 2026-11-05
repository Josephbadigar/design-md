---
version: alpha
name: Lovable
description: "Light monochrome interface measured from lovable.dev: Camera Plain Variable type, tonal surfaces and 8px corners."
colors:
  background: "#FCFBF8"
  surface: "#FCFBF8"
  on-surface: "#636363"
  on-background: "#636363"
  on-surface-strong: "#030303"
  on-surface-variant: "#1C1C1C"
  surface-container-low: "#FFFFFF"
  surface-container: "#F5F5F5"
  surface-container-high: "#F7F4ED"
  overlay: "#000000E0"
  overlay-strong: "#FFFFFFCC"
  outline: "#5F5F5D1A"
  outline-variant: "#ECEAE4"
  primary: "#1E1E1E"
  on-primary: "#FAFAFA"
  secondary: "#1F55F1"
typography:
  headline-display:
    fontFamily: Camera Plain Variable
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Camera Plain Variable
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-md:
    fontFamily: Camera Plain Variable
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Camera Plain Variable
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: Camera Plain Variable
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.67
  label-md:
    fontFamily: Camera Plain Variable
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-lg-mobile:
    fontFamily: Camera Plain Variable
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
rounded:
  sm: 6px
  md: 8px
  lg: 16px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 32px
  xl: 56px
  gutter: 8px
  section: 160px
  margin: 24px
  container: 1536px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 6px 10px
    height: 32px
  button-ghost:
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 4px 0px 4px 6px
  card:
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Lovable Design System

## Overview

Lovable describes itself as: “Describe what you want in plain language and Lovable builds it: full-stack apps, websites and internal tools. Start free.” The interface is light, built on **Snow (#FCFBF8)** with **Slate (#636363)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Camera Plain Variable**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [lovable.dev](https://lovable.dev/) on November 4, 2026 at 1440×900 and 390×844 from 370 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #82BCFF, #2483FF, #FF66F4, #FF3029.

- **Snow (#FCFBF8):** Page background. Token `background`.
- **Slate (#636363):** Primary text and headings, seen 82 times. Token `on-surface`.
- **Near Black (#030303):** Headings and emphasis, seen 13 times. Token `on-surface-strong`.
- **Charcoal (#1C1C1C):** Secondary text, seen 15 times. Token `on-surface-variant`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`.
- **Snow (#F5F5F5):** Cards and panels, seen 2 times. Token `surface-container`.
- **Warm Mist (#F7F4ED):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Near Black 88% (#000000E0):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **White 80% (#FFFFFFCC):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Slate 10% (#5F5F5D1A):** Borders and dividers, seen 2 times. Token `outline`.
- **Warm Mist (#ECEAE4):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Charcoal (#1E1E1E):** Primary buttons and calls to action, seen 19 times. Token `primary`.
- **Snow (#FAFAFA):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#1F55F1):** Accent, seen 2 times. Token `secondary`.

## Typography

**Camera Plain Variable** carries the whole interface. Fallback stack: `Camera Plain Variable, ui-sans-serif, system-ui, sans-serif`.

- **headline-display:** Camera Plain Variable 36px at weight 600, line height 1.1, tracking -0.04em. Page title (h1).
- **headline-lg:** Camera Plain Variable 18px at weight 400, line height 1.56 (14px on mobile). Section headings (h2).
- **body-md:** Camera Plain Variable 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Camera Plain Variable 15px at weight 400, line height 1.6. Lead paragraphs.
- **body-sm:** Camera Plain Variable 12px at weight 400, line height 1.67. Secondary and small text.
- **label-md:** Camera Plain Variable 16px at weight 400, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 47% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 16px, lg 32px, xl 56px.
- **Sections:** 160px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1536px.
- **Page margin:** 24px on each side of full-width sections.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#FFFFFF → #F5F5F5 → #F7F4ED):

- `oklch(0 0 0 / 0.25) 0px 0px 0px 1px inset`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.1 0 0 / 0.5) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`
- `oklch(0 0 0 / 0.16) 0px 0px 0px 1px inset`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(95, 95, 93, 0.12) 0px 0px 0px 1px, rgba(95, 95, 93, 0.1) 0px 4px 2px -3px, rgba(95, 95, 93, 0.15) 0px 5px 10px -4px`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 40 elements.
- **lg (16px):** 28 elements.
- **sm (6px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #000000E0 fill, #FAFAFA text, 14px/400, 8px radius, padding 6px 10px.
- **button-ghost (“Solutions”):** transparent fill, 15px/400, padding 4px 0px 4px 6px.
- **card:** transparent fill, 16px/400, 16px radius, padding 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(118, 118, 118, 0.1) 0px 0px 0px 1px, rgba(118, 118, 118, 0.07) 0px 1px 1px 0px, rgba(118, 118, 118, 0.05) 0px 2px 5px 0px, rgba(118, 118, 118, 0.1) 0px 4px 24px -8px, rgba(118, 118, 118, 0.08) 0px 4px 34px -5px`.
- **link:** transparent fill, #636363 text, padding 0px.

## Do's and Don'ts

- Do use #FCFBF8 for the page and lift surfaces in small steps: #FFFFFF, #F5F5F5, #F7F4ED.
- Do keep text in 3 levels: #636363, #030303, #1C1C1C.
- Do let contrast carry emphasis; primary actions use #1E1E1E on #FCFBF8.
- Do set headlines in Camera Plain Variable with tight tracking (-0.04em).
- Do reuse the measured spacing steps (6px, 16px, 32px).
- Do use 8px corners on most elements; larger surfaces also use 16px and 6px.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Camera Plain Variable.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.2s. Longer ambient animations run 1.2s.

- **Easing:** `cubic-bezier(0.215, 0.61, 0.355, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/lovable.dev/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
