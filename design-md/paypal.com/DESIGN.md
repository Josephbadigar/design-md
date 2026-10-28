---
version: alpha
name: PayPal
description: "Light interface measured from paypal.com: PayPal Pro type with PayPal Pro Text VF, dark blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#5E5E5E"
  surface-container-low: "#F5F7FA"
  overlay: "#05378214"
  overlay-strong: "#FFFFFFB3"
  outline: "#CFD3D8"
  primary: "#002991"
  on-primary: "#FFFFFF"
  secondary: "#60CDFF"
  tertiary: "#0066F5"
typography:
  headline-display:
    fontFamily: PayPal Pro
    fontSize: 81.5px
    fontWeight: 900
    lineHeight: 1.1
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
    fontFamily: PayPal Pro
    fontSize: 38px
    fontWeight: 900
    lineHeight: 1.1
    letterSpacing: -0.03em
  body-md:
    fontFamily: PayPal Pro Text VF
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  body-lg:
    fontFamily: PayPal Pro Text VF
    fontSize: 18px
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
  headline-display-mobile:
    fontFamily: PayPal Pro
    fontSize: 49px
    fontWeight: 900
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-lg-mobile:
    fontFamily: PayPal Pro
    fontSize: 42.5px
    fontWeight: 900
    lineHeight: 1.1
    letterSpacing: -0.03em
  title-lg-mobile:
    fontFamily: PayPal Pro
    fontSize: 28px
    fontWeight: 900
    lineHeight: 1.1
    letterSpacing: -0.03em
rounded:
  sm: 24px
  md: 96px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 52.8px
  gutter: 24px
  section: 52.8px
  container: 1440px
components:
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 10px 30px
    height: 48px
  button-outline-hover:
    backgroundColor: "#F0F2F9"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 20px
    height: 48px
  button-secondary-hover:
    backgroundColor: "#333333"
  card:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# PayPal Design System

## Overview

PayPal describes itself as: “PayPal Open's streamlined payment platform makes it simple for customers to pay their way—online, offline, on-the-go, using cards, digital wallets, instalments, and more.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Dark Blue (#002991)** as the main accent.

Type is set in **PayPal Pro** and **PayPal Pro Text VF**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [paypal.com](https://www.paypal.com/in/home) on October 21, 2026 at 1440×900 and 390×844 from 172 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 9 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Near Black (#000000):** Primary text and headings, seen 49 times. Token `on-surface`.
- **Slate (#5E5E5E):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Snow (#F5F7FA):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **Dark Blue 8% (#05378214):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **White 70% (#FFFFFFB3):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Cool Silver (#CFD3D8):** Borders and dividers, seen 2 times. Token `outline`.
- **Dark Blue (#002991):** Brand color on large areas, seen 2 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Cyan (#60CDFF):** Most used accent color, seen 11 times. Token `secondary`.
- **Vivid Blue (#0066F5):** Most used accent color, seen 3 times. Token `tertiary`.

## Typography

**PayPal Pro** and **PayPal Pro Text VF** share the interface. Fallback stack: `PayPal Pro, Century Gothic, Helvetica, Arial`.

- **headline-display:** PayPal Pro 81.5px at weight 900, line height 1.1, tracking -0.03em (49px on mobile). Page title (h1).
- **headline-lg:** PayPal Pro 67px at weight 900, line height 1.1, tracking -0.03em (42.5px on mobile). Section headings (h2).
- **headline-md:** PayPal Pro 55.5px at weight 900, line height 1.1, tracking -0.03em. Sub-section headings.
- **headline-sm:** PayPal Pro 45.5px at weight 900, line height 1.1, tracking -0.03em. Card and feature titles.
- **title-lg:** PayPal Pro 38px at weight 900, line height 1.1, tracking -0.03em (28px on mobile). Small titles.
- **body-md:** PayPal Pro Text VF 16px at weight 400, line height 1.15. Body text.
- **body-lg:** PayPal Pro Text VF 18px at weight 400, line height 1.5, tracking -0.015em. Lead paragraphs.
- **label-md:** PayPal Pro Text VF 16px at weight 700, line height 1.5, tracking -0.015em. Buttons, navigation and labels.
- **label-sm:** PayPal Pro Text VF 14px at weight 700, line height 1.5, tracking -0.015em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 64% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 12px, lg 24px, xl 52.8px.
- **Sections:** 52.8px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Breakpoints:** 752px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F5F7FA) and #CFD3D8 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 48 elements.
- **sm (24px):** 24 elements.
- **md (96px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Accept”):** #FFFFFFB3 fill, #000000 text, 14px/500, 1000px radius, padding 10px 30px, border 2px solid #CFD3D8.
- **button-outline-hover:** background #F0F2F9, text #000000 on hover.
- **button-secondary (“Sign Up”):** #000000 fill, #FFFFFF text, 16px/700, 1000px radius, padding 12px 20px.
- **button-secondary-hover:** background #333333, text #FFFFFF on hover.
- **card:** #000000 fill, #000000 text, 16px/400, 24px radius, padding 0px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5F7FA.
- Do keep text in 2 levels: #000000, #5E5E5E.
- Do use #002991 as the brand accent: header, logo and key highlights.
- Do set headlines in PayPal Pro with tight tracking (-0.03em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 24px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond PayPal Pro and PayPal Pro Text VF.
- Don't use #002991 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s.

- **Easing:** `cubic-bezier(0.4, 1.2, 0.2, 1)`, `ease`, `cubic-bezier(0.22, 1, 0.36, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/paypal.com/), the free DESIGN.md generator.
