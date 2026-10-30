---
version: alpha
name: Robinhood
description: "Dark interface measured from robinhood.com: Phonic type with Capsule Sans Text, vivid lime accents, tonal surfaces and 36px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#D9D9D9"
  surface-container-low: "#110E08"
  outline: "#110E08"
  primary: "#CCFF00"
  on-primary: "#110E08"
typography:
  display-hero:
    fontFamily: Phonic
    fontSize: 52px
    fontWeight: 400
    lineHeight: 1.19
    letterSpacing: -0.029em
  headline-display:
    fontFamily: Phonic
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Phonic
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.36
    letterSpacing: -0.023em
  body-md:
    fontFamily: Phonic
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.016em
  body-sm:
    fontFamily: Capsule Sans Text
    fontSize: 13px
    fontWeight: 400
    letterSpacing: -0.077em
  label-md:
    fontFamily: Capsule Sans Text
    fontSize: 16px
    fontWeight: 400
  headline-display-mobile:
    fontFamily: Phonic
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.21
    letterSpacing: -0.012em
  display-hero-mobile:
    fontFamily: Phonic
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.025em
rounded:
  md: 36px
spacing:
  sm: 8px
  md: 10px
  lg: 32px
  xl: 36px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 0px 32px
    height: 44px
  button-outline:
    textColor: "{colors.primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 32px
    height: 44px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-primary}"
---

# Robinhood Design System

## Overview

Robinhood describes itself as: “Trade stocks on Robinhood with commission-free investing & advanced trading tools. Access fractional shares, real-time market data, and more. Terms and fees may apply.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Vivid Lime (#CCFF00)** as the main accent.

Type is set in **Phonic** and **Capsule Sans Text**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 36px.

Measured from [robinhood.com](https://robinhood.com/us/en/) on October 29, 2026 at 1440×900 and 390×844 from 349 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **Near Black (#000000):** Page background, seen 2 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 11 times. Token `on-surface`.
- **Silver (#D9D9D9):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Warm Charcoal (#110E08):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Warm Charcoal (#110E08):** Borders and dividers, seen 2 times. Token `outline`.
- **Vivid Lime (#CCFF00):** Brand color in the header, seen 14 times. Token `primary`.
- **Warm Charcoal (#110E08):** Text and icons on primary. Token `on-primary`.

## Typography

**Phonic** and **Capsule Sans Text** share the interface. Fallback stack: `Phonic, Helvetica, system-ui, -apple-system`. Other loaded fonts: Martina Plantijn.

- **display-hero:** Phonic 52px at weight 400, line height 1.19, tracking -0.029em (40px on mobile). Oversized hero statements.
- **headline-display:** Phonic 40px at weight 400, line height 1.2, tracking -0.025em (28px on mobile). Page title (h1).
- **headline-lg:** Phonic 22px at weight 400, line height 1.36, tracking -0.023em. Section headings (h2).
- **body-md:** Phonic 16px at weight 400, line height 1.5, tracking -0.016em. Body text.
- **body-sm:** Capsule Sans Text 13px at weight 400, tracking -0.077em. Secondary and small text.
- **label-md:** Capsule Sans Text 16px at weight 400. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (89% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** sm 8px, md 10px, lg 32px, xl 36px.
- **Breakpoints:** 360px, 425px, 426px, 485px, 767px, 768px, 900px, 901px, 1023px, 1024px, 1048px, 1049px, 1279px, 1280px, 1399px, 1400px, 1441px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#110E08) and #110E08 borders.

## Shapes

Most elements use 36px corners. Measured radii, most used first:

- **md (36px):** 32 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #CCFF00 fill, #110E08 text, 13px/400, 36px radius, padding 0px 32px, border 1px solid #CCFF00.
- **button-outline (“Log in”):** transparent fill, #CCFF00 text, 16px/400, 36px radius, padding 0px 32px, border 1px solid #CCFF00.
- **button-ghost (“Crypto Risk Disclosures”):** transparent fill, #110E08 text, 13px/400, padding 0px.
- **link:** transparent fill, #110E08 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #110E08.
- Do keep text in 2 levels: #FFFFFF, #D9D9D9.
- Do use #CCFF00 as the brand accent: header, logo and key highlights.
- Do set headlines in Phonic with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 10px, 32px).
- Do use 36px corners on most elements.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Phonic and Capsule Sans Text.
- Don't use #CCFF00 for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/robinhood.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
