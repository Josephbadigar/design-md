---
version: alpha
name: Chase
description: "Light interface measured from chase.com: Open Sans type, dark blue accents, flat surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#101820"
  on-background: "#101820"
  on-surface-variant: "#414042"
  on-surface-muted: "#717171"
  outline: "#C6C4C4"
  primary: "#005EB8"
  on-primary: "#FFFFFF"
  secondary: "#0060F0"
  tertiary: "#002F6C"
  success: "#128842"
typography:
  display-hero:
    fontFamily: Open Sans
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.33
  headline-display:
    fontFamily: Open Sans
    fontSize: 32px
    fontWeight: 700
    lineHeight: 0.75
  headline-lg:
    fontFamily: Open Sans
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1
  body-md:
    fontFamily: Open Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
  body-sm:
    fontFamily: Open Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: Open Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Open Sans
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1.33
  display-hero-mobile:
    fontFamily: Open Sans
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.29
rounded:
  md: 4px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 10px
  lg: 24px
components:
  button-primary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 5px
    padding: 1px 6px
    height: 36px
  button-primary-hover:
    backgroundColor: "#0A4386"
  button-secondary:
    backgroundColor: "{colors.success}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 6px 16px
    height: 36px
  button-secondary-hover:
    backgroundColor: "#0E6D35"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 1px 6px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  input-field:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 14px 0px 4.2px 0px
  link:
    textColor: "{colors.secondary}"
---

# Chase Design System

## Overview

Chase describes itself as: “Chase online; credit cards, mortgages, commercial banking, auto loans, investing & retirement planning, checking and business banking.” The interface is light, built on **White (#FFFFFF)** with **Cool Charcoal (#101820)** text, and **Dark Blue (#005EB8)** as the main accent.

Type is set in **Open Sans**. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [chase.com](https://www.chase.com/) on November 4, 2026 at 1440×900 and 390×844 from 319 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`, CSS `--light-background-text-color`.
- **Cool Charcoal (#101820):** Primary text and headings, seen 28 times. Token `on-surface`, CSS `--dropdown-item-color`.
- **Graphite (#414042):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Slate (#717171):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Silver (#C6C4C4):** Borders and dividers, seen 1 time. Token `outline`.
- **Dark Blue (#005EB8):** Brand color on large areas, seen 11 times. Token `primary`, CSS `--flip-card-link-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0060F0):** Secondary buttons, seen 12 times. Token `secondary`, CSS `--mds-cta-tertiary-color`.
- **Deep Blue (#002F6C):** Accent (CSS variable). Token `tertiary`.
- **Dark Green (#128842):** Success and positive states, seen 4 times. Token `success`, CSS `--green-cta-secondary-color`.

## Typography

**Open Sans** carries the whole interface. Fallback stack: `Open Sans, Helvetica Neue, helvetica, arial`.

- **display-hero:** Open Sans 36px at weight 600, line height 1.33 (28px on mobile). Oversized hero statements.
- **headline-display:** Open Sans 32px at weight 700, line height 0.75. Page title (h1).
- **headline-lg:** Open Sans 24px at weight 700, line height 1. Section headings (h2).
- **body-md:** Open Sans 14px at weight 400, line height 1.71. Body text.
- **body-sm:** Open Sans 12px at weight 400, line height 1.33. Secondary and small text.
- **label-md:** Open Sans 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Open Sans 12px at weight 600, line height 1.33. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 52% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 10px, lg 24px.
- **Breakpoints:** 0px, 575px, 576px, 767px, 768px, 992px, 1200px, 1440px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgb(140, 142, 144) 0px -1px 0px 0px inset`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 36 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign in”):** #0060F0 fill, #FFFFFF text, 16px/600, 5px radius, padding 1px 6px.
- **button-primary-hover:** background #0A4386, text #FFFFFF on hover.
- **button-secondary (“Learn more”):** #128842 fill, #FFFFFF text, 16px/400, 4px radius, padding 6px 16px.
- **button-secondary-hover:** background #0E6D35, text #FFFFFF on hover.
- **button-outline (“Passwordless sign in”):** #FFFFFF fill, #005EB8 text, 16px/600, 4px radius, padding 1px 6px, border 1px solid #005EB8.
- **button-ghost (“Customer service”):** transparent fill, #101820 text, 16px/400, padding 0px.
- **input-field:** transparent fill, #414042 text, 14px/400, padding 14px 0px 4.2px 0px, shadow `rgb(140, 142, 144) 0px -1px 0px 0px inset`.
- **link:** transparent fill, #0060F0 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #101820, #414042, #717171.
- Do use #005EB8 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (6px, 10px, 24px).
- Do use 4px corners on most elements.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond Open Sans.
- Don't use #005EB8 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s.

- **Easing:** `cubic-bezier(0, 0.4, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/chase.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
