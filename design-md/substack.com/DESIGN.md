---
version: alpha
name: Substack
description: "Light interface measured from substack.com: Cahuenga type with system-ui, vivid orange accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#363737"
  on-background: "#363737"
  on-surface-variant: "#777777"
  outline: "#0000001A"
  primary: "#FF6719"
  on-primary: "#FFFFFF"
  inverse-surface: "#232525"
  secondary: "#2F6D5D"
  tertiary: "#EB5757"
  link: "#0083D5"
typography:
  headline-display:
    fontFamily: Cahuenga
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.24
  headline-lg:
    fontFamily: Cahuenga
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.25
  body-md:
    fontFamily: system-ui
    fontSize: 19px
    fontWeight: 400
  body-sm:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.31
  label-md:
    fontFamily: system-ui
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.33
  label-sm:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.54
rounded:
  sm: 8px
  md: 12px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  xl: 40px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
    height: 40px
  button-primary-hover:
    backgroundColor: "#D74D00"
  button-outline:
    backgroundColor: "#EEEEEE"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
    height: 40px
  button-outline-hover:
    backgroundColor: "#DBDBDB"
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 40px
  link:
    textColor: "{colors.link}"
---

# Substack Design System

## Overview

Substack describes itself as: “Substack is the app for independent voices: a free newsletter, video, and podcast hosting platform with paid subscriptions built in.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#363737)** text, and **Vivid Orange (#FF6719)** as the main accent.

Type is set in **Cahuenga** and **system-ui**. Headlines run large; body text is 19px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [substack.com](https://substack.com/) on October 29, 2026 at 1440×900 and 390×844 from 313 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles, plus gradient stops #593C34BF.

- **White (#FFFFFF):** Page background, seen 10 times. Token `background`, CSS `--color-light-semantic-paid-utility-contrast`.
- **Graphite (#363737):** Primary text and headings, seen 36 times. Token `on-surface`.
- **Slate (#777777):** Secondary text, seen 19 times. Token `on-surface-variant`, CSS `--color-light-button-quaternary-outline-fg`.
- **Near Black 10% (#0000001A):** Borders and dividers, seen 2 times. Token `outline`.
- **Vivid Orange (#FF6719):** Primary buttons and calls to action, seen 18 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Graphite (#232525):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Dark Teal (#2F6D5D):** Accent on large areas. Token `secondary`.
- **Red (#EB5757):** Accent (CSS variable). Token `tertiary`.
- **Blue (#0083D5):** Inline links, seen 3 times. Token `link`.

## Typography

**Cahuenga** and **system-ui** share the interface. Fallback stack: `Cahuenga, serif`.

- **headline-display:** Cahuenga 32px at weight 500, line height 1.24. Page title (h1).
- **headline-lg:** Cahuenga 24px at weight 500, line height 1.25. Section headings (h2).
- **body-md:** system-ui 19px at weight 400. Body text.
- **body-sm:** system-ui 13px at weight 400, line height 1.31. Secondary and small text.
- **label-md:** system-ui 15px at weight 400, line height 1.33. Buttons, navigation and labels.
- **label-sm:** system-ui 13px at weight 600, line height 1.54. Small labels and badges.

## Layout

Spacing follows a 4px grid: 91% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgba(255, 255, 255, 0.2) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.1) 0px -1px 0px 0px inset`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 172 elements.
- **sm (8px):** 108 elements.
- **md (12px):** 40 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Create”):** #FF6719 fill, #FFFFFF text, 15px/600, 8px radius, padding 0px 16px, shadow `rgba(255, 255, 255, 0.2) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.1) 0px -1px 0px 0px inset`.
- **button-primary-hover:** background #D74D00, text #FFFFFF on hover.
- **button-outline (“Sign in”):** #EEEEEE fill, #363737 text, 15px/600, 8px radius, padding 0px 16px.
- **button-outline-hover:** background #DBDBDB, text #363737 on hover.
- **button-ghost (“Learn more”):** transparent fill, #FFFFFF text, 15px/600, 8px radius, padding 0px 16px.
- **input-field (“Search Substack”):** #FFFFFF fill, #363737 text, 15px/400, 12px radius, padding 0px 40px, border 1px solid #0000001A.
- **link:** transparent fill, #0083D5 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #363737, #777777.
- Do reserve #FF6719 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't use #777777 for body text; it reaches 4.48:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond Cahuenga and system-ui.
- Don't use #FF6719 for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.25s.

- **Easing:** `cubic-bezier(0.19, 1, 0.22, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/substack.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
