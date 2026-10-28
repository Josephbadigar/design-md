---
version: alpha
name: Sketch
description: "Light monochrome interface measured from sketch.com: Reckless type with InterVariable, tonal surfaces and 20px corners."
colors:
  background: "#F5F5F5"
  surface: "#F5F5F5"
  on-surface: "#212123"
  on-background: "#212123"
  on-surface-strong: "#000000"
  on-surface-variant: "#494949"
  on-surface-muted: "#585858"
  surface-container-low: "#F9F9F9"
  surface-container: "#FAFAFA"
  surface-container-high: "#FFFFFF"
  overlay: "#FFFFFF7A"
  outline: "#0000001A"
  primary: "#151515"
  on-primary: "#FFFFFF"
  secondary: "#0000EE"
typography:
  headline-display:
    fontFamily: Reckless
    fontSize: 76px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Reckless
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.09
    letterSpacing: -0.023em
  body-md:
    fontFamily: InterVariable
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  body-lg:
    fontFamily: InterVariable
    fontSize: 22px
    fontWeight: 600
    lineHeight: 1.09
  body-sm:
    fontFamily: InterVariable
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
  caption:
    fontFamily: InterVariable
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: InterVariable
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Reckless
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
  headline-lg-mobile:
    fontFamily: Reckless
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.016em
rounded:
  sm: 3px
  md: 16px
  lg: 20px
  xl: 24px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 14px
  lg: 32px
  xl: 52px
  gutter: 24px
  section: 128px
  margin: 32px
  container: 1200px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 11px 16px 12px 24px
    height: 47px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px 14px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 100px 100px 78px 78px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Sketch Design System

## Overview

Sketch describes itself as: “Sketch puts the focus back on you and your work. Made by designers, for designers.” The interface is light, built on **Snow (#F5F5F5)** with **Charcoal (#212123)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Reckless** and **InterVariable**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 20px.

Measured from [sketch.com](https://www.sketch.com/) on October 21, 2026 at 1440×900 and 390×844 from 315 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #32ADF7, #744BD0, #E97F42, #FCC1C1.

- **Snow (#F5F5F5):** Page background, seen 1 time. Token `background`.
- **Charcoal (#212123):** Primary text and headings, seen 16 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 8 times. Token `on-surface-strong`.
- **Graphite (#494949):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Slate (#585858):** Muted text and metadata, seen 30 times. Token `on-surface-muted`.
- **Snow (#F9F9F9):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#FAFAFA):** Cards and panels, seen 1 time. Token `surface-container`.
- **White (#FFFFFF):** Hover and pressed fills, seen 7 times. Token `surface-container-high`.
- **White 48% (#FFFFFF7A):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Near Black 10% (#0000001A):** Borders and dividers, seen 2 times. Token `outline`.
- **Charcoal (#151515):** Primary buttons and calls to action, seen 4 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#0000EE):** Most used accent color, seen 3 times. Token `secondary`.

## Typography

**Reckless** and **InterVariable** share the interface. Fallback stack: `Reckless, serif`. Other loaded fonts: Inter.

- **headline-display:** Reckless 76px at weight 500, line height 1, tracking -0.02em (48px on mobile). Page title (h1).
- **headline-lg:** Reckless 44px at weight 500, line height 1.09, tracking -0.023em (32px on mobile). Section headings (h2).
- **body-md:** InterVariable 16px at weight 400, line height 1. Body text.
- **body-lg:** InterVariable 22px at weight 600, line height 1.09. Lead paragraphs.
- **body-sm:** InterVariable 15px at weight 400, line height 1.6. Secondary and small text.
- **caption:** InterVariable 14px at weight 400, line height 1.5. Captions and fine print.
- **label-md:** InterVariable 16px at weight 600, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 91% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 14px, lg 32px, xl 52px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1200px.
- **Page margin:** 32px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.05) 0px 1px 1px 0px inset, rgba(255, 255, 255, 0.5) 0px 1px 4px 0px inset, rgba(0, 0, 0, 0.94) 0px -2px 4px 0px inset, rgba(0, 0, 0, 0.2) 0px 1px 4px 0px`
- `rgba(0, 0, 0, 0.1) 0px 1px 2px 0px`
- `rgba(0, 0, 0, 0.08) 0px 0px 4px 0px, rgba(0, 0, 0, 0.02) 0px 4px 8px 0px, rgba(0, 0, 0, 0.08) 0px 1px 2px 0px`

Hairline rings and inset highlights also appear: `rgb(230, 230, 230) 0px 0px 0px 1px, rgba(0, 0, 0, 0.04) 0px 1px 2px 0px inset`.

## Shapes

Most elements use 20px corners. Measured radii, most used first:

- **lg (20px):** 28 elements.
- **xl (24px):** 16 elements.
- **sm (3px):** 4 elements.
- **md (16px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #151515 fill, #FFFFFF text, 16px/600, 24px radius, padding 11px 16px 12px 24px, shadow `rgba(0, 0, 0, 0.05) 0px 1px 1px 0px inset, rgba(255, 255, 255, 0.5) 0px 1px 4px 0px inset, rgba(0, 0, 0, 0.94) 0px -2px 4px 0px inset, rgba(0, 0, 0, 0.2) 0px 1px 4px 0px`.
- **input-field (“Email address”):** #F9F9F9 fill, #000000 text, 16px/400, 16px radius, padding 12px 14px, shadow `rgb(230, 230, 230) 0px 0px 0px 1px, rgba(0, 0, 0, 0.04) 0px 1px 2px 0px inset`.
- **card:** #FFFFFF7A fill, #212123 text, 16px/400, 20px radius, padding 100px 100px 78px 78px, shadow `rgba(0, 0, 0, 0.08) 0px 0px 4px 0px, rgba(0, 0, 0, 0.02) 0px 4px 8px 0px, rgba(0, 0, 0, 0.08) 0px 1px 2px 0px`.
- **link:** transparent fill, #000000A3 text, padding 0px.

## Do's and Don'ts

- Do use #F5F5F5 for the page and lift surfaces in small steps: #F9F9F9, #FAFAFA, #FFFFFF.
- Do keep text in 4 levels: #212123, #000000, #494949, #585858.
- Do let contrast carry emphasis; primary actions use #151515 on #F5F5F5.
- Do set headlines in Reckless with tight tracking (-0.02em).
- Do keep spacing on the 4px grid.
- Do use 20px corners on most elements; larger surfaces also use 24px, 3px and 16px.
- Don't introduce new font families beyond Reckless and InterVariable.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.001s, 0.25s, 0.4s. Longer ambient animations run 6s.

- **Easing:** `cubic-bezier(0.455, 0.03, 0.515, 0.955)`, `ease`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/sketch.com/), the free DESIGN.md generator.
