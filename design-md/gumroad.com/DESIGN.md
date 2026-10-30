---
version: alpha
name: Gumroad
description: "Light monochrome interface measured from gumroad.com: ABC Favorit type with Arial, tonal surfaces and 4px corners."
colors:
  background: "#F4F4F0"
  surface: "#F4F4F0"
  on-surface: "#000000"
  on-background: "#000000"
  surface-container-low: "#FFFFFF"
  outline: "#D1D5DC"
  outline-variant: "#FFFFFF4D"
  primary: "#000000"
  on-primary: "#FFFFFF"
  secondary: "#FF90E8"
typography:
  headline-display:
    fontFamily: ABC Favorit
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.006em
  headline-lg:
    fontFamily: ABC Favorit
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.008em
  headline-md:
    fontFamily: ABC Favorit
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.11
    letterSpacing: -0.011em
  headline-sm:
    fontFamily: ABC Favorit
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.017em
  body-md:
    fontFamily: ABC Favorit
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.63
    letterSpacing: -0.025em
  body-lg:
    fontFamily: ABC Favorit
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
    letterSpacing: -0.022em
  body-sm:
    fontFamily: ABC Favorit
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: -0.029em
  label-md:
    fontFamily: Arial
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: ABC Favorit
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.011em
rounded:
  sm: 4px
  md: 6px
spacing:
  base: 8px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    padding: 8px 16px
    height: 46px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#242423"
    rounded: "{rounded.md}"
    padding: 8px
    height: 42px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    padding: 6px
    height: 34px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
    padding: 0px 80px 0px 32px
  link:
    textColor: "#24242380"
---

# Gumroad Design System

## Overview

Gumroad describes itself as: “Start selling what you know, see what sticks, and get paid. Simple and effective.” The interface is light, built on **Mist (#F4F4F0)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **ABC Favorit** and **Arial**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 4px.

Measured from [gumroad.com](https://gumroad.com/) on October 29, 2026 at 1440×900 and 390×844 from 186 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Mist (#F4F4F0):** Page background, seen 4 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 131 times. Token `on-surface`, CSS `--color-warning-foreground`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 88 times. Token `surface-container-low`, CSS `--active-bg`.
- **Cool Silver (#D1D5DC):** Borders and dividers, seen 86 times. Token `outline`.
- **White 30% (#FFFFFF4D):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Near Black (#000000):** Primary buttons and calls to action, seen 154 times. Token `primary`, CSS `--color-warning-foreground`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Purple (#FF90E8):** Accent, seen 3 times. Token `secondary`, CSS `--color-indicator`.

## Typography

**ABC Favorit** and **Arial** share the interface. Fallback stack: `ABC Favorit`.

- **headline-display:** ABC Favorit 72px at weight 500, line height 1, tracking -0.006em (36px on mobile). Page title (h1).
- **headline-lg:** ABC Favorit 48px at weight 500, line height 1, tracking -0.008em. Section headings (h2).
- **headline-md:** ABC Favorit 36px at weight 400, line height 1.11, tracking -0.011em. Sub-section headings.
- **headline-sm:** ABC Favorit 24px at weight 500, line height 1.33, tracking -0.017em. Card and feature titles.
- **body-md:** ABC Favorit 16px at weight 400, line height 1.63, tracking -0.025em. Body text.
- **body-lg:** ABC Favorit 18px at weight 400, line height 1.56, tracking -0.022em. Lead paragraphs.
- **body-sm:** ABC Favorit 14px at weight 400, line height 1.43, tracking -0.029em. Secondary and small text.
- **label-md:** Arial 16px at weight 400, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing follows a 8px grid: 98% of measured gaps and paddings are multiples of 8px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Gaps:** 32px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF) and #D1D5DC borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 16 elements.
- **md (6px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“About”):** #000000 fill, #FFFFFF text, 18px/400, 3.35544e+07px radius, padding 8px 16px, border 1px solid #000000.
- **button-outline (“Search”):** #FFFFFF fill, #242423 text, 13.3333px/400, 6px radius, padding 8px, border 1px solid #242423.
- **button-ghost (“10K”):** transparent fill, #000000 text, 16px/400, 3.35544e+07px radius, padding 6px, border 1px solid #000000.
- **input-field (“Search marketplace ...”):** #F4F4F0 fill, #000000 text, 20px/400, 4px radius, padding 0px 80px 0px 32px, border 1px solid #242423.
- **link:** transparent fill, #24242380 text, padding 0px.

## Do's and Don'ts

- Do use #F4F4F0 for the page and lift surfaces in small steps: #FFFFFF.
- Do let contrast carry emphasis; primary actions use #000000 on #F4F4F0.
- Do set headlines in ABC Favorit with tight tracking (-0.006em).
- Do keep spacing on the 8px grid.
- Do use 4px corners on most elements; larger surfaces also use 6px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond ABC Favorit and Arial.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/gumroad.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
