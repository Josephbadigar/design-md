---
version: alpha
name: Hootsuite
description: "Light interface measured from hootsuite.com: Montserrat type, blue accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#012B3A"
  on-background: "#012B3A"
  on-surface-strong: "#000000"
  surface-container-low: "#FFFFFFE6"
  surface-container: "#F2F4F5"
  overlay: "#FFFFFFD9"
  outline: "#BFCACE"
  outline-variant: "#012B3A33"
  primary: "#1F60C9"
  on-primary: "#FFFFFF"
  secondary: "#7E48EC"
  error: "#E03035"
typography:
  headline-display:
    fontFamily: Montserrat
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.11
  headline-lg:
    fontFamily: Montserrat
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.15
  headline-md:
    fontFamily: Montserrat
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.15
  body-md:
    fontFamily: Montserrat
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Montserrat
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Montserrat
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.6
  label-md:
    fontFamily: Montserrat
    fontSize: 15.5px
    fontWeight: 600
    lineHeight: 1.6
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Montserrat
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.71
  headline-display-mobile:
    fontFamily: Montserrat
    fontSize: 11px
    fontWeight: 600
    lineHeight: 1.11
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: -0.015em
rounded:
  sm: 2px
  md: 5.33px
  lg: 8px
spacing:
  xs: 2.02px
  sm: 8px
  md: 16px
  lg: 18px
  xl: 56px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.lg}"
    padding: 12px 16px
    height: 42px
  button-primary-hover:
    backgroundColor: "#759CDB"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "#0B2735"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px
    height: 69px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 20px 12px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    rounded: 0px
    padding: 1px 2px
  link:
    textColor: "{colors.on-surface}"
---

# Hootsuite Design System

## Overview

Hootsuite describes itself as: “Hootsuite is a social media management tool that brings scheduling, content creation, analytics, and social listening to one place.” The interface is light, built on **White (#FFFFFF)** with **Deep Cyan (#012B3A)** text, and **Blue (#1F60C9)** as the main accent.

Type is set in **Montserrat**. Headlines run large; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [hootsuite.com](https://www.hootsuite.com/) on October 29, 2026 at 1440×900 and 390×844 from 419 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`.
- **Deep Cyan (#012B3A):** Primary text and headings, seen 118 times. Token `on-surface`, CSS `--color-nocturn`.
- **Near Black (#000000):** Headings and emphasis, seen 2 times. Token `on-surface-strong`.
- **White 90% (#FFFFFFE6):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Mist (#F2F4F5):** Cards and panels, seen 2 times. Token `surface-container`.
- **White 85% (#FFFFFFD9):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Cool Silver (#BFCACE):** Borders and dividers, seen 5 times. Token `outline`, CSS `--color-nocturn25`.
- **Deep Cyan 20% (#012B3A33):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Blue (#1F60C9):** Primary buttons and calls to action, seen 5 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Violet (#7E48EC):** Accent, seen 3 times. Token `secondary`, CSS `--color-lumen-dark`.
- **Red (#E03035):** Errors and destructive states, seen 1 time. Token `error`, CSS `--color-saffron`.

## Typography

**Montserrat** carries the whole interface. Fallback stack: `Montserrat, -apple-system, BlinkMacSystemFont, sans-serif`. Other loaded fonts: slick.

- **headline-display:** Montserrat 40px at weight 600, line height 1.11 (11px on mobile). Page title (h1).
- **headline-lg:** Montserrat 36px at weight 700, line height 1.15 (24px on mobile). Section headings (h2).
- **headline-md:** Montserrat 28px at weight 700, line height 1.15. Sub-section headings.
- **body-md:** Montserrat 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Montserrat 14px at weight 400, line height 1.5. Secondary and small text.
- **label-lg:** Montserrat 16px at weight 500, line height 1.6. Large buttons and tabs.
- **label-md:** Montserrat 15.5px at weight 600, line height 1.6, tracking 0.02em. Buttons, navigation and labels.
- **label-sm:** Montserrat 14px at weight 500, line height 1.71. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (72% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2.02px, sm 8px, md 16px, lg 18px, xl 56px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 320px, 400px, 425px, 426px, 550px, 576px, 600px, 640px, 768px, 896px, 992px, 1200px, 1441px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#FFFFFFE6 → #F2F4F5) and hairline rings:

- `rgb(1, 43, 58) 0px 0px 0px 1px inset`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **lg (8px):** 68 elements.
- **sm (2px):** 8 elements.
- **md (5.33px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start your free trial”):** #1F60C9 fill, #FFFFFF text, 14px/700, 8px radius, padding 12px 16px.
- **button-primary-hover:** background #759CDB, text #FFFFFF on hover.
- **button-outline (“Request a demo”):** #FFFFFFD9 fill, #0B2735 text, 15.408px/600, 5.328px radius, padding 0px.
- **button-ghost (“Products”):** transparent fill, #012B3A text, 14px/600, padding 20px 12px.
- **input-field:** #FFFFFF fill, #000000 text, 13.3333px/400, padding 1px 2px, border 2px inset #767676.
- **link:** transparent fill, #012B3A text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FFFFFFE6, #F2F4F5.
- Do keep text in 2 levels: #012B3A, #000000.
- Do reserve #1F60C9 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 18px).
- Do use 8px corners on most elements; larger surfaces also use 2px and 5.33px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Montserrat.
- Don't use #1F60C9 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.1s, 0.2s. Longer ambient animations run 15s, 5.5s, 5.1s.

- **Easing:** `ease-out`, `ease`, `cubic-bezier(0.3, 0.9, 0.35, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/hootsuite.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
