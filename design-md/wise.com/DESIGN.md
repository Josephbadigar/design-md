---
version: alpha
name: Wise
description: "Light interface measured from wise.com: Wise Sans type with Inter, deep lime accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#9FE870"
  surface: "#9FE870"
  on-surface: "#163300"
  on-background: "#163300"
  on-surface-strong: "#0E0F0C"
  on-surface-variant: "#454745"
  surface-container-low: "#FFFFFF"
  overlay: "#16330014"
  overlay-strong: "#3E3B0712"
  outline: "#0E0F0C1F"
  primary: "#163300"
  on-primary: "#9FE870"
  secondary: "#054D28"
  tertiary: "#B8232B"
  success: "#9FE870"
typography:
  headline-display:
    fontFamily: Wise Sans
    fontSize: 88.5px
    fontWeight: 900
    lineHeight: 0.85
  headline-lg:
    fontFamily: Wise Sans
    fontSize: 58px
    fontWeight: 900
    lineHeight: 0.85
  headline-md:
    fontFamily: Wise Sans
    fontSize: 52px
    fontWeight: 400
    lineHeight: 1.5
  headline-sm:
    fontFamily: Inter
    fontSize: 45px
    fontWeight: 600
    lineHeight: 1.27
    letterSpacing: -0.03em
  title-lg:
    fontFamily: Wise Sans
    fontSize: 40px
    fontWeight: 900
    lineHeight: 0.85
  body-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.44
    letterSpacing: -0.006em
  body-lg:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: 0.005em
  body-sm:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.005em
  caption:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: -0.006em
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: 0.005em
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.55
    letterSpacing: -0.006em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Wise Sans
    fontSize: 45px
    fontWeight: 900
    lineHeight: 0.85
rounded:
  md: 2px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 9.38px
  lg: 24px
  xl: 48px
  gutter: 12px
  section: 56.31px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 8px 12px
    height: 32px
  button-primary-hover:
    backgroundColor: "#0D1F00"
    textColor: "#BBEF9A"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.caption}"
    rounded: "{rounded.full}"
    padding: 12px 16px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 8px 12px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-md}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: 28.15px
    padding: 37.54px 28.15px
  link:
    textColor: "{colors.primary}"
---

# Wise Design System

## Overview

Wise describes itself as: “Banks charge a lot for overseas transfers. We don't. Transfer money abroad easily and quickly with our low cost money transfers.” The interface is light, built on **Green (#9FE870)** with **Deep Lime (#163300)** text, and **Deep Lime (#163300)** as the main accent.

Type is set in **Wise Sans** and **Inter**. Headlines run large; body text is 18px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [wise.com](https://wise.com/) on October 29, 2026 at 1440×900 and 390×844 from 432 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Green (#9FE870):** Page background, seen 14 times. Token `background`.
- **Deep Lime (#163300):** Primary text and headings, seen 76 times. Token `on-surface`.
- **Charcoal (#0E0F0C):** Headings and emphasis, seen 30 times. Token `on-surface-strong`, CSS `--color-content-link-active`.
- **Graphite (#454745):** Secondary text, seen 10 times. Token `on-surface-variant`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 14 times. Token `surface-container-low`, CSS `--color-white`.
- **Deep Lime 8% (#16330014):** Translucent fill for cards and controls, seen 8 times. Token `overlay`.
- **Deep Yellow 7% (#3E3B0712):** Stronger translucent fill, seen 5 times. Token `overlay-strong`.
- **Charcoal 12% (#0E0F0C1F):** Borders and dividers, seen 1 time. Token `outline`.
- **Deep Lime (#163300):** Primary buttons and calls to action, seen 103 times. Token `primary`.
- **Green (#9FE870):** Text and icons on primary. Token `on-primary`.
- **Deep Green (#054D28):** Accent (CSS variable), seen 5 times. Token `secondary`, CSS `--color-sentiment-positive-primary`.
- **Red (#B8232B):** Accent (CSS variable). Token `tertiary`.
- **Green (#9FE870):** Success and positive states, seen 38 times. Token `success`.

## Typography

**Wise Sans** and **Inter** share the interface. Fallback stack: `Wise Sans, Inter, sans-serif`.

- **headline-display:** Wise Sans 88.5px at weight 900, line height 0.85 (45px on mobile). Page title (h1).
- **headline-lg:** Wise Sans 58px at weight 900, line height 0.85. Section headings (h2).
- **headline-md:** Wise Sans 52px at weight 400, line height 1.5. Sub-section headings.
- **headline-sm:** Inter 45px at weight 600, line height 1.27, tracking -0.03em. Card and feature titles.
- **title-lg:** Wise Sans 40px at weight 900, line height 0.85. Small titles.
- **body-md:** Inter 18px at weight 400, line height 1.44, tracking -0.006em. Body text.
- **body-lg:** Inter 20px at weight 600, line height 1.4, tracking 0.005em. Lead paragraphs.
- **body-sm:** Inter 16px at weight 400, line height 1.5, tracking 0.005em. Secondary and small text.
- **caption:** Inter 14px at weight 400, line height 1.55, tracking -0.006em. Captions and fine print.
- **label-lg:** Inter 16px at weight 600, line height 1.5, tracking 0.005em. Large buttons and tabs.
- **label-md:** Inter 14px at weight 600, line height 1.55, tracking -0.006em. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 600, line height 1. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 55% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 9.38px, lg 24px, xl 48px.
- **Sections:** 56.31px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 0px, 319.98px, 320px, 599.98px, 600px, 839.98px, 840px, 1159.98px, 1160px, 1279.98px, 1280px, 1439.98px, 1440px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#FFFFFF) and hairline rings:

- `rgb(134, 134, 133) 0px 0px 0px 1px inset`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (2px):** 208 elements.
- **full (9999px):** 196 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #163300 fill, #9FE870 text, 18px/600, 9999px radius, padding 8px 12px.
- **button-primary-hover:** background #0D1F00, text #BBEF9A on hover.
- **button-outline (“Send money”):** #9FE870 fill, #163300 text, 14px/400, 9999px radius, padding 12px 16px.
- **button-ghost (“Personal”):** transparent fill, #163300 text, 18px/400, 9999px radius, padding 8px 12px.
- **input-field (“0.00”):** transparent fill, #163300 text, 52px/400, padding 0px.
- **card:** #FFFFFF fill, #454745 text, 18px/400, 28.1539px radius, padding 37.54px 28.15px.
- **link:** transparent fill, #163300 text, padding 0px.

## Do's and Don'ts

- Do use #9FE870 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 3 levels: #163300, #0E0F0C, #454745.
- Do reserve #163300 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 9.38px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 2px corners.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Wise Sans and Inter.
- Don't use #163300 for large backgrounds or body text.
- Don't make interface transitions slower than 0.35s.

## Motion

Interface transitions are quick: 0.35s, 0.15s, 0.2s, 0.3s. Longer ambient animations run 1.5s, 1s, 2s.

- **Easing:** `ease`, `ease-in-out`, `cubic-bezier(0.8, 0.05, 0.2, 0.95)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/wise.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
