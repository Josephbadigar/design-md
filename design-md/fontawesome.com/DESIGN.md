---
version: alpha
name: Font Awesome
description: "Light interface measured from fontawesome.com: cera-round-pro type, vivid amber accents, tonal surfaces and 12px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#183153"
  on-background: "#183153"
  on-surface-strong: "#000000"
  on-surface-variant: "#616D8A"
  surface-container-low: "#F0F1F3"
  overlay: "#1831534D"
  outline: "#74C0FC"
  outline-variant: "#C3C6D1"
  primary: "#FFD43B"
  on-primary: "#183153"
  secondary: "#418FDE"
  tertiary: "#146EBE"
  success: "#63E6BE"
  warning: "#FAB005"
typography:
  headline-display:
    fontFamily: cera-round-pro
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.13
  headline-lg:
    fontFamily: cera-round-pro
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.15
  headline-md:
    fontFamily: cera-round-pro
    fontSize: 30.5px
    fontWeight: 400
    lineHeight: 1.5
  headline-sm:
    fontFamily: cera-round-pro
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.13
  body-md:
    fontFamily: cera-round-pro
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: cera-round-pro
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: cera-round-pro
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.38
  headline-display-mobile:
    fontFamily: cera-round-pro
    fontSize: 37px
    fontWeight: 700
    lineHeight: 1.13
  headline-lg-mobile:
    fontFamily: cera-round-pro
    fontSize: 30.5px
    fontWeight: 700
    lineHeight: 1.15
  headline-sm-mobile:
    fontFamily: cera-round-pro
    fontSize: 18.5px
    fontWeight: 700
    lineHeight: 1.13
rounded:
  sm: 4.5px
  md: 9px
  lg: 12px
  xl: 32px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 32px
  xl: 64px
  gutter: 17.6px
  section: 64px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 15px 24px
    height: 58px
  button-primary-hover:
    backgroundColor: "{colors.warning}"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 16px 32px
    height: 63px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: 2px
    padding: 16px 32px
    height: 63px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: 8px
    padding: 8px 16px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 18px 128px 18px 55.2px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 24px 0px
  link:
    textColor: "{colors.background}"
---

# Font Awesome Design System

## Overview

Font Awesome describes itself as: “The internet's icon library + toolkit. Used by millions of designers, devs, & content creators. Open-source. Always free. Always awesome.” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#183153)** text, and **Vivid Amber (#FFD43B)** as the main accent.

Type is set in **cera-round-pro**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 12px.

Measured from [fontawesome.com](https://fontawesome.com/) on November 4, 2026 at 1440×900 and 390×844 from 423 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **White (#FFFFFF):** Page background, seen 25 times. Token `background`, CSS `--message-border-color`.
- **Deep Blue (#183153):** Primary text and headings, seen 63 times. Token `on-surface`, CSS `--tab-color`.
- **Near Black (#000000):** Headings and emphasis, seen 16 times. Token `on-surface-strong`.
- **Blue (#616D8A):** Secondary text, seen 25 times. Token `on-surface-variant`.
- **Mist (#F0F1F3):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **Deep Blue 30% (#1831534D):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Light Blue (#74C0FC):** Borders and dividers, seen 1 time. Token `outline`.
- **Cool Silver (#C3C6D1):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--table-th-border-color`.
- **Vivid Amber (#FFD43B):** Brand color in the header, seen 17 times. Token `primary`.
- **Deep Blue (#183153):** Text and icons on primary. Token `on-primary`.
- **Blue (#418FDE):** Accent in the logo, seen 1 time. Token `secondary`.
- **Blue (#146EBE):** Accent in text, fills and borders, seen 9 times. Token `tertiary`.
- **Teal (#63E6BE):** Success and positive states, seen 4 times. Token `success`, CSS `--pro-plus-plan-color`.
- **Vivid Amber (#FAB005):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**cera-round-pro** carries the whole interface. Fallback stack: `cera-round-pro, Helvetica Neue, Helvetica, Arial`. Other loaded fonts: Font Awesome 7 Pro.

- **headline-display:** cera-round-pro 48px at weight 700, line height 1.13 (37px on mobile). Page title (h1).
- **headline-lg:** cera-round-pro 40px at weight 700, line height 1.15 (30.5px on mobile). Section headings (h2).
- **headline-md:** cera-round-pro 30.5px at weight 400, line height 1.5. Sub-section headings.
- **headline-sm:** cera-round-pro 24px at weight 700, line height 1.13 (18.5px on mobile). Card and feature titles.
- **body-md:** cera-round-pro 14px at weight 400, line height 1.5. Body text.
- **label-md:** cera-round-pro 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** cera-round-pro 14px at weight 600, line height 1.38. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 66% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 16px, lg 32px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 17.6px is the most common gap in flex and grid layouts.
- **Breakpoints:** 450px, 750px, 767px, 768px, 1151px, 1152px, 1536px, 2000px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgb(195, 198, 209) 0px 4px 0px 0px`
- `rgb(24, 49, 83) 0px 4px 0px 0px`
- `rgb(195, 198, 209) 0px 6px 0px 0px`

Hairline rings and inset highlights also appear: `rgb(240, 241, 243) 0px 4px 0px 0px inset`.

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **lg (12px):** 68 elements.
- **md (9px):** 40 elements.
- **full (9999px):** 16 elements.
- **xl (32px):** 8 elements.
- **sm (4.5px):** 6 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start Free”):** #FFD43B fill, #183153 text, 16px/600, 12px radius, padding 15px 24px, border 2px solid #183153, shadow `rgb(24, 49, 83) 0px 6px 0px 0px`.
- **button-primary-hover:** background #FAB005, text #183153 on hover.
- **button-outline (“Font Awesome”):** #FFFFFF fill, #183153 text, 16px/400, 4.5px 4.5px 0px 0px radius, padding 16px 32px.
- **button-secondary (“Web Awesome”):** #183153 fill, #616D8A text, 16px/400, 2px radius, padding 16px 32px.
- **button-ghost (“Sign In”):** transparent fill, #616D8A text, 16px/600, 8px radius, padding 8px 16px.
- **input-field (“Find the perfect icon...”):** #FFFFFF fill, #000000 text, 16px/700, 32px radius, padding 18px 128px 18px 55.2px, border 2px solid #183153, shadow `rgb(240, 241, 243) 0px 4px 0px 0px inset`.
- **card:** #FFFFFF fill, #183153 text, 16px/400, padding 24px 0px, shadow `rgb(195, 198, 209) 0px 6px 0px 0px`.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F0F1F3.
- Do keep text in 3 levels: #183153, #000000, #616D8A.
- Do use #FFD43B as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (6px, 16px, 32px).
- Do use 12px corners on most elements; larger surfaces also use 9px, 32px and 4.5px.
- Don't introduce new font families beyond cera-round-pro.
- Don't use #FFD43B for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.1s, 0.5s, 0.25s. Longer ambient animations run 3.5s, 2.4s, 9.6s.

- **Easing:** `ease-in`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/fontawesome.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
