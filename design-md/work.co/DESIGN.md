---
version: alpha
name: Work & Co
description: "Light interface measured from work.co: HelveticaNowDisplay type with adobe-garamond-pro, vivid red accents, tonal surfaces and 50px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  surface-container-low: "#DDDDDD"
  primary: "#FF3029"
  on-primary: "#000000"
  error: "#DB2223"
typography:
  headline-display:
    fontFamily: HelveticaNowDisplay
    fontSize: 56px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: HelveticaNowDisplay
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.02em
  body-md:
    fontFamily: adobe-garamond-pro
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  body-lg:
    fontFamily: adobe-garamond-pro
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.01em
  label-md:
    fontFamily: HelveticaNowDisplay
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.01em
  headline-display-mobile:
    fontFamily: HelveticaNowDisplay
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.19
    letterSpacing: -0.02em
rounded:
  md: 50px
spacing:
  md: 10px
  lg: 30px
  xl: 40px
components:
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    rounded: 0px
    padding: 191.23px 0px 0px 0px
  link:
    textColor: "{colors.error}"
---

# Work & Co Design System

## Overview

Work & Co describes itself as: “Work & Co is a digital product agency. We drive tangible business impact through strategy, design, and development of new platforms and experiences.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Red (#FF3029)** as the main accent.

Type is set in **HelveticaNowDisplay** and **adobe-garamond-pro**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 50px.

Measured from [work.co](https://work.co/) on November 4, 2026 at 1440×900 and 390×844 from 106 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 6 roles.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 36 times. Token `on-surface`.
- **Silver (#DDDDDD):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **Vivid Red (#FF3029):** Brand color in the logo. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Red (#DB2223):** Errors and destructive states, seen 6 times. Token `error`.

## Typography

**HelveticaNowDisplay** and **adobe-garamond-pro** share the interface. Fallback stack: `HelveticaNowDisplay, Helvetica Neue, Helvetica, Arial`.

- **headline-display:** HelveticaNowDisplay 56px at weight 500, line height 1, tracking -0.02em (32px on mobile). Page title (h1).
- **headline-lg:** HelveticaNowDisplay 36px at weight 500, line height 1.11, tracking -0.02em. Section headings (h2).
- **body-md:** adobe-garamond-pro 16px at weight 400, line height 1.15. Body text.
- **body-lg:** adobe-garamond-pro 20px at weight 400, line height 1.5, tracking -0.01em. Lead paragraphs.
- **label-md:** HelveticaNowDisplay 18px at weight 500, line height 1.5, tracking -0.01em. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 22% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** md 10px, lg 30px, xl 40px.
- **Breakpoints:** 400px, 425px, 426px, 550px, 600px, 749px, 750px, 896px, 950px, 1024px, 1099px, 1100px, 1799px, 1800px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#DDDDDD) and hairline rings:

- `rgb(255, 255, 255) 0px -1px 0px 0px inset, rgb(0, 0, 0) 0px -2px 0px 0px inset`
- `rgb(255, 255, 255) 0px -1px 0px 0px inset, rgb(219, 34, 35) 0px -2px 0px 0px inset`

## Shapes

Most elements use 50px corners. Measured radii, most used first:

- **md (50px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **card:** #DDDDDD fill, #000000 text, 0px/400, padding 191.23px 0px 0px 0px.
- **link:** transparent fill, #DB2223 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #DDDDDD.
- Do use #FF3029 as the brand accent: header, logo and key highlights.
- Do set headlines in HelveticaNowDisplay with tight tracking (-0.02em).
- Do reuse the measured spacing steps (10px, 30px).
- Do use 50px corners on most elements.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond HelveticaNowDisplay and adobe-garamond-pro.
- Don't use #FF3029 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.25s, 0.5s.

- **Easing:** `ease`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/work.co/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
