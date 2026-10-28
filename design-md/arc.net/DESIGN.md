---
version: alpha
name: Arc
description: "Light interface measured from arc.net: Marlin Soft SQ type with Marlin, vivid indigo accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFCEC"
  surface: "#FFFCEC"
  on-surface: "#000000"
  on-background: "#000000"
  surface-container-low: "#FFFFFF"
  overlay: "#000000D9"
  primary: "#3139FB"
  on-primary: "#FFFFFF"
  secondary: "#2702C2"
  tertiary: "#FF5060"
  error: "#FF9999"
typography:
  headline-display:
    fontFamily: Marlin Soft SQ
    fontSize: 45.5px
    fontWeight: 700
    lineHeight: 0.93
    letterSpacing: -0.04em
  body-md:
    fontFamily: Marlin
    fontSize: 16px
    fontWeight: 400
  body-lg:
    fontFamily: Marlin Soft SQ
    fontSize: 40px
    fontWeight: 700
    lineHeight: 0.97
    letterSpacing: -0.04em
  label-lg:
    fontFamily: Marlin Soft SQ
    fontSize: 16px
    fontWeight: 700
  label-md:
    fontFamily: Marlin Soft SQ
    fontSize: 14px
    fontWeight: 500
    letterSpacing: -0.02em
  label-sm:
    fontFamily: InterVariable
    fontSize: 12px
    fontWeight: 600
    letterSpacing: 0.033em
  headline-display-mobile:
    fontFamily: Marlin Soft SQ
    fontSize: 32px
    fontWeight: 700
    lineHeight: 0.97
    letterSpacing: -0.05em
rounded:
  sm: 4px
  md: 8px
  lg: 10px
  xl: 22px
spacing:
  xs: 3px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 37px
  gutter: 12px
components:
  button-primary:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.xl}"
    padding: 8px 22px 8px 8px
    height: 76px
  button-primary-hover:
    backgroundColor: "#000000A6"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.secondary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 8px 0px
    height: 45px
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 8px 0px
    height: 45px
  link:
    textColor: "{colors.on-primary}"
---

# Arc Design System

## Overview

Arc describes itself as: “Experience a calmer, more personal internet in this browser designed for you. Let go of the clicks, the clutter, the distractions with the Arc browser.” The interface is light, built on **Pale Amber (#FFFCEC)** with **Near Black (#000000)** text, and **Vivid Indigo (#3139FB)** as the main accent.

Type is set in **Marlin Soft SQ** and **Marlin**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [arc.net](https://arc.net/) on October 21, 2026 at 1440×900 and 390×844 from 165 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **Pale Amber (#FFFCEC):** Page background, seen 1 time. Token `background`, CSS `--colors-brandOffwhite`.
- **Near Black (#000000):** Primary text and headings, seen 1 time. Token `on-surface`, CSS `--colors-highContrast`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`, CSS `--colors-lowContrast`.
- **Near Black 85% (#000000D9):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Vivid Indigo (#3139FB):** Brand color on large areas, seen 56 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Indigo (#2702C2):** Secondary buttons, seen 41 times. Token `secondary`, CSS `--colors-students-dark_blue`.
- **Red (#FF5060):** Brand color in the logo, seen 15 times. Token `tertiary`.
- **Light Red (#FF9999):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**Marlin Soft SQ**, **Marlin** and **InterVariable** share the interface. Fallback stack: `Marlin Soft SQ, -apple-system, BlinkMacSystemFont, Segoe UI`. Other loaded fonts: Inter, ABC Favorit Mono, ABC Oracle, Exposure VAR.

- **headline-display:** Marlin Soft SQ 45.5px at weight 700, line height 0.93, tracking -0.04em (32px on mobile). Page title (h1).
- **body-md:** Marlin 16px at weight 400. Body text.
- **body-lg:** Marlin Soft SQ 40px at weight 700, line height 0.97, tracking -0.04em. Lead paragraphs.
- **label-lg:** Marlin Soft SQ 16px at weight 700. Large buttons and tabs.
- **label-md:** Marlin Soft SQ 14px at weight 500, tracking -0.02em. Buttons, navigation and labels.
- **label-sm:** InterVariable 12px at weight 600, tracking 0.033em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (79% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 3px, sm 8px, md 12px, lg 24px, xl 37px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 580px, 600px, 650px, 750px, 800px, 1000px, 1075px, 1100px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 5px 5px 0px`
- `rgba(0, 0, 0, 0.25) 0px 2px 8px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 20 elements.
- **lg (10px):** 12 elements.
- **sm (4px):** 4 elements.
- **xl (22px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try Dia”):** #000000D9 fill, #FFFFFF text, 24px/400, 22px radius, padding 8px 22px 8px 8px, shadow `rgba(0, 0, 0, 0.25) 0px 2px 8px 0px`.
- **button-primary-hover:** background #000000A6, text #FFFFFF on hover.
- **button-outline (“Download Arc for Windows”):** #FFFFFF fill, #2702C2 text, 14px/600, 10px radius, padding 8px 0px, shadow `rgba(0, 0, 0, 0.1) 0px 5px 5px 0px`.
- **button-secondary (“Download Arc for Mac”):** #2702C2 fill, #FFFFFF text, 14px/600, 10px radius, padding 8px 0px, shadow `rgba(0, 0, 0, 0.1) 0px 5px 5px 0px`.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFCEC for the page and lift surfaces in small steps: #FFFFFF.
- Do use #3139FB as the brand accent: header, logo and key highlights.
- Do set headlines in Marlin Soft SQ with tight tracking (-0.04em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 10px, 4px and 22px.
- Don't introduce new font families beyond Marlin Soft SQ, Marlin and InterVariable.
- Don't use #3139FB for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s.

- **Easing:** `ease`, `ease-out`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/arc.net/), the free DESIGN.md generator.
