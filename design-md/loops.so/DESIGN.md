---
version: alpha
name: Loops
description: "Light monochrome interface measured from loops.so: Newsreader type with ui-serif, tonal surfaces and pill-shaped controls."
colors:
  background: "#F9F9F8"
  surface: "#F9F9F8"
  on-surface: "#21201C"
  on-background: "#21201C"
  on-surface-variant: "#44433F"
  on-surface-muted: "#63635E"
  surface-container-low: "#FDFDFC"
  surface-container: "#F1F0EF"
  surface-container-high: "#E9E8E6"
  outline: "#E9E8E6"
  outline-variant: "#CFCECA"
  primary: "#21201C"
  on-primary: "#FDFDFC"
  secondary: "#7D1B0C"
typography:
  headline-display:
    fontFamily: Newsreader
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: ui-serif
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.12
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Newsreader
    fontSize: 25px
    fontWeight: 500
    lineHeight: 1.15
  headline-sm:
    fontFamily: Georgia
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.035em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.02em
  body-lg:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.42
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.01em
  label-md:
    fontFamily: sans-serif
    fontSize: 15.5px
    fontWeight: 600
    lineHeight: 1.2
  label-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: -0.01em
  headline-md-mobile:
    fontFamily: Newsreader
    fontSize: 26.5px
    fontWeight: 500
    lineHeight: 1.15
rounded:
  sm: 6px
  md: 8px
  lg: 10px
  full: 9999px
spacing:
  xs: 4px
  sm: 7px
  md: 12px
  lg: 20px
  xl: 48px
  gutter: 10px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: 40px
    padding: 10px 20px
    height: 44px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 8px 14px
    height: 44px
  button-outline-hover:
    backgroundColor: "{colors.background}"
  button-secondary:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 8px 14px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: 12px
    padding: 0px
  link:
    textColor: "#FFECE2BD"
---

# Loops Design System

## Overview

Loops describes itself as: “Loops is the email platform for SaaS teams and their agents. Send marketing, product, and transactional email from one contact record. Start for free.” The interface is light, built on **Snow (#F9F9F8)** with **Charcoal (#21201C)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Newsreader** and **ui-serif**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [loops.so](https://loops.so/) on November 4, 2026 at 1440×900 and 390×844 from 403 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Snow (#F9F9F8):** Page background, seen 21 times. Token `background`.
- **Charcoal (#21201C):** Primary text and headings, seen 67 times. Token `on-surface`.
- **Graphite (#44433F):** Secondary text, seen 7 times. Token `on-surface-variant`.
- **Slate (#63635E):** Muted text and metadata, seen 35 times. Token `on-surface-muted`.
- **Snow (#FDFDFC):** Raised areas one step from the page, seen 40 times. Token `surface-container-low`.
- **Mist (#F1F0EF):** Cards and panels, seen 6 times. Token `surface-container`.
- **Mist (#E9E8E6):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Mist (#E9E8E6):** Borders and dividers, seen 51 times. Token `outline`.
- **Silver (#CFCECA):** Secondary dividers, seen 5 times. Token `outline-variant`.
- **Charcoal (#21201C):** Primary buttons and calls to action, seen 96 times. Token `primary`.
- **Snow (#FDFDFC):** Text and icons on primary. Token `on-primary`.
- **Dark Red (#7D1B0C):** Accent, seen 7 times. Token `secondary`, CSS `--laod-ox`.

## Typography

**Newsreader**, **ui-serif**, **Georgia**, **Inter**, **system-ui** and **sans-serif** share the interface. Fallback stack: `Newsreader, Newsreader Placeholder, serif`. Other loaded fonts: Inter Placeholder.

- **headline-display:** Newsreader 44px at weight 500, line height 1.08, tracking -0.02em. Page title (h1).
- **headline-lg:** ui-serif 30px at weight 400, line height 1.12, tracking -0.02em. Section headings (h2).
- **headline-md:** Newsreader 25px at weight 500, line height 1.15 (26.5px on mobile). Sub-section headings.
- **headline-sm:** Georgia 22px at weight 400, line height 1.1, tracking -0.035em. Card and feature titles.
- **body-md:** Inter 14px at weight 400, line height 1.5, tracking -0.02em. Body text.
- **body-lg:** system-ui 16px at weight 400, line height 1.3. Lead paragraphs.
- **body-sm:** Inter 12px at weight 400, line height 1.42. Secondary and small text.
- **label-lg:** Inter 16px at weight 500, line height 1.5, tracking 0.01em. Large buttons and tabs.
- **label-md:** sans-serif 15.5px at weight 600, line height 1.2. Buttons, navigation and labels.
- **label-sm:** Inter 13px at weight 500, line height 1.4, tracking -0.01em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 42% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 7px, md 12px, lg 20px, xl 48px.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Breakpoints:** 359.98px, 499px, 499.98px, 500px, 649.98px, 650px, 809px, 809.98px, 810px, 1199px, 1199.98px, 1200px, 1299.98px, 1599.98px, 1600px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.04) 0px 1px 2px 0px`
- `rgba(28, 25, 23, 0.055) 0px 2px 6px 0px`
- `rgba(33, 32, 28, 0.04) 0px 1px 2px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **lg (10px):** 108 elements.
- **full (9999px):** 108 elements.
- **sm (6px):** 68 elements.
- **md (8px):** 36 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for free”):** #21201C fill, #FDFDFC text, 12px/400, 40px radius, padding 10px 20px, shadow `rgba(255, 255, 255, 0.05) 0px 1px 2px 0px inset, rgba(28, 25, 23, 0.14) 0px 2px 5px 0px, rgba(28, 25, 23, 0.3) 0px 8px 18px -12px`.
- **button-outline (“Book a demo”):** #FDFDFC fill, #21201C text, 12px/400, 999px radius, padding 8px 14px, border 1px solid #DAD9D6.
- **button-outline-hover:** background #F9F9F8, text #21201C on hover.
- **button-secondary (“Start for free”):** transparent fill, #FDFDFC text, 12px/400, 999px radius, padding 8px 14px, shadow `color(srgb 0.992157 0.992157 0.988235 / 0.04) 0px 1px 2px 0px inset, color(srgb 0.129412 0.12549 0.109804 / 0.12) 0px 2px 5px 0px`.
- **button-ghost (“Framer · Customer since Dec 2022”):** transparent fill, #63635E text, 12px/400, padding 0px.
- **card:** #FDFDFC fill, #21201C text, 12px/400, 12px radius, padding 0px, border 1px solid #E9E8E6, shadow `rgba(33, 32, 28, 0.04) 0px 1px 2px 0px`.
- **link:** transparent fill, #FFECE2BD text, padding 0px.

## Do's and Don'ts

- Do use #F9F9F8 for the page and lift surfaces in small steps: #FDFDFC, #F1F0EF, #E9E8E6.
- Do keep text in 3 levels: #21201C, #44433F, #63635E.
- Do let contrast carry emphasis; primary actions use #21201C on #F9F9F8.
- Do set headlines in Newsreader with tight tracking (-0.02em).
- Do reuse the measured spacing steps (7px, 12px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 10px corners.
- Don't introduce new font families beyond Newsreader, ui-serif, Georgia, Inter, system-ui and sans-serif.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.42s.

## Motion

Interface transitions are quick: 0.15s, 0.16s, 0.22s, 0.18s.

- **Easing:** `ease`, `linear`, `cubic-bezier(0.12, 0.23, 0.5, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/loops.so/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
