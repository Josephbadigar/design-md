---
version: alpha
name: iA
description: "Light interface measured from ia.net: iASansDay type, vivid cyan accents, tonal surfaces and 30px corners."
colors:
  background: "#F7F7F7"
  surface: "#F7F7F7"
  on-surface: "#222222"
  on-background: "#222222"
  on-surface-strong: "#000000"
  surface-container-low: "#FFFFFF"
  outline: "#DFDFDF"
  outline-variant: "#00B5FF"
  primary: "#00B5FF"
  on-primary: "#FFFFFF"
  inverse-surface: "#070707"
  secondary: "#00A9EE"
typography:
  headline-display:
    fontFamily: iASansDay
    fontSize: 58px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.015em
  body-md:
    fontFamily: iASansDay
    fontSize: 18.5px
    fontWeight: 400
    lineHeight: 1.65
  body-lg:
    fontFamily: iASansDay
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.65
  body-sm:
    fontFamily: iASansDay
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.65
  headline-display-mobile:
    fontFamily: iASansDay
    fontSize: 35px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.015em
rounded:
  sm: 3.1px
  md: 30px
  lg: 100px
spacing:
  sm: 5.75px
  md: 15.53px
  lg: 20.7px
  xl: 57.83px
  gutter: 15.53px
  container: 1024px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 10.47px 20.57px 8.23px 20.57px
    height: 46px
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 10.47px 20.57px 8.23px 20.57px
    height: 46px
  button-tertiary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "#F0F0F0"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 10.47px 20.57px 8.23px 20.57px
    height: 46px
  button-ghost:
    textColor: "{colors.inverse-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 10.47px 20.57px 8.23px 20.57px
  input-field:
    textColor: "{colors.on-surface-strong}"
    rounded: "{rounded.lg}"
    padding: 0px 0px 0px 20.7px
  link:
    textColor: "{colors.on-primary}"
---

# iA Design System

## Overview

iA describes itself as: “iA builds products for focus and flow.” The interface is light, built on **Snow (#F7F7F7)** with **Charcoal (#222222)** text, and **Vivid Cyan (#00B5FF)** as the main accent.

Type is set in **iASansDay**. Headlines run large with tight negative tracking; body text is 18.5px. The surface language is flat. Corners are mostly 30px.

Measured from [ia.net](https://ia.net/) on November 4, 2026 at 1440×900 and 390×844 from 108 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Snow (#F7F7F7):** Page background, seen 1 time. Token `background`.
- **Charcoal (#222222):** Primary text and headings, seen 55 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 13 times. Token `on-surface-strong`, CSS `--link-dark`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`, CSS `--link-light`.
- **Silver (#DFDFDF):** Borders and dividers, seen 4 times. Token `outline`.
- **Vivid Cyan (#00B5FF):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Cyan (#00B5FF):** Primary buttons and calls to action, seen 5 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Near Black (#070707):** High-contrast fills, seen 2 times. Token `inverse-surface`.
- **Vivid Cyan (#00A9EE):** Secondary buttons, seen 3 times. Token `secondary`.

## Typography

**iASansDay** carries the whole interface. Fallback stack: `iASansDay, system-ui, -apple-system, sans-serif`. Other loaded fonts: iASansNight.

- **headline-display:** iASansDay 58px at weight 700, line height 1.1, tracking -0.015em (35px on mobile). Page title (h1).
- **body-md:** iASansDay 18.5px at weight 400, line height 1.65. Body text.
- **body-lg:** iASansDay 22px at weight 400, line height 1.65. Lead paragraphs.
- **body-sm:** iASansDay 17px at weight 400, line height 1.65. Secondary and small text.

## Layout

Spacing does not follow a strict grid: 15% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 5.75px, md 15.53px, lg 20.7px, xl 57.83px.
- **Gaps:** 15.53px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1024px.
- **Breakpoints:** 416px, 512px, 560px, 640px, 768px, 1024px, 1040px, 1126px, 1140px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF) and #DFDFDF borders.

## Shapes

Most elements use 30px corners. Measured radii, most used first:

- **md (30px):** 28 elements.
- **sm (3.1px):** 16 elements.
- **lg (100px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Learn more”):** #00B5FF fill, #FFFFFF text, 18.7px/500, 30px radius, padding 10.47px 20.57px 8.23px 20.57px.
- **button-secondary (“Learn more”):** #00A9EE fill, #FFFFFF text, 18.7px/500, 30px radius, padding 10.47px 20.57px 8.23px 20.57px.
- **button-tertiary (“Learn more”):** #070707 fill, #F0F0F0 text, 18.7px/500, 30px radius, padding 10.47px 20.57px 8.23px 20.57px.
- **button-ghost (“Buy”):** transparent fill, #070707 text, 18.7px/500, 30px radius, padding 10.47px 20.57px 8.23px 20.57px, border 2px solid #070707.
- **input-field (“your@email.com”):** transparent fill, #000000 text, 20.7px/400, 100px radius, padding 0px 0px 0px 20.7px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #F7F7F7 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 2 levels: #222222, #000000.
- Do reserve #00B5FF for primary actions and key highlights.
- Do set headlines in iASansDay with tight tracking (-0.015em).
- Do reuse the measured spacing steps (5.75px, 15.53px, 20.7px).
- Do use 30px corners on most elements; larger surfaces also use 3.1px and 100px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond iASansDay.
- Don't use #00B5FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.3s.

- **Easing:** `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/ia.net/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
