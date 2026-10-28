---
version: alpha
name: Node.js
description: "Dark interface measured from nodejs.org: OPEN SANS type, dark orange accents, tonal surfaces and 4px corners."
colors:
  background: "#0D121C"
  surface: "#0D121C"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#ECEFF4"
  on-surface-muted: "#D8DEE9"
  on-surface-subtle: "#6E7B83"
  surface-container-low: "#2C3437"
  overlay: "#417E381A"
  outline: "#2C3437"
  outline-variant: "#417E384D"
  primary: "#AE5F00"
  on-primary: "#FFFFFF"
  secondary: "#84BA64"
  tertiary: "#417E38"
  warning: "#EBCB8B"
typography:
  headline-display:
    fontFamily: OPEN SANS
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.02em
  body-md:
    fontFamily: OPEN SANS
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: OPEN SANS
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-sm:
    fontFamily: OPEN SANS
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: OPEN SANS
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: OPEN SANS
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  code:
    fontFamily: SFMono-Regular
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.38
  headline-display-mobile:
    fontFamily: OPEN SANS
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.02em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 18px
  gutter: 8px
  margin: 32px
  container: 768px
components:
  button-primary:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#B1BCC2"
    typography: "{typography.body-sm}"
    padding: 4px 10px 4px 4px
    height: 30px
  button-secondary:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#E9EDF0"
    rounded: "{rounded.sm}"
    padding: 4px 10px
    height: 24px
  button-secondary-hover:
    backgroundColor: "#556066"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "#E9EDF0"
    typography: "{typography.body-md}"
    rounded: 12px
    padding: 6px
    height: 42px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.secondary}"
---

# Node.js Design System

## Overview

Node.js describes itself as: “Node.js® is a free, open-source, cross-platform JavaScript runtime environment that lets developers create servers, web apps, command line tools and scripts.” The interface is dark, built on **Cool Charcoal (#0D121C)** with **White (#FFFFFF)** text, and **Dark Orange (#AE5F00)** as the main accent.

Type is set in **OPEN SANS**, with **SFMono-Regular** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [nodejs.org](https://nodejs.org/en) on October 21, 2026 at 1440×900 and 401×868 from 279 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #84BA64, #417E38.

- **Cool Charcoal (#0D121C):** Page background, seen 4 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 12 times. Token `on-surface`, CSS `--tw-ring-offset-color`.
- **Cool Mist (#ECEFF4):** Secondary text, seen 29 times. Token `on-surface-variant`.
- **Cool Mist (#D8DEE9):** Muted text and metadata, seen 15 times. Token `on-surface-muted`.
- **Cool Slate (#6E7B83):** Subtle text and placeholders, seen 11 times. Token `on-surface-subtle`.
- **Cool Graphite (#2C3437):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **Dark Green 10% (#417E381A):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Cool Graphite (#2C3437):** Borders and dividers, seen 12 times. Token `outline`.
- **Dark Green 30% (#417E384D):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Dark Orange (#AE5F00):** Brand color in the header, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Green (#84BA64):** Brand accent (CSS variable), seen 49 times. Token `secondary`, CSS `--color-brand-400`.
- **Dark Green (#417E38):** Brand accent (CSS variable), seen 12 times. Token `tertiary`, CSS `--color-brand-600`.
- **Light Amber (#EBCB8B):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**OPEN SANS** and **SFMono-Regular** (monospace) share the interface. Fallback stack: `OPEN_SANS, OPEN_SANS Fallback`. Other loaded fonts: OPEN_SANS, OPEN_SANS Fallback.

- **headline-display:** OPEN SANS 48px at weight 600, line height 1.33, tracking -0.02em (36px on mobile). Page title (h1).
- **body-md:** OPEN SANS 16px at weight 400, line height 1.5. Body text.
- **body-lg:** OPEN SANS 18px at weight 400, line height 1.56. Lead paragraphs.
- **body-sm:** OPEN SANS 14px at weight 400, line height 1.43. Secondary and small text.
- **label-md:** OPEN SANS 16px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** OPEN SANS 14px at weight 600, line height 1.43. Small labels and badges.
- **code:** SFMono-Regular 14px at weight 400, line height 1.38. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (81% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 18px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 768px.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 896px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#2C3437):

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(44, 52, 55) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.20991 -0.003893 -0.0339065 / 0.05) 0px 1px 2px 0px`.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 96 elements.
- **lg (8px):** 40 elements.
- **md (6px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“v24.22.0 Latest LTS”):** #2C3437 fill, #B1BCC2 text, 14px/500, 3.35544e+07px radius, padding 4px 10px 4px 4px, border 1px solid #066291.
- **button-secondary (“Copy to clipboard”):** #2C3437 fill, #E9EDF0 text, 12px/500, 4px radius, padding 4px 10px.
- **button-secondary-hover:** background #556066, text #E9EDF0 on hover.
- **button-outline (“Start typing... ⌘ K”):** #0D121C fill, #E9EDF0 text, 16px/400, 12px radius, padding 6px, border 1px solid #2C3437.
- **button-ghost (“×”):** transparent fill, #FFFFFF text, 18px/400, padding 0px.
- **link:** transparent fill, #84BA64 text, padding 0px.

## Do's and Don'ts

- Do use #0D121C for the page and lift surfaces in small steps: #2C3437.
- Do keep text in 4 levels: #FFFFFF, #ECEFF4, #D8DEE9, #6E7B83.
- Do use #AE5F00 as the brand accent: header, logo and key highlights.
- Do set headlines in OPEN SANS with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 18px).
- Do use 4px corners on most elements; larger surfaces also use 8px and 6px.
- Don't use #6E7B83 for body text; it reaches 4.3:1 on #0D121C. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond OPEN SANS and SFMono-Regular.
- Don't use #AE5F00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/nodejs.org/), the free DESIGN.md generator.
