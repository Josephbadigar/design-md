---
version: alpha
name: Nike
description: "Light monochrome interface measured from nike.com: Nike Futura ND type with Helvetica Now Text, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#111111"
  on-background: "#111111"
  on-surface-strong: "#000000"
  on-surface-variant: "#707072"
  overlay: "#FFFFFF80"
  outline: "#E5E5E5"
  primary: "#111111"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: Nike Futura ND
    fontSize: 72px
    fontWeight: 500
    lineHeight: 0.9
    letterSpacing: -0.007em
  headline-lg:
    fontFamily: Helvetica Now Text
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.43
  headline-md:
    fontFamily: Helvetica Now Display
    fontSize: 24px
    fontWeight: 500
  headline-sm:
    fontFamily: Helvetica Now Display
    fontSize: 20px
    fontWeight: 500
  body-md:
    fontFamily: Helvetica Now Text
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Helvetica Now Text
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Helvetica Now Text
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Helvetica Now Text
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Nike Futura ND
    fontSize: 40px
    fontWeight: 500
    lineHeight: 0.9
    letterSpacing: -0.013em
rounded:
  md: 24px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 60px
  gutter: 8px
components:
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 1px 6px
  input-field:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.primary}"
---

# Nike Design System

## Overview

Nike describes itself as: “Nike - Official Online Store for Athletic Shoes, Clothing & Sports Gear. Shop the latest Nike products and enjoy free shipping.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#111111)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Nike Futura ND** and **Helvetica Now Text**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Controls are pill-shaped.

Measured from [nike.com](https://www.nike.in/) on October 21, 2026 at 1440×900 and 390×844 from 124 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **White (#FFFFFF):** Page background, seen 12 times. Token `background`.
- **Charcoal (#111111):** Primary text and headings, seen 39 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 7 times. Token `on-surface-strong`.
- **Slate (#707072):** Secondary text, seen 21 times. Token `on-surface-variant`.
- **White 50% (#FFFFFF80):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Mist (#E5E5E5):** Borders and dividers, seen 1 time. Token `outline`.
- **Charcoal (#111111):** Primary actions (the main text color; the palette is monochrome), seen 42 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**Nike Futura ND**, **Helvetica Now Text** and **Helvetica Now Display** share the interface. Fallback stack: `Nike Futura ND, Helvetica Now Text Medium, Helvetica, Arial`.

- **headline-display:** Nike Futura ND 72px at weight 500, line height 0.9, tracking -0.007em (40px on mobile). Page title (h1).
- **headline-lg:** Helvetica Now Text 32px at weight 700, line height 1.43. Section headings (h2).
- **headline-md:** Helvetica Now Display 24px at weight 500, capitalize. Sub-section headings.
- **headline-sm:** Helvetica Now Display 20px at weight 500. Card and feature titles.
- **body-md:** Helvetica Now Text 14px at weight 400, line height 1.5. Body text.
- **label-lg:** Helvetica Now Text 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** Helvetica Now Text 14px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Helvetica Now Text 12px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (83% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 60px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 340px, 768px, 960px, 1300px, 1600px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #E5E5E5 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (24px):** 24 elements.
- **full (9999px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Sign Up”):** transparent fill, #111111 text, 12px/500, padding 1px 6px.
- **input-field (“Search”):** transparent fill, #000000 text, 16px/500, padding 0px.
- **link:** transparent fill, #111111 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #111111, #000000, #707072.
- Do let contrast carry emphasis; primary actions use #111111 on #FFFFFF.
- Do set headlines in Nike Futura ND with tight tracking (-0.007em).
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 24px corners.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Nike Futura ND, Helvetica Now Text and Helvetica Now Display.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.5s. Longer ambient animations run 8s.

- **Easing:** `ease`, `linear`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/nike.com/), the free DESIGN.md generator.
