---
version: alpha
name: v0
description: "Light monochrome interface measured from v0.app: GeistSans type with Inter, tonal surfaces and 4px corners."
colors:
  background: "#FAFAFA"
  surface: "#FAFAFA"
  on-surface: "#171717"
  on-background: "#171717"
  on-surface-variant: "#4D4D4D"
  surface-container-low: "#FFFFFF"
  surface-container: "#F2F2F2"
  overlay: "#00000014"
  outline: "#00000014"
  outline-variant: "#EBEBEB"
  primary: "#171717"
  on-primary: "#FFFFFF"
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
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    padding: 0px 12px
    height: 32px
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

v0 describes itself as: “Your collaborative AI assistant to design, iterate, and scale full-stack applications for the web.” The interface is light, built on **Snow (#FAFAFA)** with **Charcoal (#171717)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **GeistSans** and **Inter**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [v0.app](https://v0.app/) on October 29, 2026 at 1440×900 and 390×844 from 310 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Snow (#FAFAFA):** Page background, seen 2 times. Token `background`.
- **Charcoal (#171717):** Primary text and headings, seen 30 times. Token `on-surface`.
- **Slate (#4D4D4D):** Secondary text, seen 76 times. Token `on-surface-variant`, CSS `--color-v0-gray-900`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 12 times. Token `surface-container-low`.
- **Mist (#F2F2F2):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--color-v0-gray-100`.
- **Near Black 8% (#00000014):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **Near Black 8% (#00000014):** Borders and dividers, seen 11 times. Token `outline`.
- **Mist (#EBEBEB):** Secondary dividers, seen 6 times. Token `outline-variant`.
- **Charcoal (#171717):** Primary buttons and calls to action, seen 44 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

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

The design avoids drop shadows. Layers are separated by tonal surface steps (#FFFFFF → #F2F2F2) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklch(0.573 0.2146 258.2) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 52 elements.
- **md (6px):** 36 elements.
- **lg (8px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign Up”):** #171717 fill, #FFFFFF text, 14px/500, 8px radius, padding 0px 12px, border 1px solid #171717.
- **button-outline (“Contact Form”):** #FFFFFF fill, #4D4D4D text, 14px/500, 3.35544e+07px radius, padding 0px 12px, border 1px solid #00000014.
- **button-ghost (“Log In”):** #FFFFFF fill, #171717 text, 14px/500, 8px radius, padding 0px 12px, border 1px solid #E4E4E7.
- **link:** transparent fill, #4D4D4D text, padding 0px.

## Do's and Don'ts

- Do use #FAFAFA for the page and lift surfaces in small steps: #FFFFFF, #F2F2F2.
- Do keep text in 2 levels: #171717, #4D4D4D.
- Do let contrast carry emphasis; primary actions use #171717 on #FAFAFA.
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

Generated by [Sitepeel](https://sitepeel.dev/design-md/v0.app/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
