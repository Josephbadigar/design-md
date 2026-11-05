---
version: alpha
name: American Express
description: "Light interface measured from americanexpress.com: BentonSans type with system-ui, blue accents, flat surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#3D3D3D"
  on-background: "#3D3D3D"
  on-surface-strong: "#262626"
  on-surface-variant: "#595959"
  outline: "#B5D7F4"
  outline-variant: "#E0E0E0"
  primary: "#006FCF"
  on-primary: "#FFFFFF"
  inverse-surface: "#737373"
  secondary: "#0066BE"
  tertiary: "#00175A"
typography:
  display-hero:
    fontFamily: BentonSans
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.25
  headline-display:
    fontFamily: BentonSans
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.33
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Helvetica Neue
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.46
  caption:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.57
  label-lg:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: Helvetica Neue
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.46
  label-sm:
    fontFamily: BentonSans
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.38
rounded:
  sm: 4px
  md: 8px
  lg: 16px
  xl: 100px
spacing:
  xs: 3px
  sm: 8px
  md: 16px
  lg: 23px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 11px 23px
    height: 48px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.tertiary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 8px 16px 4px 16px
    height: 47px
  button-outline-hover:
    backgroundColor: "#F7F8F9"
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.secondary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 0px 15px
    height: 32px
  link:
    textColor: "{colors.secondary}"
---

# American Express Design System

## Overview

American Express describes itself as: “American Express offers world-class Charge and Credit Cards, Gift Cards, Rewards, Travel, Personal Savings, Business Services, Insurance and more.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#3D3D3D)** text, and **Blue (#006FCF)** as the main accent.

Type is set in **BentonSans** and **system-ui**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [americanexpress.com](https://www.americanexpress.com/) on November 4, 2026 at 1440×900 and 390×844 from 283 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 17 times. Token `background`, CSS `--ds-1218`.
- **Graphite (#3D3D3D):** Primary text and headings, seen 22 times. Token `on-surface`, CSS `--ds-391`.
- **Graphite (#262626):** Headings and emphasis, seen 3 times. Token `on-surface-strong`, CSS `--ds-754`.
- **Slate (#595959):** Secondary text, seen 4 times. Token `on-surface-variant`, CSS `--ds-456`.
- **Light Blue (#B5D7F4):** Borders and dividers, seen 7 times. Token `outline`, CSS `--ds-549`.
- **Silver (#E0E0E0):** Secondary dividers, seen 6 times. Token `outline-variant`, CSS `--ds-739`.
- **Blue (#006FCF):** Primary buttons and calls to action, seen 16 times. Token `primary`, CSS `--ds-582`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Slate (#737373):** High-contrast fills, seen 2 times. Token `inverse-surface`, CSS `--ds-745`.
- **Dark Blue (#0066BE):** Links and interactive text, seen 57 times. Token `secondary`, CSS `--ds-669`.
- **Deep Blue (#00175A):** Accent, seen 3 times. Token `tertiary`, CSS `--ds-1072`.

## Typography

**BentonSans**, **system-ui** and **Helvetica Neue** share the interface. Fallback stack: `BentonSans`.

- **display-hero:** BentonSans 32px at weight 400, line height 1.25. Oversized hero statements.
- **headline-display:** BentonSans 24px at weight 400, line height 1.33. Page title (h1).
- **body-md:** system-ui 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Helvetica Neue 15px at weight 400, line height 1.46. Secondary and small text.
- **caption:** system-ui 14px at weight 400, line height 1.57. Captions and fine print.
- **label-lg:** system-ui 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** Helvetica Neue 15px at weight 500, line height 1.46. Buttons, navigation and labels.
- **label-sm:** BentonSans 13px at weight 600, line height 1.38, uppercase. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 57% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 8px, md 16px, lg 23px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 319px, 320px, 375px, 567px, 568px, 767px, 799px, 800px, 1023px, 1024px, 1279px, 1280px, 1439px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.06) 0px 2px 4px -1px, rgba(0, 0, 0, 0.06) 0px 2px 5px 2px`
- `rgba(0, 0, 0, 0.16) 0px 2px 4px -1px, rgba(0, 0, 0, 0.04) 0px 2px 8px 3px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 60 elements.
- **sm (4px):** 38 elements.
- **lg (16px):** 28 elements.
- **xl (100px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Log In”):** #006FCF fill, #FFFFFF text, 16px/500, 8px radius, padding 11px 23px, border 1px solid #006FCF.
- **button-outline (“Personal”):** #FFFFFF fill, #00175A text, 16px/500, 4px 4px 0px 0px radius, padding 8px 16px 4px 16px, border 3px solid #00175A, shadow `rgba(0, 0, 0, 0.16) 0px 2px 4px -1px, rgba(0, 0, 0, 0.04) 0px 2px 8px 3px`.
- **button-outline-hover:** background #F7F8F9, text #00175A on hover.
- **button-ghost (“Explore Cards”):** #FFFFFF fill, #0066BE text, 16px/500, 8px radius, padding 0px 15px, border 1px solid #B5D7F4.
- **link:** transparent fill, #0066BE text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #3D3D3D, #262626, #595959.
- Do reserve #006FCF for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 23px).
- Do use 8px corners on most elements; larger surfaces also use 4px, 16px and 100px.
- Don't introduce new font families beyond BentonSans, system-ui and Helvetica Neue.
- Don't use #006FCF for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.25s, 0.15s. Longer ambient animations run 1s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/americanexpress.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
