---
version: alpha
name: Uber
description: "Dark monochrome interface measured from uber.com: UberMove type with sans-serif, tonal surfaces and pill-shaped controls."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#AFAFAF"
  on-surface-muted: "#4A4A4A"
  surface-container-low: "#111111"
  surface-container: "#292929"
  overlay: "#E0E0E099"
  primary: "#FFFFFF"
  on-primary: "#000000"
  secondary: "#0000EE"
typography:
  headline-display:
    fontFamily: UberMove
    fontSize: 52px
    fontWeight: 700
    lineHeight: 1.23
  headline-lg:
    fontFamily: UberMove
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.22
  headline-md:
    fontFamily: UberMove
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.33
  body-md:
    fontFamily: sans-serif
    fontSize: 16px
    fontWeight: 400
  body-lg:
    fontFamily: UberMoveText
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.33
  body-sm:
    fontFamily: UberMoveText
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  caption:
    fontFamily: UberMoveText
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.67
  label-md:
    fontFamily: UberMoveText
    fontSize: 16px
    fontWeight: 500
  label-sm:
    fontFamily: UberMoveText
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.14
  headline-display-mobile:
    fontFamily: UberMove
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.22
  headline-lg-mobile:
    fontFamily: UberMove
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.29
rounded:
  md: 8px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 18px
  xl: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 10px 12px
    height: 36px
  button-primary-hover:
    backgroundColor: "#E2E2E2"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#FCFCFC"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 10px 12px
    height: 36px
  button-secondary:
    backgroundColor: "#F6F6F6"
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 14px 16px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px
  input-field:
    textColor: "{colors.surface-container-low}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.primary}"
---

# Uber Design System

## Overview

Uber describes itself as: “Get a ride in minutes. Or become a driver and earn money on your schedule. Uber is finding you better ways to move, work, and succeed in India.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **UberMove** and **sans-serif**. Headlines run large; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [uber.com](https://www.uber.com/in/en/) on October 21, 2026 at 1440×900 and 390×844 from 265 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Near Black (#000000):** Page background, seen 10 times. Token `background`, CSS `--base-magenta-0`.
- **White (#FFFFFF):** Primary text and headings, seen 62 times. Token `on-surface`.
- **Gray (#AFAFAF):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Graphite (#4A4A4A):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Charcoal (#111111):** Raised areas one step from the page, seen 13 times. Token `surface-container-low`.
- **Graphite (#292929):** Cards and panels, seen 5 times. Token `surface-container`.
- **Silver 60% (#E0E0E099):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 76 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#0000EE):** Accent, seen 1 time. Token `secondary`.

## Typography

**UberMove**, **sans-serif** and **UberMoveText** share the interface. Fallback stack: `UberMove, UberMoveText, system-ui, Helvetica Neue`.

- **headline-display:** UberMove 52px at weight 700, line height 1.23 (36px on mobile). Page title (h1).
- **headline-lg:** UberMove 36px at weight 700, line height 1.22 (28px on mobile). Section headings (h2).
- **headline-md:** UberMove 24px at weight 700, line height 1.33. Sub-section headings.
- **body-md:** sans-serif 16px at weight 400. Body text.
- **body-lg:** UberMoveText 18px at weight 500, line height 1.33. Lead paragraphs.
- **body-sm:** UberMoveText 14px at weight 400, line height 1.43. Secondary and small text.
- **caption:** UberMoveText 12px at weight 400, line height 1.67. Captions and fine print.
- **label-md:** UberMoveText 16px at weight 500. Buttons, navigation and labels.
- **label-sm:** UberMoveText 14px at weight 500, line height 1.14. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 68% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 16px, lg 18px, xl 48px.
- **Breakpoints:** 320px, 600px, 767px, 768px, 1023px, 1024px, 1119px, 1120px, 1136px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#111111 → #292929).

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (8px):** 60 elements.
- **full (9999px):** 52 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #FFFFFF fill, #000000 text, 14px/500, 999px radius, padding 10px 12px.
- **button-primary-hover:** background #E2E2E2, text #000000 on hover.
- **button-outline (“Ride”):** #111111 fill, #FCFCFC text, 14px/500, 999px radius, padding 10px 12px.
- **button-secondary (“Schedule ahead”):** #F6F6F6 fill, #111111 text, 16px/500, 999px radius, padding 14px 16px.
- **button-ghost (“Change city”):** transparent fill, #FFFFFF text, 16px/400, 8px radius, padding 0px.
- **input-field (“Pickup location needs to be fill”):** transparent fill, #111111 text, 16px/400, padding 0px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #111111, #292929.
- Do keep text in 3 levels: #FFFFFF, #AFAFAF, #4A4A4A.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #000000.
- Do reuse the measured spacing steps (8px, 16px, 18px).
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't use #4A4A4A for body text; it reaches 2.4:1 on #000000. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond UberMove, sans-serif and UberMoveText.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.5s, 0.3s.

- **Easing:** `cubic-bezier(0.22, 1, 0.36, 1)`, `cubic-bezier(0, 0, 1, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/uber.com/), the free DESIGN.md generator.
