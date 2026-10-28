---
version: alpha
name: Glossier
description: "Light monochrome interface measured from glossier.com: Apercu type, tonal surfaces and square corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#666666"
  surface-container-low: "#F5F5F5"
  surface-container: "#F0F0F0"
  surface-container-high: "#F1EFD8"
  surface-container-highest: "#E8E8E8"
  outline: "#0000000F"
  primary: "#FFFFFF"
  on-primary: "#000000"
  inverse-surface: "#464545"
  secondary: "#0600FF"
  tertiary: "#C8102E"
  error: "#9D2235"
  warning: "#F4C67B"
typography:
  headline-display:
    fontFamily: Apercu
    fontSize: 32px
    fontWeight: 500
    lineHeight: 0.61
  body-md:
    fontFamily: Apercu
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.23
  body-sm:
    fontFamily: Apercu
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.67
    letterSpacing: 0.003em
  label-md:
    fontFamily: Apercu
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
rounded:
  none: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 31.98px
  xl: 34px
  gutter: 9px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.none}"
    padding: 8px 16px
    height: 40px
  button-secondary:
    backgroundColor: "{colors.surface-container-highest}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.none}"
    padding: 8px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.none}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Glossier Design System

## Overview

Glossier describes itself as: “Glossier” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Apercu**. Headlines run large; body text is 16px. The surface language is flat. Corners are square.

Measured from [glossier.com](https://www.glossier.com/en-in) on October 21, 2026 at 1440×900 and 390×844 from 338 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **White (#FFFFFF):** Page background, seen 17 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 117 times. Token `on-surface`, CSS `--rc-active-color`.
- **Slate (#666666):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Snow (#F5F5F5):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Mist (#F0F0F0):** Cards and panels, seen 2 times. Token `surface-container`.
- **Pale Yellow (#F1EFD8):** Hover and pressed fills, seen 2 times. Token `surface-container-high`.
- **Mist (#E8E8E8):** Highest raised elements, seen 1 time. Token `surface-container-highest`.
- **Near Black 6% (#0000000F):** Borders and dividers, seen 1 time. Token `outline`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 29 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Graphite (#464545):** High-contrast fills, seen 8 times. Token `inverse-surface`.
- **Vivid Indigo (#0600FF):** Most used accent color, seen 7 times. Token `secondary`.
- **Vivid Red (#C8102E):** Most used accent color, seen 3 times. Token `tertiary`.
- **Dark Red (#9D2235):** Errors and destructive states, seen 2 times. Token `error`.
- **Light Orange (#F4C67B):** Warnings and highlights, seen 2 times. Token `warning`.

## Typography

**Apercu** carries the whole interface. Fallback stack: `Apercu, Gill Sans, sans-serif`. Other loaded fonts: Apercu Mono.

- **headline-display:** Apercu 32px at weight 500, line height 0.61. Page title (h1).
- **body-md:** Apercu 16px at weight 400, line height 1.23. Body text.
- **body-sm:** Apercu 12px at weight 400, line height 1.67, tracking 0.003em. Secondary and small text.
- **label-md:** Apercu 14px at weight 400, line height 1.4. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (75% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 31.98px, xl 34px.
- **Gaps:** 9px is the most common gap in flex and grid layouts.
- **Breakpoints:** 374px, 413px, 480px, 767px, 768px, 834px, 979px, 980px, 1024px, 1025px, 1280px, 1281px, 1400px, 1401px, 1921px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F5F5F5 → #F0F0F0 → #F1EFD8 → #E8E8E8) and #0000000F borders.

## Shapes

Corners are square. Measured radii, most used first:

- **none (0px):** measured.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Shop now”):** #FFFFFF fill, #000000 text, 14px/400, padding 8px 16px.
- **button-secondary (“Shop now”):** #E8E8E8 fill, #000000 text, 14px/400, padding 8px 16px.
- **button-ghost (“Previous Slide”):** transparent fill, #000000 text, 14px/400, padding 0px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5F5F5, #F0F0F0, #F1EFD8, #E8E8E8.
- Do keep text in 2 levels: #000000, #666666.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #FFFFFF.
- Do reuse the measured spacing steps (8px, 16px, 31.98px).
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Apercu.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.4s, 0.5s, 0.2s. Longer ambient animations run 1.5s, 1s.

- **Easing:** `ease-in-out`, `linear`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/glossier.com/), the free DESIGN.md generator.
