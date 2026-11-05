---
version: alpha
name: Bootstrap
description: "Light interface measured from getbootstrap.com: Geist type with system-ui, violet accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#444B51"
  on-background: "#444B51"
  on-surface-strong: "#171A1D"
  on-surface-variant: "#5D666E"
  surface-container-low: "#F6F7F8"
  outline: "#171A1D1F"
  outline-variant: "#FFFFFF80"
  primary: "#7740FF"
  on-primary: "#FFFFFF"
  secondary: "#A87700"
typography:
  headline-display:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.025em
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Geist
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.2
  label-sm:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  code:
    fontFamily: Geist Mono
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.32
  headline-display-mobile:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.025em
rounded:
  sm: 8px
  md: 10px
  lg: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 24px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 8px 16px
    height: 46px
  button-outline:
    backgroundColor: "#FFF6D3"
    textColor: "{colors.secondary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 8px 16px
    height: 38px
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 6px 8px 6px 12px
    height: 35px
  button-ghost-hover:
    backgroundColor: "#F1F2F3"
    textColor: "{colors.on-surface-strong}"
  link:
    textColor: "{colors.on-surface}"
---

# Bootstrap Design System

## Overview

Bootstrap describes itself as: “Powerful, extensible, and feature-packed frontend toolkit. Build and customize with Sass, utilize prebuilt grid system and components, and bring projects to life with powerful JavaScript plugins.” The interface is light, built on **White (#FFFFFF)** with **Cool Graphite (#444B51)** text, and **Violet (#7740FF)** as the main accent.

Type is set in **Geist** and **system-ui**, with **Geist Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [getbootstrap.com](https://getbootstrap.com/) on November 4, 2026 at 1440×900 and 390×844 from 111 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`, CSS `--bs-primary-contrast`.
- **Cool Graphite (#444B51):** Primary text and headings, seen 40 times. Token `on-surface`.
- **Cool Charcoal (#171A1D):** Headings and emphasis, seen 3 times. Token `on-surface-strong`.
- **Cool Slate (#5D666E):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Snow (#F6F7F8):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Cool Charcoal 12% (#171A1D1F):** Borders and dividers, seen 1 time. Token `outline`.
- **White 50% (#FFFFFF80):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Violet (#7740FF):** Primary buttons and calls to action, seen 2 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Amber (#A87700):** Accent, seen 1 time. Token `secondary`.

## Typography

**Geist**, **system-ui** and **Geist Mono** (monospace) share the interface. Fallback stack: `Geist, -apple-system, BlinkMacSystemFont, Segoe UI`.

- **headline-display:** Geist 48px at weight 600, line height 1, tracking -0.025em (32px on mobile). Page title (h1).
- **body-md:** Geist 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Geist 20px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** system-ui 14px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Geist 16px at weight 500, line height 1.2. Buttons, navigation and labels.
- **label-sm:** Geist 14px at weight 400, line height 1.5. Small labels and badges.
- **code:** Geist Mono 15px at weight 400, line height 1.32. Code and technical values.

## Layout

Spacing does not follow a strict grid: 53% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 16px, lg 24px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.15) 0px 1px 2px 0px, rgba(255, 255, 255, 0.1) 0px 1px 0px 0px inset`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 32 elements.
- **lg (12px):** 8 elements.
- **md (10px):** 4 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Read the docs”):** #7740FF fill, #FFFFFF text, 16px/500, 12px radius, padding 8px 16px, border 1px solid #6C3BE3, shadow `rgba(0, 0, 0, 0.15) 0px 1px 2px 0px, rgba(255, 255, 255, 0.1) 0px 1px 0px 0px inset`.
- **button-outline (“Security updates for Bootstrap 3”):** #FFF6D3 fill, #A87700 text, 16px/400, 800px radius, padding 8px 16px, border 1px solid #FFFFFF80.
- **button-ghost (“Search docs… Ctrl K”):** #F6F7F8 fill, #5D666E text, 14px/400, 10px radius, padding 6px 8px 6px 12px, border 1px solid #171A1D1F.
- **button-ghost-hover:** background #F1F2F3, text #171A1D on hover.
- **link:** transparent fill, #444B51 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F6F7F8.
- Do keep text in 3 levels: #444B51, #171A1D, #5D666E.
- Do reserve #7740FF for primary actions and key highlights.
- Do set headlines in Geist with tight tracking (-0.025em).
- Do reuse the measured spacing steps (6px, 16px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 12px and 10px.
- Don't introduce new font families beyond Geist, system-ui and Geist Mono.
- Don't use #7740FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s.

- **Easing:** `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/getbootstrap.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
