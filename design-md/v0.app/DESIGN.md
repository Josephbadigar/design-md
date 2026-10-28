---
version: alpha
name: v0
description: "Dark monochrome interface measured from v0.app: GeistSans type with Inter, tonal surfaces and 4px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#EDEDED"
  on-background: "#EDEDED"
  on-surface-variant: "#A0A0A0"
  surface-container-low: "#0A0A0A"
  surface-container: "#121212"
  surface-container-high: "#1A1A1A"
  overlay: "#FFFFFF25"
  outline: "#FFFFFF25"
  outline-variant: "#2E2E2E"
  primary: "#EDEDED"
  on-primary: "#0A0A0A"
typography:
  headline-display:
    fontFamily: GeistSans
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.17
    letterSpacing: -0.06em
  headline-lg:
    fontFamily: GeistSans
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.04em
  headline-md:
    fontFamily: GeistSans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: -0.02em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  label-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1
  headline-lg-mobile:
    fontFamily: GeistSans
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.04em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
spacing:
  xs: 4px
  sm: 6px
  md: 12px
  lg: 24px
  xl: 64px
  gutter: 12px
  section: 80px
  margin: 24px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px 12px
    height: 32px
  button-primary-hover:
    backgroundColor: "{colors.on-surface-variant}"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    padding: 0px 12px
    height: 32px
  button-outline-hover:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px 12px
    height: 32px
  link:
    textColor: "{colors.on-surface-variant}"
---

# v0 Design System

## Overview

v0 describes itself as: “Your collaborative AI assistant to design, iterate, and scale full-stack applications for the web.” The interface is dark, built on **Near Black (#000000)** with **Mist (#EDEDED)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **GeistSans** and **Inter**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [v0.app](https://v0.app/) on October 21, 2026 at 1440×900 and 390×844 from 310 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Near Black (#000000):** Page background, seen 2 times. Token `background`.
- **Mist (#EDEDED):** Primary text and headings, seen 30 times. Token `on-surface`.
- **Gray (#A0A0A0):** Secondary text, seen 76 times. Token `on-surface-variant`.
- **Near Black (#0A0A0A):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Charcoal (#121212):** Cards and panels, seen 9 times. Token `surface-container`.
- **Charcoal (#1A1A1A):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **White 14% (#FFFFFF25):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **White 14% (#FFFFFF25):** Borders and dividers, seen 11 times. Token `outline`.
- **Graphite (#2E2E2E):** Secondary dividers, seen 6 times. Token `outline-variant`.
- **Mist (#EDEDED):** Primary buttons and calls to action, seen 45 times. Token `primary`.
- **Near Black (#0A0A0A):** Text and icons on primary. Token `on-primary`.

## Typography

**GeistSans** and **Inter** share the interface. Fallback stack: `GeistSans, GeistSans Fallback, ui-sans-serif, system-ui`. Other loaded fonts: GeistMono.

- **headline-display:** GeistSans 48px at weight 600, line height 1.17, tracking -0.06em. Page title (h1).
- **headline-lg:** GeistSans 32px at weight 600, line height 1.25, tracking -0.04em (24px on mobile). Section headings (h2).
- **headline-md:** GeistSans 20px at weight 600, line height 1.3, tracking -0.02em. Sub-section headings.
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Inter 14px at weight 400, line height 1.43. Secondary and small text.
- **label-md:** Inter 14px at weight 500, line height 1.43. Buttons, navigation and labels.
- **label-sm:** Inter 13px at weight 400, line height 1. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 64% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 12px, lg 24px, xl 64px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 540px, 600px, 601px, 640px, 768px, 960px, 961px, 1024px, 1280px, 1536px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#0A0A0A → #121212 → #1A1A1A) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklch(0.719 0.1515 250.7) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 52 elements.
- **md (6px):** 36 elements.
- **lg (8px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign Up”):** #EDEDED fill, #0A0A0A text, 14px/500, 8px radius, padding 0px 12px, border 1px solid #EDEDED.
- **button-primary-hover:** background #A0A0A0, text #0A0A0A on hover.
- **button-outline (“Contact Form”):** #121212 fill, #A0A0A0 text, 14px/500, 3.35544e+07px radius, padding 0px 12px, border 1px solid #FFFFFF25.
- **button-outline-hover:** background #1A1A1A, text #EDEDED on hover.
- **button-ghost (“Log In”):** #0A0A0A fill, #EDEDED text, 14px/500, 8px radius, padding 0px 12px, border 1px solid #27272A.
- **link:** transparent fill, #A0A0A0 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #0A0A0A, #121212, #1A1A1A.
- Do keep text in 2 levels: #EDEDED, #A0A0A0.
- Do let contrast carry emphasis; primary actions use #EDEDED on #000000.
- Do set headlines in GeistSans with tight tracking (-0.06em).
- Do reuse the measured spacing steps (6px, 12px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 6px and 8px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond GeistSans and Inter.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.6s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.34, 1.56, 0.64, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/v0.app/), the free DESIGN.md generator.
