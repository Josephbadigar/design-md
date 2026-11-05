---
version: alpha
name: GIMP
description: "Light interface measured from gimp.org: League Gothic type with Questrial, blue accents, flat surfaces and 3px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#555555"
  on-background: "#555555"
  on-surface-variant: "#777777"
  overlay: "#ECF0F11F"
  outline: "#AAAAAA"
  outline-variant: "#EEEEEE"
  primary: "#497BAD"
  on-primary: "#000000"
  inverse-surface: "#0E2426"
  secondary: "#F57900"
typography:
  headline-display:
    fontFamily: League Gothic
    fontSize: 211px
    fontWeight: 400
    lineHeight: 1.3
  headline-lg:
    fontFamily: Questrial
    fontSize: 29px
    fontWeight: 400
    lineHeight: 1.5
  headline-md:
    fontFamily: Questrial
    fontSize: 27px
    fontWeight: 400
    lineHeight: 1.5
  body-md:
    fontFamily: Open Sans
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Questrial
    fontSize: 23px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Open Sans
    fontSize: 14.5px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: Open Sans
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Open Sans
    fontSize: 13.5px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: 0.214em
  headline-display-mobile:
    fontFamily: League Gothic
    fontSize: 160px
    fontWeight: 400
    lineHeight: 1.3
  headline-md-mobile:
    fontFamily: Questrial
    fontSize: 22.5px
    fontWeight: 400
    lineHeight: 1.5
rounded:
  sm: 3px
  md: 4.03px
spacing:
  sm: 5.76px
  md: 9.6px
  lg: 19.2px
  xl: 38.4px
  gutter: 9.6px
  section: 76.8px
components:
  input-field:
    backgroundColor: "{colors.overlay}"
    textColor: "#ECF0F1"
    typography: "{typography.caption}"
    rounded: 0px
    padding: 0px 0px 0px 21.5px
  link:
    textColor: "{colors.primary}"
---

# GIMP Design System

## Overview

The interface is light, built on **White (#FFFFFF)** with **Slate (#555555)** text, and **Blue (#497BAD)** as the main accent.

Type is set in **League Gothic** and **Questrial**. Headlines run large; body text is 19px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 3px.

Measured from [gimp.org](https://www.gimp.org/) on November 4, 2026 at 1440×900 and 390×844 from 150 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`.
- **Slate (#555555):** Primary text and headings, seen 6 times. Token `on-surface`.
- **Slate (#777777):** Secondary text, seen 12 times. Token `on-surface-variant`.
- **Mist 12% (#ECF0F11F):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Gray (#AAAAAA):** Borders and dividers, seen 4 times. Token `outline`.
- **Mist (#EEEEEE):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Blue (#497BAD):** Most used accent color, seen 26 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Deep Cyan (#0E2426):** High-contrast fills, seen 5 times. Token `inverse-surface`.
- **Vivid Orange (#F57900):** Accent in text, fills and borders, seen 14 times. Token `secondary`.

## Typography

**League Gothic**, **Questrial** and **Open Sans** share the interface. Fallback stack: `League Gothic, sans`. Other loaded fonts: Ostrich Sans Rounded, CC.

- **headline-display:** League Gothic 211px at weight 400, line height 1.3, uppercase (160px on mobile). Page title (h1).
- **headline-lg:** Questrial 29px at weight 400, line height 1.5. Section headings (h2).
- **headline-md:** Questrial 27px at weight 400, line height 1.5 (22.5px on mobile). Sub-section headings.
- **body-md:** Open Sans 19px at weight 400, line height 1.5. Body text.
- **body-lg:** Questrial 23px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** Open Sans 14.5px at weight 400, line height 1.5. Secondary and small text.
- **caption:** Open Sans 13px at weight 400, line height 1.5. Captions and fine print.
- **label-md:** Open Sans 13.5px at weight 600, line height 1.5, tracking 0.214em. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 0% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 5.76px, md 9.6px, lg 19.2px, xl 38.4px.
- **Sections:** 76.8px vertical padding between major sections.
- **Gaps:** 9.6px is the most common gap in flex and grid layouts.
- **Breakpoints:** 1367px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgb(0, 0, 0) 0px 7px 15px -5px inset`

## Shapes

Most elements use 3px corners. Measured radii, most used first:

- **sm (3px):** 12 elements.
- **md (4.03px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **input-field (“Search GIMP.org”):** #ECF0F11F fill, #ECF0F1 text, 13.44px/400, padding 0px 0px 0px 21.5px, border 1px solid #E1EFFF1A.
- **link:** transparent fill, #497BAD text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #555555, #777777.
- Do reserve #497BAD for primary actions and key highlights.
- Do reuse the measured spacing steps (5.76px, 9.6px, 19.2px).
- Do use 3px corners on most elements; larger surfaces also use 4.03px.
- Don't use #777777 for body text; it reaches 4.48:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond League Gothic, Questrial and Open Sans.
- Don't use #497BAD for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.5s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/gimp.org/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
