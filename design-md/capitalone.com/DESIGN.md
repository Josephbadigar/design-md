---
version: alpha
name: Capital One
description: "Light interface measured from capitalone.com: Optimist type, dark blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#141414"
  on-surface-muted: "#1F1F1F"
  on-surface-subtle: "#696969"
  surface-container-low: "#FFFFFFF2"
  outline: "#EBEBEB"
  primary: "#0276B1"
  on-primary: "#FFFFFF"
  inverse-surface: "#3D3D3D"
  secondary: "#CC2427"
  tertiary: "#013D5B"
typography:
  display-hero:
    fontFamily: Optimist
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.3
  headline-display:
    fontFamily: Optimist
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.5
  headline-lg:
    fontFamily: Optimist
    fontSize: 24px
    fontWeight: 300
    lineHeight: 1.5
  body-md:
    fontFamily: Optimist
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Optimist
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: Optimist
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Optimist
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: Optimist
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.5
  display-hero-mobile:
    fontFamily: Optimist
    fontSize: 32px
    fontWeight: 300
    lineHeight: 1.3
rounded:
  sm: 2px
  md: 4px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 40px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 6px 20px 7px 20px
    height: 32px
  button-primary-hover:
    backgroundColor: "#026597"
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px 12px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 5px 8px 5px 32px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 40px
  link:
    textColor: "#D4D4D4"
---

# Capital One Design System

## Overview

Capital One describes itself as: “Learn how banking with Capital One can help you meet your financial goals.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Dark Blue (#0276B1)** as the main accent.

Type is set in **Optimist**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [capitalone.com](https://www.capitalone.com/) on November 4, 2026 at 1440×900 and 390×844 from 231 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 9 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 19 times. Token `on-surface`.
- **Charcoal (#141414):** Secondary text, seen 26 times. Token `on-surface-variant`.
- **Charcoal (#1F1F1F):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Slate (#696969):** Subtle text and placeholders, seen 5 times. Token `on-surface-subtle`.
- **White 95% (#FFFFFFF2):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Mist (#EBEBEB):** Borders and dividers, seen 1 time. Token `outline`.
- **Dark Blue (#0276B1):** Primary buttons and calls to action, seen 17 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Graphite (#3D3D3D):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Red (#CC2427):** Accent in the logo, seen 1 time. Token `secondary`, CSS `--gds-color-border-critical-empahsis-high`.
- **Deep Blue (#013D5B):** Accent in the logo, seen 10 times. Token `tertiary`, CSS `--gds-color-text-and-icon-interactive-press`.

## Typography

**Optimist** carries the whole interface. Fallback stack: `Optimist, Helvetica Neue, Helvetica, Arial`.

- **display-hero:** Optimist 40px at weight 300, line height 1.3 (32px on mobile). Oversized hero statements.
- **headline-display:** Optimist 32px at weight 700, line height 1.5. Page title (h1).
- **headline-lg:** Optimist 24px at weight 300, line height 1.5. Section headings (h2).
- **body-md:** Optimist 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Optimist 14px at weight 400, line height 1.5. Secondary and small text.
- **caption:** Optimist 12px at weight 400, line height 1.5. Captions and fine print.
- **label-md:** Optimist 16px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Optimist 14px at weight 600, line height 1.5. Small labels and badges.

## Layout

Spacing follows a 4px grid: 91% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 40px.
- **Breakpoints:** 0px, 368px, 369px, 599px, 600px, 767px, 768px, 1023px, 1024px, 1200px, 1920px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.2) 0px 1px 4px 0px`

Hairline rings and inset highlights also appear: `rgb(105, 105, 105) 0px 0px 0px 1px inset`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (4px):** 26 elements.
- **sm (2px):** 12 elements.
- **full (9999px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign in”):** #0276B1 fill, #FFFFFF text, 16px/600, 2px radius, padding 6px 20px 7px 20px.
- **button-primary-hover:** background #026597, text #FFFFFF on hover.
- **button-ghost (“Search”):** transparent fill, #141414 text, 14px/300, padding 0px 12px.
- **input-field (“Username”):** #FFFFFF fill, #141414 text, 14px/400, 2px radius, padding 5px 8px 5px 32px, shadow `rgb(105, 105, 105) 0px 0px 0px 1px inset`.
- **card:** #FFFFFFF2 fill, #141414 text, 16px/400, 4px radius, padding 40px.
- **link:** transparent fill, #D4D4D4 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FFFFFFF2.
- Do keep text in 4 levels: #000000, #141414, #1F1F1F, #696969.
- Do reserve #0276B1 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't introduce new font families beyond Optimist.
- Don't use #0276B1 for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/capitalone.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
