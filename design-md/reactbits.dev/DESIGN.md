---
version: alpha
name: React Bits
description: "Dark monochrome interface measured from reactbits.dev: Geist type, tonal surfaces and 16px corners."
colors:
  background: "#120F17"
  surface: "#120F17"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#F6F4F9"
  on-surface-muted: "#9B989F"
  on-surface-subtle: "#96909F"
  surface-container-low: "#0E0B13"
  surface-container: "#221E29"
  overlay: "#18141F8C"
  overlay-strong: "#09080B8C"
  outline: "#FFFFFF0D"
  primary: "#F4F2F7"
  on-primary: "#141118"
typography:
  headline-display:
    fontFamily: Geist
    fontSize: 42px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.036em
  headline-lg:
    fontFamily: Geist
    fontSize: 37.5px
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: -0.036em
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Geist
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.7
  caption:
    fontFamily: Geist
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.55
  label-lg:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: Geist
    fontSize: 15px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: -0.017em
  label-sm:
    fontFamily: Geist
    fontSize: 14.5px
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: -0.005em
  code:
    fontFamily: ui-monospace
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.72
  headline-display-mobile:
    fontFamily: Geist
    fontSize: 29px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.036em
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 29px
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: -0.036em
rounded:
  xs: 5px
  sm: 8px
  md: 11px
  lg: 14px
  xl: 16px
  full: 9999px
spacing:
  sm: 5px
  md: 16px
  lg: 17px
  xl: 52px
  gutter: 16px
  section: 80px
  margin: 24px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: 13px
    padding: 0px 17px 0px 21px
    height: 46px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: 13px
    padding: 0px 20px
    height: 46px
  button-outline-hover:
    backgroundColor: "#2B2633"
  button-secondary:
    backgroundColor: "#64646A"
    textColor: "{colors.on-surface}"
    typography: "{typography.caption}"
    rounded: 10px
    padding: 0px 18px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.code}"
    rounded: "{rounded.xs}"
    padding: 0px 1.4px
  card:
    backgroundColor: "#FFFFFF0A"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.xl}"
    padding: 5px
  link:
    textColor: "{colors.on-surface}"
---

# React Bits Design System

## Overview

React Bits describes itself as: “Free, open source React components for animated text, backgrounds, interactive cards and micro interactions. Explore live demos and copy the source.” The interface is dark, built on **Cool Charcoal (#120F17)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Geist**, with **ui-monospace** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 16px.

Measured from [reactbits.dev](https://reactbits.dev/) on November 4, 2026 at 1440×900 and 390×844 from 375 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Cool Charcoal (#120F17):** Page background, seen 13 times. Token `background`, CSS `--field-bg`.
- **White (#FFFFFF):** Primary text and headings, seen 19 times. Token `on-surface`.
- **Snow (#F6F4F9):** Secondary text, seen 18 times. Token `on-surface-variant`.
- **Cool Gray (#9B989F):** Muted text and metadata, seen 12 times. Token `on-surface-muted`.
- **Cool Gray (#96909F):** Subtle text and placeholders, seen 14 times. Token `on-surface-subtle`.
- **Cool Charcoal (#0E0B13):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Cool Charcoal (#221E29):** Cards and panels, seen 2 times. Token `surface-container`.
- **Cool Charcoal 55% (#18141F8C):** Translucent fill for cards and controls, seen 27 times. Token `overlay`.
- **Near Black 55% (#09080B8C):** Stronger translucent fill, seen 20 times. Token `overlay-strong`.
- **White 5% (#FFFFFF0D):** Borders and dividers, seen 5 times. Token `outline`.
- **Snow (#F4F2F7):** Primary buttons and calls to action, seen 20 times. Token `primary`.
- **Cool Charcoal (#141118):** Text and icons on primary. Token `on-primary`.

## Typography

**Geist** and **ui-monospace** (monospace) share the interface. Fallback stack: `Geist, sans-serif`. Other loaded fonts: Geist Mono.

- **headline-display:** Geist 42px at weight 500, line height 1.1, tracking -0.036em (29px on mobile). Page title (h1).
- **headline-lg:** Geist 37.5px at weight 500, line height 1.08, tracking -0.036em (29px on mobile). Section headings (h2).
- **body-md:** Geist 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Geist 15px at weight 400, line height 1.7. Secondary and small text.
- **caption:** Geist 13px at weight 400, line height 1.55. Captions and fine print.
- **label-lg:** Geist 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** Geist 15px at weight 600, line height 1.5, tracking -0.017em. Buttons, navigation and labels.
- **label-sm:** Geist 14.5px at weight 500, line height 1.6, tracking -0.005em. Small labels and badges.
- **code:** ui-monospace 14px at weight 400, line height 1.72. Code and technical values.

## Layout

Spacing does not follow a strict grid: 41% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 5px, md 16px, lg 17px, xl 52px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 480px, 600px, 601px, 640px, 700px, 768px, 769px, 900px, 960px, 1000px, 1024px, 1100px, 2160px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#0E0B13 → #221E29):

- `rgba(255, 255, 255, 0.07) 0px 1px 0px 0px inset`
- `rgba(255, 255, 255, 0.07) 0px 1px 0px 0px inset, rgba(255, 255, 255, 0.04) 0px 0px 0px 1px inset`
- `rgba(255, 255, 255, 0.055) 0px 0px 0px 1px inset`

A few raised panels add a soft drop shadow: `rgba(255, 255, 255, 0.2) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.2) 0px 1px 2px 0px`.

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **xl (16px):** 128 elements.
- **md (11px):** 124 elements.
- **lg (14px):** 36 elements.
- **xs (5px):** 28 elements.
- **sm (8px):** 24 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Browse components”):** #F4F2F7 fill, #141118 text, 15px/500, 13px radius, padding 0px 17px 0px 21px.
- **button-primary-hover:** background #FFFFFF, text #141118 on hover.
- **button-outline (“Star on GitHub”):** #221E29 fill, #F6F4F9 text, 15px/500, 13px radius, padding 0px 20px, shadow `rgba(255, 255, 255, 0.07) 0px 1px 0px 0px inset, rgba(255, 255, 255, 0.04) 0px 0px 0px 1px inset`.
- **button-outline-hover:** background #2B2633, text #F6F4F9 on hover.
- **button-secondary (“Get React Bits Pro”):** #64646A fill, #FFFFFF text, 13px/600, 10px radius, padding 0px 18px, shadow `rgba(255, 255, 255, 0.2) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.2) 0px 1px 2px 0px`.
- **button-ghost (“"#a1a1aa"”):** transparent fill, #F6F4F9 text, 14px/400, 5px radius, padding 0px 1.4px.
- **card:** #FFFFFF0A fill, #FFFFFF text, 16px/500, 16px radius, padding 5px, shadow `rgba(255, 255, 255, 0.07) 0px 1px 0px 0px inset`.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #120F17 for the page and lift surfaces in small steps: #0E0B13, #221E29.
- Do keep text in 4 levels: #FFFFFF, #F6F4F9, #9B989F, #96909F.
- Do let contrast carry emphasis; primary actions use #F4F2F7 on #120F17.
- Do set headlines in Geist with tight tracking (-0.036em).
- Do reuse the measured spacing steps (5px, 16px, 17px).
- Do use 16px corners on most elements; larger surfaces also use 11px, 14px and 5px.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Geist and ui-monospace.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.46s.

## Motion

Interface transitions are quick: 0.15s, 0.12s, 0.2s, 0.3s.

- **Easing:** `cubic-bezier(0.23, 1, 0.32, 1)`, `ease`, `cubic-bezier(0.22, 1, 0.36, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/reactbits.dev/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
