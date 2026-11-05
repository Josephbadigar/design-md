---
version: alpha
name: Refero
description: "Light monochrome interface measured from refero.design: Title type with Base-Variable, tonal surfaces and 20px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#13151B"
  surface-container-low: "#F7F8FB"
  surface-container: "#DDDFEA"
  outline: "#EEF0F6"
  outline-variant: "#0111583D"
  primary: "#13151B"
  on-primary: "#FFFFFF"
  secondary: "#FA2413"
typography:
  headline-display:
    fontFamily: Title
    fontSize: 50px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Base-Variable
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.028em
  headline-md:
    fontFamily: Base-Variable
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: -0.022em
  label-lg:
    fontFamily: Base-Variable
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.02em
  label-md:
    fontFamily: Base-Variable
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: -0.02em
  label-sm:
    fontFamily: Base-Variable
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.015em
  headline-display-mobile:
    fontFamily: Title
    fontSize: 34px
    fontWeight: 400
    lineHeight: 1.18
    letterSpacing: -0.02em
rounded:
  xs: 8px
  sm: 12px
  md: 16px
  lg: 20px
  xl: 24px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 35px
  gutter: 8px
  container: 1600px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 0px
    height: 40px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.xs}"
    padding: 0px
    height: 48px
  button-secondary-hover:
    backgroundColor: "#2D313F"
  button-outline:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
    height: 42px
  input-field:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.primary}"
---

# Refero Design System

## Overview

Refero describes itself as: “The largest collection of UI/UX references and design inspiration for web and iOS. Explore tens of thousands of screenshots with advanced search capabilities” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Title** and **Base-Variable**. Headlines run large with tight negative tracking; body text is compact. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 20px.

Measured from [refero.design](https://refero.design/) on November 4, 2026 at 1440×900 and 390×844 from 307 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 80 times. Token `on-surface`.
- **Cool Charcoal (#13151B):** Secondary text, seen 13 times. Token `on-surface-variant`.
- **Snow (#F7F8FB):** Raised areas one step from the page, seen 14 times. Token `surface-container-low`.
- **Cool Mist (#DDDFEA):** Cards and panels, seen 1 time. Token `surface-container`.
- **Cool Mist (#EEF0F6):** Borders and dividers, seen 74 times. Token `outline`.
- **Deep Indigo 24% (#0111583D):** Secondary dividers, seen 4 times. Token `outline-variant`.
- **Cool Charcoal (#13151B):** Primary buttons and calls to action, seen 27 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Red (#FA2413):** Accent, seen 6 times. Token `secondary`.

## Typography

**Title** and **Base-Variable** share the interface. Fallback stack: `Title, -apple-system, BlinkMacSystemFont, Helvetica`.

- **headline-display:** Title 50px at weight 400, line height 1.2, tracking -0.02em (34px on mobile). Page title (h1).
- **headline-lg:** Base-Variable 32px at weight 500, line height 1.25, tracking -0.028em. Section headings (h2).
- **headline-md:** Base-Variable 20px at weight 500, line height 1.4, tracking -0.022em. Sub-section headings.
- **label-lg:** Base-Variable 16px at weight 500, line height 1.5, tracking -0.02em. Large buttons and tabs.
- **label-md:** Base-Variable 14px at weight 500, line height 1.43, tracking -0.02em. Buttons, navigation and labels.
- **label-sm:** Base-Variable 12px at weight 500, line height 1.33, tracking -0.015em. Small labels and badges.

## Layout

Spacing follows a 4px grid: 90% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 35px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1600px.
- **Breakpoints:** 768px, 980px, 1100px, 1293px, 1320px, 1500px, 1529px, 1600px, 1693px, 1747px, 1765px, 2048px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#F7F8FB → #DDDFEA):

- `rgba(12, 41, 126, 0.07) 0px 0px 0px 1px inset`
- `rgba(55, 80, 155, 0.04) 0px 0px 1px 0px inset`
- `rgba(1, 17, 88, 0.24) 0px 0px 0px 0.3px`

A few raised panels add a soft drop shadow: `rgba(12, 41, 126, 0.09) 0px 1px 3px 0px, rgba(12, 41, 126, 0.03) 0px 0px 1px 0.4px`.

## Shapes

Most elements use 20px corners. Measured radii, most used first:

- **lg (20px):** 300 elements.
- **xs (8px):** 108 elements.
- **sm (12px):** 60 elements.
- **xl (24px):** 36 elements.
- **md (16px):** 24 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“New research”):** #13151B fill, #FFFFFF text, 16px/500, 12px radius, padding 0px.
- **button-secondary (“Explore MCP”):** #000000 fill, #F7F8FB text, 16px/500, 8px radius, padding 0px.
- **button-secondary-hover:** background #2D313F, text #F7F8FB on hover.
- **button-outline (“Log In/Sign Up”):** transparent fill, #13151B text, 16px/500, 12px radius, padding 0px 12px, border 1px solid #0111583D, shadow `rgba(12, 41, 126, 0.09) 0px 1px 3px 0px, rgba(12, 41, 126, 0.03) 0px 0px 1px 0.4px`.
- **input-field (“Describe a task or ask a questio”):** transparent fill, #13151B text, 16px/500, padding 0px.
- **link:** transparent fill, #13151B text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F7F8FB, #DDDFEA.
- Do keep text in 2 levels: #000000, #13151B.
- Do let contrast carry emphasis; primary actions use #13151B on #FFFFFF.
- Do set headlines in Title with tight tracking (-0.02em).
- Do keep spacing on the 4px grid.
- Do use 20px corners on most elements; larger surfaces also use 8px, 12px and 24px.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Title and Base-Variable.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.3s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/refero.design/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
