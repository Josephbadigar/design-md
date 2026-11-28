---
version: alpha
name: Pinterest
description: "Light interface measured from pinterest.com: Pin Sans type, vivid red accents, tonal surfaces and 16px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#62625B"
  surface-container-low: "#E5E5E0"
  primary: "#E60023"
  on-primary: "#FFFFFF"
  secondary: "#DD0E0E"
typography:
  headline-display:
    fontFamily: Pin Sans
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.018em
  body-md:
    fontFamily: Pin Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: Pin Sans
    fontSize: 14px
    fontWeight: 400
  label-md:
    fontFamily: Pin Sans
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.4
  label-sm:
    fontFamily: Pin Sans
    fontSize: 12px
    fontWeight: 400
rounded:
  sm: 8px
  md: 12px
  lg: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  xl: 44px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 8px 16px
    height: 48px
  button-secondary:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 8px 16px
    height: 48px
  button-ghost:
    textColor: "#211922"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 8px 16px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Pinterest Design System

## Overview

Pinterest describes itself as: “Discover recipes, home ideas, style inspiration and other ideas to try.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Red (#E60023)** as the main accent.

Type is set in **Pin Sans**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 16px.

Measured from [pinterest.com](https://www.pinterest.com/) on November 27, 2026 at 1440×900 and 390×844 from 146 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **White (#FFFFFF):** Page background, seen 3 times. Token `background`, CSS `--comp-iconbutton-color-icon-gray-enabled-selected`.
- **Near Black (#000000):** Primary text and headings, seen 15 times. Token `on-surface`, CSS `--comp-bannerslim-color-text-body-warning-expanded`.
- **Warm Slate (#62625B):** Secondary text, seen 4 times. Token `on-surface-variant`, CSS `--sema-color-icon-subtle`.
- **Mist (#E5E5E0):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Vivid Red (#E60023):** Primary buttons and calls to action, seen 18 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Red (#DD0E0E):** Accent, seen 4 times. Token `secondary`.

## Typography

**Pin Sans** carries the whole interface. Fallback stack: `Pin Sans, -apple-system, BlinkMacSystemFont, Segoe UI`.

- **headline-display:** Pin Sans 28px at weight 700, line height 1.1, tracking -0.018em. Page title (h1).
- **body-md:** Pin Sans 16px at weight 400, line height 1.4. Body text.
- **body-sm:** Pin Sans 14px at weight 400. Secondary and small text.
- **label-md:** Pin Sans 16px at weight 700, line height 1.4. Buttons, navigation and labels.
- **label-sm:** Pin Sans 12px at weight 400. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (87% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, xl 44px.
- **Breakpoints:** 576px, 768px, 1312px, 1440px, 1680px, 2048px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#E5E5E0).

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **lg (16px):** 64 elements.
- **sm (8px):** 16 elements.
- **md (12px):** 12 elements.
- **full (9999px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Log in”):** #E60023 fill, #FFFFFF text, 12px/400, 16px radius, padding 8px 16px.
- **button-secondary (“Sign up”):** #E5E5E0 fill, #000000 text, 12px/400, 16px radius, padding 8px 16px.
- **button-ghost (“Explore”):** transparent fill, #211922 text, 12px/400, 16px radius, padding 8px 16px.
- **input-field (“Search for easy dinners, fashion”):** transparent fill, #000000 text, 16px/400, padding 0px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #E5E5E0.
- Do keep text in 2 levels: #000000, #62625B.
- Do reserve #E60023 for primary actions and key highlights.
- Do set headlines in Pin Sans with tight tracking (-0.018em).
- Do reuse the measured spacing steps (8px, 16px).
- Do use 16px corners on most elements; larger surfaces also use 8px and 12px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Pin Sans.
- Don't use #E60023 for large backgrounds or body text.
- Don't make interface transitions slower than 0.085s.

## Motion

Interface transitions are quick: 0.085s.

- **Easing:** `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/pinterest.com/), the free DESIGN.md generator (engine 2026.10.29+f0c146f7cdfd).
