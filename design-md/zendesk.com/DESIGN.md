---
version: alpha
name: Zendesk
description: "Dark interface measured from zendesk.com: Vanilla Sans type, lime accents, tonal surfaces and 4px corners."
colors:
  background: "#11110D"
  surface: "#11110D"
  on-surface: "#F5F5F2"
  on-background: "#F5F5F2"
  on-surface-strong: "#FFFFFF"
  surface-container-low: "#203524"
  overlay: "#11110D1C"
  overlay-strong: "#11110D0D"
  outline: "#11110D52"
  outline-variant: "#FFFFFF1A"
  primary: "#D1F470"
  on-primary: "#11110D"
  secondary: "#775427"
  tertiary: "#70A32A"
typography:
  headline-display:
    fontFamily: Vanilla Sans
    fontSize: 42px
    fontWeight: 500
    lineHeight: 1.15
  headline-lg:
    fontFamily: Vanilla Sans
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1
  headline-md:
    fontFamily: Vanilla Sans
    fontSize: 26px
    fontWeight: 500
    lineHeight: 1.25
  body-md:
    fontFamily: Vanilla Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.45
  body-lg:
    fontFamily: Vanilla Sans
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.56
  body-sm:
    fontFamily: Vanilla Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Vanilla Sans
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.45
  label-sm:
    fontFamily: Vanilla Sans
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: 0.054em
  headline-display-mobile:
    fontFamily: Vanilla Sans
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.15
  headline-md-mobile:
    fontFamily: Vanilla Sans
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.25
rounded:
  sm: 4px
  md: 8px
  lg: 16px
spacing:
  xs: 2.4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 48px
  gutter: 8px
  section: 88px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 10px 16px
    height: 43px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    padding: 0px
    height: 64px
  button-secondary:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    padding: 9px
    height: 42px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 20px 0px
  input-field:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.on-primary}"
    rounded: 12px
    padding: 12px
  link:
    textColor: "{colors.on-surface-strong}"
---

# Zendesk Design System

## Overview

Zendesk describes itself as: “Move beyond deflection with AI agents that resolve issues end-to-end. Improve service quality, speed, and scale. Start your free trial.” The interface is dark, built on **Charcoal (#11110D)** with **Mist (#F5F5F2)** text, and **Lime (#D1F470)** as the main accent.

Type is set in **Vanilla Sans**. Headlines run large; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [zendesk.com](https://www.zendesk.com/) on November 4, 2026 at 1440×900 and 390×844 from 412 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #2D4C33, #355E34.

- **Charcoal (#11110D):** Page background, seen 1 time. Token `background`.
- **Mist (#F5F5F2):** Primary text and headings, seen 23 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 7 times. Token `on-surface-strong`.
- **Deep Green (#203524):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Charcoal 11% (#11110D1C):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Charcoal 5% (#11110D0D):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Charcoal 32% (#11110D52):** Borders and dividers, seen 5 times. Token `outline`.
- **White 10% (#FFFFFF1A):** Secondary dividers, seen 4 times. Token `outline-variant`.
- **Lime (#D1F470):** Primary buttons and calls to action, seen 15 times. Token `primary`.
- **Charcoal (#11110D):** Text and icons on primary. Token `on-primary`.
- **Dark Orange (#775427):** Accent in logos and imagery. Token `secondary`.
- **Lime (#70A32A):** Accent in text, fills and borders, seen 55 times. Token `tertiary`.

## Typography

**Vanilla Sans** carries the whole interface. Fallback stack: `Vanilla Sans, Arial, sans-serif`.

- **headline-display:** Vanilla Sans 42px at weight 500, line height 1.15 (30px on mobile). Page title (h1).
- **headline-lg:** Vanilla Sans 40px at weight 500, line height 1. Section headings (h2).
- **headline-md:** Vanilla Sans 26px at weight 500, line height 1.25 (22px on mobile). Sub-section headings.
- **body-md:** Vanilla Sans 16px at weight 400, line height 1.45. Body text.
- **body-lg:** Vanilla Sans 18px at weight 600, line height 1.56. Lead paragraphs.
- **body-sm:** Vanilla Sans 14px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Vanilla Sans 16px at weight 600, line height 1.45. Buttons, navigation and labels.
- **label-sm:** Vanilla Sans 14px at weight 700, line height 1.3, tracking 0.054em, uppercase. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (83% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2.4px, sm 8px, md 16px, lg 20px, xl 48px.
- **Sections:** 88px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 0px, 480px, 480.98px, 481px, 767.98px, 768px, 969px, 970px, 1149px, 1149.98px, 1150px, 1165px, 1599.98px, 1600px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#203524) and hairline rings:

- `rgb(213, 213, 210) 0px 0px 0px 1px inset`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 240 elements.
- **lg (16px):** 124 elements.
- **md (8px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try for free”):** #D1F470 fill, #11110D text, 16px/600, 16px radius, padding 10px 16px.
- **button-outline (“Open chat”):** #11110D fill, #FFFFFF text, 13.3333px/400, 50% radius, padding 0px, shadow `rgba(23, 73, 77, 0.15) 0px 20px 30px 0px`.
- **button-secondary (“Pause animation”):** #FFFFFF fill, #11110D text, 16px/600, 100% radius, padding 9px.
- **button-ghost (“What is Zendesk?”):** transparent fill, #11110D text, 16px/600, padding 20px 0px.
- **input-field (“Enter work email”):** #FFFFFF fill, #11110D text, 15px/400, 12px radius, padding 12px, shadow `rgb(213, 213, 210) 0px 0px 0px 1px inset`.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #11110D for the page and lift surfaces in small steps: #203524.
- Do keep text in 2 levels: #F5F5F2, #FFFFFF.
- Do reserve #D1F470 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do use 4px corners on most elements; larger surfaces also use 16px and 8px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Vanilla Sans.
- Don't use #D1F470 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.1s, 0.6s, 0.3s, 0.25s.

- **Easing:** `linear`, `cubic-bezier(0.7, 0, 0.3, 1)`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/zendesk.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
