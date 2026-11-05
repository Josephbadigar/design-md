---
version: alpha
name: Fonts In Use
description: "Light monochrome interface measured from fontsinuse.com: RelayCond type with BentonSansRE, tonal surfaces and 2px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#999999"
  surface-container-low: "#F0F0F0"
  surface-container: "#DDDDDD"
  surface-container-high: "#CCCCCC"
  outline: "#F0F0F0"
  outline-variant: "#DDDDDD"
  primary: "#000000"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: RelayCond
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1
  body-md:
    fontFamily: BentonSansRE
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: BentonSansRE
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.1
  label-md:
    fontFamily: BentonSansRE
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.2
  label-sm:
    fontFamily: BentonSansRE
    fontSize: 12px
    fontWeight: 700
    lineHeight: 1.6
rounded:
  md: 2px
spacing:
  sm: 5px
  md: 10px
  lg: 20px
components:
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: 3px
    padding: 0px 10px
  link:
    textColor: "{colors.primary}"
---

# Fonts In Use Design System

## Overview

Fonts In Use describes itself as: “A searchable archive of typographic design, indexed by typeface, format, and topic.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **RelayCond** and **BentonSansRE**. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 2px.

Measured from [fontsinuse.com](https://fontsinuse.com/) on November 4, 2026 at 1440×900 and 390×844 from 240 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 6 times. Token `background`, CSS `--fiu-col-bkgd`.
- **Near Black (#000000):** Primary text and headings, seen 24 times. Token `on-surface`, CSS `--fiu-col-text`.
- **Gray (#999999):** Secondary text, seen 4 times. Token `on-surface-variant`, CSS `--fiu-col-midGrey1`.
- **Mist (#F0F0F0):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--fiu-col-superPale`.
- **Silver (#DDDDDD):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--fiu-col-paleGrey`.
- **Silver (#CCCCCC):** Hover and pressed fills, seen 1 time. Token `surface-container-high`, CSS `--fiu-col-paleGrey2`.
- **Mist (#F0F0F0):** Borders and dividers, seen 46 times. Token `outline`, CSS `--fiu-col-superPale`.
- **Silver (#DDDDDD):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--fiu-col-paleGrey`.
- **Near Black (#000000):** Primary actions (the main text color; the palette is monochrome), seen 24 times. Token `primary`, CSS `--fiu-col-text`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**RelayCond** and **BentonSansRE** share the interface. Fallback stack: `RelayCond, Arial, serif`.

- **headline-display:** RelayCond 36px at weight 700, line height 1. Page title (h1).
- **body-md:** BentonSansRE 14px at weight 400, line height 1.6. Body text.
- **body-sm:** BentonSansRE 10px at weight 400, line height 1.1. Secondary and small text.
- **label-md:** BentonSansRE 16px at weight 700, line height 1.2. Buttons, navigation and labels.
- **label-sm:** BentonSansRE 12px at weight 700, line height 1.6. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 31% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 5px, md 10px, lg 20px.
- **Breakpoints:** 640px, 768px, 992px, 1024px, 1200px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F0F0F0 → #DDDDDD → #CCCCCC) and hairline rings:

- `rgba(0, 0, 0, 0.05) 1px 1px 3px 1px inset`

## Shapes

Most elements use 2px corners. Measured radii, most used first:

- **md (2px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **input-field (“Enter a word, typeface, tag …”):** #FFFFFF fill, #000000 text, 12px/400, 3px radius, padding 0px 10px, border 1px solid #DDDDDD, shadow `rgba(0, 0, 0, 0.05) 1px 1px 3px 1px inset`.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F0F0F0, #DDDDDD, #CCCCCC.
- Do keep text in 2 levels: #000000, #999999.
- Do let contrast carry emphasis; primary actions use #000000 on #FFFFFF.
- Do reuse the measured spacing steps (5px, 10px, 20px).
- Do use 2px corners on most elements.
- Don't use #999999 for body text; it reaches 2.85:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond RelayCond and BentonSansRE.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.

Generated by [Sitepeel](https://sitepeel.dev/design-md/fontsinuse.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
