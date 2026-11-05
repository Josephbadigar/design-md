---
version: alpha
name: Semantic UI
description: "Light monochrome interface measured from semantic-ui.com: Lato type, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#212121"
  on-background: "#212121"
  on-surface-variant: "#666666"
  on-surface-muted: "#858188"
  on-surface-subtle: "#8D8A8A"
  surface-container-low: "#F3F4F5"
  surface-container: "#E8E8E8"
  surface-container-high: "#E0E1E2"
  overlay: "#0000000D"
  overlay-strong: "#2224261A"
  outline: "#22242626"
  outline-variant: "#D4D4D5"
  primary: "#1B1C1D"
  on-primary: "#FFFFFF"
  secondary: "#4183C4"
  tertiary: "#008C79"
  warning: "#573A08"
typography:
  headline-display:
    fontFamily: Lato
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.29
  headline-lg:
    fontFamily: Lato
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.29
  headline-md:
    fontFamily: Lato
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.29
  body-md:
    fontFamily: Lato
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Lato
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.29
  label-lg:
    fontFamily: Lato
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1
  label-md:
    fontFamily: Lato
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.29
  label-sm:
    fontFamily: Lato
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Lato
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.29
rounded:
  sm: 2px
  md: 4px
spacing:
  xs: 3px
  sm: 7px
  md: 14px
  lg: 18px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: 7px 10px
    height: 26px
  button-primary-hover:
    backgroundColor: "#27292A"
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.headline-md}"
    rounded: "{rounded.md}"
    padding: 15.71px 30px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "#000000"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 7px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.secondary}"
---

# Semantic UI Design System

## Overview

Semantic UI describes itself as: “Semantic empowers designers and developers by creating a shared vocabulary for UI.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#212121)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Lato**. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [semantic-ui.com](https://semantic-ui.com/) on November 4, 2026 at 1440×900 and 390×844 from 219 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles.

- **White (#FFFFFF):** Page background, seen 12 times. Token `background`.
- **Charcoal (#212121):** Primary text and headings. Token `on-surface`.
- **Slate (#666666):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Cool Gray (#858188):** Muted text and metadata, seen 52 times. Token `on-surface-muted`.
- **Gray (#8D8A8A):** Subtle text and placeholders, seen 15 times. Token `on-surface-subtle`.
- **Snow (#F3F4F5):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Mist (#E8E8E8):** Cards and panels, seen 4 times. Token `surface-container`.
- **Mist (#E0E1E2):** Hover and pressed fills, seen 4 times. Token `surface-container-high`.
- **Near Black 5% (#0000000D):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Graphite 10% (#2224261A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Graphite 15% (#22242626):** Borders and dividers, seen 9 times. Token `outline`.
- **Silver (#D4D4D5):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Charcoal (#1B1C1D):** Primary buttons and calls to action, seen 9 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#4183C4):** Accent in text, fills and borders, seen 22 times. Token `secondary`.
- **Dark Teal (#008C79):** Accent in text, fills and borders, seen 21 times. Token `tertiary`.
- **Deep Orange (#573A08):** Warnings and highlights, seen 4 times. Token `warning`.

## Typography

**Lato** carries the whole interface. Fallback stack: `Lato, Helvetica Neue, Arial, Helvetica`. Other loaded fonts: Icons, Accordion, Checkbox, Dropdown.

- **headline-display:** Lato 40px at weight 400, line height 1.29 (32px on mobile). Page title (h1).
- **headline-lg:** Lato 26px at weight 400, line height 1.29. Section headings (h2).
- **headline-md:** Lato 20px at weight 400, line height 1.29. Sub-section headings.
- **body-md:** Lato 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Lato 18px at weight 700, line height 1.29. Lead paragraphs.
- **label-lg:** Lato 16px at weight 700, line height 1. Large buttons and tabs.
- **label-md:** Lato 15px at weight 700, line height 1.29. Buttons, navigation and labels.
- **label-sm:** Lato 14px at weight 700, line height 1. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 34% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 7px, md 14px, lg 18px.
- **Breakpoints:** 320px, 400px, 500px, 767px, 768px, 820px, 991px, 992px, 1144px, 1145px, 1199px, 1200px, 1272px, 1500px, 1919px, 1920px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#F3F4F5 → #E8E8E8 → #E0E1E2):

- `rgba(34, 36, 38, 0.15) 0px 0px 0px 0px inset`
- `rgba(0, 0, 0, 0) 0px 0px 0px 1px inset, rgba(34, 36, 38, 0.15) 0px 0px 0px 0px inset`
- `rgb(255, 255, 255) 0px 0px 0px 2px inset`

A few raised panels add a soft drop shadow: `rgba(34, 36, 38, 0.15) 0px 1px 2px 0px`.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 102 elements.
- **sm (2px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“2.5.0”):** #1B1C1D fill, #FFFFFF text, 12px/700, 4px radius, padding 7px 10px.
- **button-primary-hover:** background #27292A, text #FFFFFF on hover.
- **button-ghost (“Get Started”):** transparent fill, #FFFFFF text, 20px/700, 4px radius, padding 15.71px 30px, shadow `rgb(255, 255, 255) 0px 0px 0px 2px inset`.
- **input-field:** #FFFFFF fill, #000000 text, 14px/400, 2px radius, padding 7px, border 1px solid #22242626.
- **card:** #FFFFFF fill, #000000DE text, 14px/400, 4px radius, padding 0px, shadow `rgb(212, 212, 213) 0px 1px 3px 0px, rgb(212, 212, 213) 0px 0px 0px 1px`.
- **link:** transparent fill, #4183C4 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F3F4F5, #E8E8E8, #E0E1E2.
- Do keep text in 4 levels: #212121, #666666, #858188, #8D8A8A.
- Do let contrast carry emphasis; primary actions use #1B1C1D on #FFFFFF.
- Do reuse the measured spacing steps (7px, 14px, 18px).
- Do use 4px corners on most elements; larger surfaces also use 2px.
- Don't use #858188 for body text; it reaches 3.82:1 on #FFFFFF. Keep it for large text or metadata.
- Don't use #8D8A8A for body text; it reaches 3.42:1 on #FFFFFF. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Lato.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.1s, 0.5s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/semantic-ui.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
