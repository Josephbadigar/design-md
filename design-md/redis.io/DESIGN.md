---
version: alpha
name: Redis
description: "Dark interface measured from redis.io: primaryFont type with Space Grotesk, vivid lime accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#091A23"
  surface: "#091A23"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#B9C2C6"
  on-surface-muted: "#8A99A0"
  surface-container-low: "#0D212C"
  surface-container: "#351D22"
  outline: "#2D4754"
  outline-variant: "#163341"
  primary: "#DCFF1E"
  on-primary: "#091A23"
  inverse-surface: "#5C707A"
  secondary: "#8A221C"
  tertiary: "#D1281E"
  error: "#FF4438"
typography:
  headline-display:
    fontFamily: primaryFont
    fontSize: 100px
    fontWeight: 400
    lineHeight: 0.85
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.2
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.45
  body-md:
    fontFamily: Times New Roman
    fontSize: 16px
    fontWeight: 400
  body-sm:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  code:
    fontFamily: Space Mono
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0.107em
  headline-display-mobile:
    fontFamily: primaryFont
    fontSize: 80px
    fontWeight: 400
    lineHeight: 0.85
    letterSpacing: -0.013em
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.2
rounded:
  sm: 4px
  md: 10px
  lg: 200px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 10px
  lg: 32px
  xl: 40px
  gutter: 8px
  section: 72px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: 5px
    padding: 13px
    height: 49px
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 1px
    height: 35px
  button-outline-hover:
    backgroundColor: "{colors.secondary}"
  button-secondary:
    backgroundColor: "{colors.outline-variant}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 5px
    padding: 12px 40px
    height: 47px
  button-secondary-hover:
    backgroundColor: "{colors.outline}"
  button-ghost:
    textColor: "#000000"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#D9D9D9"
    rounded: 5px
    padding: 0px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 32px
  link:
    textColor: "{colors.on-surface}"
---

# Redis Design System

## Overview

Redis describes itself as: “Developers love Redis. Unlock the full potential of the Redis database with Redis Enterprise and start building blazing fast apps.” The interface is dark, built on **Deep Blue (#091A23)** with **White (#FFFFFF)** text, and **Vivid Lime (#DCFF1E)** as the main accent.

Type is set in **primaryFont** and **Space Grotesk**, with **Space Mono** for code. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [redis.io](https://redis.io/) on October 21, 2026 at 1440×900 and 390×844 from 294 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #091A23.

- **Deep Blue (#091A23):** Page background, seen 13 times. Token `background`, CSS `--midnight`.
- **White (#FFFFFF):** Primary text and headings, seen 27 times. Token `on-surface`, CSS `--base-white`.
- **Cool Silver (#B9C2C6):** Secondary text, seen 25 times. Token `on-surface-variant`.
- **Cyan (#8A99A0):** Muted text and metadata, seen 12 times. Token `on-surface-muted`, CSS `--dusk-50`.
- **Deep Blue (#0D212C):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **Deep Red (#351D22):** Cards and panels, seen 4 times. Token `surface-container`, CSS `--hyper-10`.
- **Dark Blue (#2D4754):** Borders and dividers, seen 16 times. Token `outline`.
- **Deep Cyan (#163341):** Secondary dividers, seen 13 times. Token `outline-variant`.
- **Vivid Lime (#DCFF1E):** Primary buttons and calls to action, seen 12 times. Token `primary`, CSS `--yellow`.
- **Deep Blue (#091A23):** Text and icons on primary. Token `on-primary`.
- **Blue (#5C707A):** High-contrast fills, seen 10 times. Token `inverse-surface`.
- **Dark Red (#8A221C):** Brand accent (CSS variable), seen 12 times. Token `secondary`.
- **Red (#D1281E):** Brand accent (CSS variable), seen 12 times. Token `tertiary`.
- **Vivid Red (#FF4438):** Errors and destructive states, seen 13 times. Token `error`, CSS `--hyper-05`.

## Typography

**primaryFont**, **Space Grotesk**, **Times New Roman** and **Space Mono** (monospace) share the interface. Fallback stack: `primaryFont, primaryFont Fallback, sans-serif`. Other loaded fonts: Space Grotesk Fallback, Graphik.

- **headline-display:** primaryFont 100px at weight 400, line height 0.85, tracking -0.01em, uppercase (80px on mobile). Page title (h1).
- **headline-lg:** Space Grotesk 32px at weight 500, line height 1.2 (24px on mobile). Section headings (h2).
- **headline-md:** Space Grotesk 20px at weight 500, line height 1.45. Sub-section headings.
- **body-md:** Times New Roman 16px at weight 400. Body text.
- **body-sm:** Space Grotesk 14px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Space Grotesk 14px at weight 500, line height 1.5. Buttons, navigation and labels.
- **code:** Space Mono 14px at weight 500, line height 1.2, tracking 0.107em. Code and technical values.

## Layout

Spacing does not follow a strict grid: 66% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 10px, lg 32px, xl 40px.
- **Sections:** 72px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 767px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#0D212C → #351D22) and #2D4754 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (4px):** 84 elements.
- **full (9999px):** 60 elements.
- **md (10px):** 20 elements.
- **lg (200px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Accept”):** #DCFF1E fill, #091A23 text, 16px/400, 5px radius, padding 13px, border 1px solid #5C707A.
- **button-outline (“Redis Iris”):** #351D22 fill, #FFFFFF text, 14px/500, 200px radius, padding 1px.
- **button-outline-hover:** background #8A221C, text #FFFFFF on hover.
- **button-secondary (“Get a demo”):** #163341 fill, #FFFFFF text, 14px/500, 5px radius, padding 12px 40px, border 1px solid #2D4754.
- **button-secondary-hover:** background #2D4754, text #FFFFFF on hover.
- **button-ghost (“Read the report”):** transparent fill, #000000 text, 14px/500, padding 0px.
- **input-field (“Switch language”):** #0D212C fill, #D9D9D9 text, 12px/400, 5px radius, padding 0px.
- **card:** #0D212C fill, #FFFFFF text, 16px/400, 10px radius, padding 32px, border 1px solid #163341.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #091A23 for the page and lift surfaces in small steps: #0D212C, #351D22.
- Do keep text in 3 levels: #FFFFFF, #B9C2C6, #8A99A0.
- Do reserve #DCFF1E for primary actions and key highlights.
- Do set headlines in primaryFont with tight tracking (-0.01em).
- Do reuse the measured spacing steps (8px, 10px, 32px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond primaryFont, Space Grotesk, Times New Roman and Space Mono.
- Don't use #DCFF1E for large backgrounds or body text.
- Don't make interface transitions slower than 0.00001s.

## Motion

Interface transitions are quick: 1e-05s.

- **Easing:** `ease`, `ease-in-out`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/redis.io/), the free DESIGN.md generator.
