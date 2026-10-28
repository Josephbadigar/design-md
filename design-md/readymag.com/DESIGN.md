---
version: alpha
name: Readymag
description: "Dark interface measured from readymag.com: system-ui type with custom 157067, vivid orange accents, flat surfaces and 200px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#444444"
  primary: "#EC520B"
  on-primary: "#FFFFFF"
  inverse-surface: "#F4F4F4F5"
  secondary: "#C8020A"
  tertiary: "#FF5900"
typography:
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  body-lg:
    fontFamily: custom 157067
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.03
    letterSpacing: -0.03em
  body-sm:
    fontFamily: custom 190030
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.2
  label-md:
    fontFamily: custom 190030
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.5
rounded:
  sm: 40px
  md: 45px
  lg: 200px
spacing:
  base: 8px
  sm: 8px
  md: 16px
  lg: 24px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.lg}"
    padding: 0px 24px
    height: 40px
  button-secondary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px 24px
    height: 40px
  button-secondary-hover:
    textColor: "{colors.primary}"
  button-tertiary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
    height: 28px
  input-field:
    textColor: "{colors.background}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px 20px
  card:
    backgroundColor: "{colors.background}"
    textColor: "#282828"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
---

# Readymag Design System

## Overview

Readymag describes itself as: “Make the web more like you” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Vivid Orange (#EC520B)** as the main accent.

Type is set in **system-ui** and **custom 157067**. Headlines run large; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 200px.

Measured from [readymag.com](https://readymag.com/) on October 21, 2026 at 1440×900 and 390×844 from 66 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Near Black (#000000):** Page background, seen 4 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 1 time. Token `on-surface`.
- **Graphite (#444444):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Vivid Orange (#EC520B):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Snow 96% (#F4F4F4F5):** High-contrast fills, seen 6 times. Token `inverse-surface`.
- **Red (#C8020A):** Brand color in logos and imagery, seen 18 times. Token `secondary`.
- **Vivid Orange (#FF5900):** Brand color on large areas, seen 11 times. Token `tertiary`.

## Typography

**system-ui**, **custom 157067** and **custom 190030** share the interface. Fallback stack: `-apple-system, system-ui, BlinkMacSystemFont, Segoe UI`. Other loaded fonts: custom_37866, custom_157067, custom_190030.

- **body-md:** system-ui 16px at weight 400, line height 1. Body text.
- **body-lg:** custom 157067 30px at weight 400, line height 1.03, tracking -0.03em. Lead paragraphs.
- **body-sm:** custom 190030 14px at weight 400, line height 1.2. Secondary and small text.
- **label-md:** custom 190030 12px at weight 500, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing follows a 8px grid: 93% of measured gaps and paddings are multiples of 8px.

- **Scale:** sm 8px, md 16px, lg 24px.
- **Breakpoints:** 478px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgb(0, 0, 0) 0px 0px 0px 0px inset`

## Shapes

Most elements use 200px corners. Measured radii, most used first:

- **lg (200px):** 28 elements.
- **sm (40px):** 12 elements.
- **md (45px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #EC520B fill, #FFFFFF text, 0px/400, 200px radius, padding 0px 24px.
- **button-secondary (“Pricing”):** #F4F4F4F5 fill, #000000 text, 16px/400, 200px radius, padding 0px 24px.
- **button-secondary-hover:** background #F4F4F4F5, text #EC520B on hover.
- **button-tertiary (“Allow all”):** #FFFFFF fill, #444444 text, 12px/500, 40px radius, padding 8px 16px.
- **input-field (“Password”):** transparent fill, #000000 text, 14px/400, padding 0px 20px.
- **card:** #000000 fill, #282828 text, 16px/400, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page.
- Do keep text in 2 levels: #FFFFFF, #444444.
- Do reserve #EC520B for primary actions and key highlights.
- Do keep spacing on the 8px grid.
- Do use 200px corners on most elements; larger surfaces also use 40px and 45px.
- Don't use #444444 for body text; it reaches 2.2:1 on #000000. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond system-ui, custom 157067 and custom 190030.
- Don't use #EC520B for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/readymag.com/), the free DESIGN.md generator.
