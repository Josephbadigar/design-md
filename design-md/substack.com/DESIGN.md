---
version: alpha
name: Substack
description: "Dark interface measured from substack.com: Cahuenga type with system-ui, vivid orange accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#161718"
  surface: "#161718"
  on-surface: "#EEEEEE"
  on-background: "#EEEEEE"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#777777"
  surface-container-low: "#1B1C1D"
  surface-container: "#232525"
  surface-container-high: "#363737"
  overlay: "#282828BF"
  outline: "#FFFFFF1A"
  primary: "#FF6719"
  on-primary: "#FFFFFF"
  secondary: "#2F6D5D"
  tertiary: "#EB5757"
  link: "#18A0FB"
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
  lg: 20px
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
    backgroundColor: "#FF853D"
  button-secondary:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
    height: 40px
  button-secondary-hover:
    backgroundColor: "#5A5B5B"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 20px 0px 40px
  link:
    textColor: "{colors.link}"
---

# Substack Design System

## Overview

Substack describes itself as: “The app for independent voices” The interface is dark, built on **Charcoal (#161718)** with **Mist (#EEEEEE)** text, and **Vivid Orange (#FF6719)** as the main accent.

Type is set in **Cahuenga** and **system-ui**. Headlines run large; body text is 19px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [substack.com](https://substack.com/) on October 21, 2026 at 1440×900 and 390×844 from 243 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #6B4440BF.

- **Charcoal (#161718):** Page background, seen 8 times. Token `background`, CSS `--color-dark-bg-primary`.
- **Mist (#EEEEEE):** Primary text and headings, seen 22 times. Token `on-surface`, CSS `--color-light-bg-secondary`.
- **White (#FFFFFF):** Headings and emphasis, seen 7 times. Token `on-surface-strong`, CSS `--color-light-semantic-paid-utility-contrast`.
- **Slate (#777777):** Secondary text, seen 9 times. Token `on-surface-variant`, CSS `--color-light-button-quaternary-outline-fg`.
- **Charcoal (#1B1C1D):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Graphite (#232525):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--color-bg-secondary-hover-themed`.
- **Graphite (#363737):** Hover and pressed fills, seen 1 time. Token `surface-container-high`, CSS `--color-bg-elevated-tertiary`.
- **Graphite 75% (#282828BF):** Translucent fill for cards and controls, seen 1 time. Token `overlay`, CSS `--material-dark-regular`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 1 time. Token `outline`.
- **Vivid Orange (#FF6719):** Primary buttons and calls to action, seen 18 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Teal (#2F6D5D):** Brand color on large areas, seen 30 times. Token `secondary`.
- **Red (#EB5757):** Brand accent (CSS variable), seen 24 times. Token `tertiary`.
- **Vivid Blue (#18A0FB):** Inline links, seen 1 time. Token `link`.

## Typography

**Cahuenga** and **system-ui** share the interface. Fallback stack: `Cahuenga, serif`.

- **headline-display:** Cahuenga 32px at weight 500, line height 1.24. Page title (h1).
- **headline-lg:** Cahuenga 24px at weight 500, line height 1.25. Section headings (h2).
- **body-md:** system-ui 19px at weight 400. Body text.
- **body-sm:** system-ui 13px at weight 400, line height 1.31. Secondary and small text.
- **label-md:** system-ui 15px at weight 400, line height 1.33. Buttons, navigation and labels.
- **label-sm:** system-ui 13px at weight 600, line height 1.54. Small labels and badges.

## Layout

Spacing follows a 4px grid: 93% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#1B1C1D → #232525 → #363737):

- `rgba(255, 255, 255, 0.2) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.1) 0px -1px 0px 0px inset`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0.2) 0px 4px 6px -1px, rgba(0, 0, 0, 0.12) 0px 2px 4px -1px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 132 elements.
- **sm (8px):** 96 elements.
- **md (12px):** 36 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Create”):** #FF6719 fill, #FFFFFF text, 15px/600, 8px radius, padding 0px 16px, shadow `rgba(255, 255, 255, 0.2) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.1) 0px -1px 0px 0px inset`.
- **button-primary-hover:** background #FF853D, text #FFFFFF on hover.
- **button-secondary (“Sign in”):** #363737 fill, #EEEEEE text, 15px/600, 8px radius, padding 0px 16px.
- **button-secondary-hover:** background #5A5B5B, text #EEEEEE on hover.
- **button-outline (“Get app”):** #1B1C1D fill, #EEEEEE text, 15px/600, 8px radius, padding 0px 16px, shadow `rgba(0, 0, 0, 0.2) 0px 4px 6px -1px, rgba(0, 0, 0, 0.12) 0px 2px 4px -1px`.
- **button-ghost (“Learn more”):** transparent fill, #FFFFFF text, 15px/600, 8px radius, padding 0px 16px.
- **input-field (“Search Substack”):** #1B1C1D fill, #EEEEEE text, 15px/400, 12px radius, padding 0px 20px 0px 40px, border 1px solid #FFFFFF1A.
- **link:** transparent fill, #18A0FB text, padding 0px.

## Do's and Don'ts

- Do use #161718 for the page and lift surfaces in small steps: #1B1C1D, #232525, #363737.
- Do keep text in 3 levels: #EEEEEE, #FFFFFF, #777777.
- Do reserve #FF6719 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't use #777777 for body text; it reaches 4.0:1 on #161718. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Cahuenga and system-ui.
- Don't use #FF6719 for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.25s.

- **Easing:** `cubic-bezier(0.19, 1, 0.22, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/substack.com/), the free DESIGN.md generator.
