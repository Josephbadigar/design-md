---
version: alpha
name: PayPal
description: "Light interface measured from paypal.com: PayPal Pro type with PayPal Pro Text VF, cyan accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  surface-container-low: "#EDF0F2"
  surface-container: "#CCCCCC"
  overlay: "#05378214"
  overlay-strong: "#CCCCCC47"
  outline: "#CFD3D8"
  primary: "#60CDFF"
  on-primary: "#000000"
  secondary: "#002991"
  tertiary: "#0066F5"
typography:
  headline-display:
    fontFamily: PayPal Pro
    fontSize: 121px
    fontWeight: 900
    lineHeight: 1
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: PayPal Pro
    fontSize: 67px
    fontWeight: 900
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-md:
    fontFamily: PayPal Pro
    fontSize: 55.5px
    fontWeight: 900
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-sm:
    fontFamily: PayPal Pro
    fontSize: 45.5px
    fontWeight: 900
    lineHeight: 1.1
    letterSpacing: -0.03em
  title-lg:
    fontFamily: PayPal Pro Text VF
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-md:
    fontFamily: PayPal Pro Text VF
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  body-lg:
    fontFamily: PayPal Pro Text VF
    fontSize: 21.5px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.015em
  label-md:
    fontFamily: PayPal Pro Text VF
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: -0.015em
  label-sm:
    fontFamily: PayPal Pro Text VF
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: -0.015em
  headline-lg-mobile:
    fontFamily: PayPal Pro
    fontSize: 42.5px
    fontWeight: 900
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-sm-mobile:
    fontFamily: PayPal Pro
    fontSize: 32px
    fontWeight: 900
    lineHeight: 1.1
    letterSpacing: -0.03em
rounded:
  md: 24px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 23.19px
  xl: 52.8px
  gutter: 24px
  section: 52.8px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 20px
    height: 48px
  button-primary-hover:
    backgroundColor: "#333333"
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 105.6px 0px 79.2px 0px
  link:
    textColor: "{colors.on-surface}"
---

# PayPal Design System

## Overview

PayPal describes itself as: “From paying friends to saving money or getting cash back when you shop, explore what the new PayPal app has to offer.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Cyan (#60CDFF)** as the main accent.

Type is set in **PayPal Pro** and **PayPal Pro Text VF**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [paypal.com](https://www.paypal.com/us/home) on October 29, 2026 at 1440×900 and 390×844 from 247 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles, plus gradient stops #002991.

- **White (#FFFFFF):** Page background, seen 8 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Near Black (#000000):** Primary text and headings, seen 73 times. Token `on-surface`.
- **Mist (#EDF0F2):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Silver (#CCCCCC):** Cards and panels, seen 2 times. Token `surface-container`.
- **Dark Blue 8% (#05378214):** Translucent fill for cards and controls, seen 9 times. Token `overlay`.
- **Silver 28% (#CCCCCC47):** Stronger translucent fill, seen 5 times. Token `overlay-strong`.
- **Cool Silver (#CFD3D8):** Borders and dividers, seen 2 times. Token `outline`.
- **Cyan (#60CDFF):** Brand color on large areas, seen 3 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#002991):** Accent in text, fills and borders, seen 4 times. Token `secondary`.
- **Vivid Blue (#0066F5):** Accent in text, fills and borders, seen 2 times. Token `tertiary`.

## Typography

**PayPal Pro** and **PayPal Pro Text VF** share the interface. Fallback stack: `PayPal Pro, Century Gothic, Helvetica, Arial`.

- **headline-display:** PayPal Pro 121px at weight 900, line height 1, tracking -0.03em. Page title (h1).
- **headline-lg:** PayPal Pro 67px at weight 900, line height 1.1, tracking -0.03em (42.5px on mobile). Section headings (h2).
- **headline-md:** PayPal Pro 55.5px at weight 900, line height 1.1, tracking -0.03em. Sub-section headings.
- **headline-sm:** PayPal Pro 45.5px at weight 900, line height 1.1, tracking -0.03em (32px on mobile). Card and feature titles.
- **title-lg:** PayPal Pro Text VF 26px at weight 400, line height 1.2, tracking -0.02em. Small titles.
- **body-md:** PayPal Pro Text VF 16px at weight 400, line height 1.15. Body text.
- **body-lg:** PayPal Pro Text VF 21.5px at weight 400, line height 1.5, tracking -0.015em. Lead paragraphs.
- **label-md:** PayPal Pro Text VF 16px at weight 700, line height 1.5, tracking -0.015em. Buttons, navigation and labels.
- **label-sm:** PayPal Pro Text VF 14px at weight 700, line height 1.5, tracking -0.015em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 42% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 12px, lg 23.19px, xl 52.8px.
- **Sections:** 52.8px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Breakpoints:** 752px, 1024px, 1152px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.08) 0px 24px 48px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 100 elements.
- **md (24px):** 72 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Learn More”):** #000000 fill, #FFFFFF text, 16px/700, 1000px radius, padding 12px 20px.
- **button-primary-hover:** background #333333, text #FFFFFF on hover.
- **card:** #FFFFFF fill, #000000 text, 16px/400, padding 105.6px 0px 79.2px 0px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #EDF0F2, #CCCCCC.
- Do use #60CDFF as the brand accent: header, logo and key highlights.
- Do set headlines in PayPal Pro with tight tracking (-0.03em).
- Do reuse the measured spacing steps (8px, 12px, 23.19px).
- Do make buttons and chips fully rounded (9999px); most other elements use 24px corners.
- Don't introduce new font families beyond PayPal Pro and PayPal Pro Text VF.
- Don't use #60CDFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s. Longer ambient animations run 0.7s.

- **Easing:** `cubic-bezier(0.4, 1.2, 0.2, 1)`, `ease`, `cubic-bezier(0.37, 0.34, 0.26, 0.9)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/paypal.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
