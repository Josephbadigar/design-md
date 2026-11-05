---
version: alpha
name: Fluent 2
description: "Light monochrome interface measured from fluent2.microsoft.design: Segoe UI type, tonal surfaces and 2px corners."
colors:
  background: "#EEEBF0"
  surface: "#EEEBF0"
  on-surface: "#242424"
  on-background: "#242424"
  on-surface-strong: "#1B1A19"
  on-surface-variant: "#424242"
  on-surface-muted: "#616161"
  surface-container-low: "#F0F0F0"
  surface-container: "#F5F5F5"
  surface-container-high: "#FFFFFF"
  outline: "#D1D1D1"
  outline-variant: "#6161615E"
  primary: "#242424"
  on-primary: "#FFFFFF"
  inverse-surface: "#000000"
  secondary: "#D13438"
  tertiary: "#C43857"
typography:
  headline-display:
    fontFamily: Segoe UI
    fontSize: 128px
    fontWeight: 400
    lineHeight: 1
  headline-lg:
    fontFamily: Segoe UI
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.3
  headline-md:
    fontFamily: Segoe UI
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
  body-md:
    fontFamily: Segoe UI
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.15
  body-sm:
    fontFamily: Segoe UI
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  caption:
    fontFamily: Segoe UI
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: Segoe UI
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.38
  label-sm:
    fontFamily: Segoe UI
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.15
rounded:
  xs: 2px
  sm: 4px
  md: 8px
  lg: 20px
  xl: 22px
spacing:
  xs: 4px
  sm: 8px
  md: 14px
  lg: 32px
  xl: 38px
  gutter: 11px
  section: 60px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: 12px
    padding: 5px 12px
    height: 32px
  button-primary-hover:
    backgroundColor: "{colors.on-surface-variant}"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#BDBDBD"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 5px 12px
    height: 32px
  button-ghost:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 5px 12px
    height: 32px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px 0px 0px 12px
  card:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "#0000EE"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 32px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Fluent 2 Design System

## Overview

Fluent 2 describes itself as: “Explore the next evolution of Microsoft’s design system, enabling more seamless collaboration and creativity than ever. Move fluidly from design to development, between apps, and across platforms.” The interface is light, built on **Mist (#EEEBF0)** with **Graphite (#242424)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Segoe UI**. Headlines run large; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 2px.

Measured from [fluent2.microsoft.design](https://fluent2.microsoft.design/) on November 4, 2026 at 1440×900 and 390×844 from 145 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles, plus gradient stops #0F6CBD.

- **Mist (#EEEBF0):** Page background, seen 1 time. Token `background`.
- **Graphite (#242424):** Primary text and headings, seen 28 times. Token `on-surface`.
- **Charcoal (#1B1A19):** Headings and emphasis, seen 8 times. Token `on-surface-strong`.
- **Graphite (#424242):** Secondary text, seen 7 times. Token `on-surface-variant`.
- **Slate (#616161):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Mist (#F0F0F0):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#F5F5F5):** Cards and panels, seen 2 times. Token `surface-container`.
- **White (#FFFFFF):** Hover and pressed fills, seen 11 times. Token `surface-container-high`, CSS `--colorNeutralForegroundOnBrand`.
- **Silver (#D1D1D1):** Borders and dividers, seen 3 times. Token `outline`.
- **Slate 37% (#6161615E):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Graphite (#242424):** Primary buttons and calls to action, seen 41 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000000):** High-contrast fills, seen 1 time. Token `inverse-surface`, CSS `--colorStrokeFocus2`.
- **Red (#D13438):** Accent in text, fills and borders, seen 2 times. Token `secondary`, CSS `--colorPaletteRedForeground3`.
- **Red (#C43857):** Accent in text, fills and borders, seen 2 times. Token `tertiary`.

## Typography

**Segoe UI** carries the whole interface. Fallback stack: `Segoe UI, Segoe UI Web (West European), -apple-system, BlinkMacSystemFont`.

- **headline-display:** Segoe UI 128px at weight 400, line height 1. Page title (h1).
- **headline-lg:** Segoe UI 40px at weight 600, line height 1.3. Section headings (h2).
- **headline-md:** Segoe UI 24px at weight 600, line height 1.33. Sub-section headings.
- **body-md:** Segoe UI 18px at weight 400, line height 1.15. Body text.
- **body-sm:** Segoe UI 14px at weight 400, line height 1.43. Secondary and small text.
- **caption:** Segoe UI 12px at weight 400, line height 1.33. Captions and fine print.
- **label-md:** Segoe UI 16px at weight 600, line height 1.38. Buttons, navigation and labels.
- **label-sm:** Segoe UI 14px at weight 600, line height 1.15. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 47% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 14px, lg 32px, xl 38px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 11px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Breakpoints:** 440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.12) 0px 0px 2px 0px, rgba(0, 0, 0, 0.14) 0px 2px 4px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 2px inset`
- `rgba(0, 0, 0, 0.12) 0px 0px 2px 0px, rgba(0, 0, 0, 0.14) 0px 4px 8px 0px`
- `rgb(68, 68, 68) 0px 0px 4px -2px`

## Shapes

Most elements use 2px corners. Measured radii, most used first:

- **xs (2px):** 72 elements.
- **md (8px):** 36 elements.
- **sm (4px):** 24 elements.
- **xl (22px):** 24 elements.
- **lg (20px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Employee sign-in”):** #242424 fill, #FFFFFF text, 14px/600, 12px radius, padding 5px 12px.
- **button-primary-hover:** background #424242, text #FFFFFF on hover.
- **button-outline (“Submit”):** #F0F0F0 fill, #BDBDBD text, 14px/600, 4px radius, padding 5px 12px.
- **button-ghost (“Cancel”):** #FFFFFF fill, #242424 text, 14px/600, 4px radius, padding 5px 12px, border 1px solid #D1D1D1.
- **input-field (“- Please choose -”):** transparent fill, #242424 text, 14px/400, padding 0px 0px 0px 12px.
- **card:** #FFFFFF fill, #0000EE text, 18px/400, 22px radius, padding 32px, shadow `rgba(0, 0, 0, 0.12) 0px 0px 2px 0px, rgba(0, 0, 0, 0.14) 0px 2px 4px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 2px inset`.
- **link:** transparent fill, #616161 text, padding 0px.

## Do's and Don'ts

- Do use #EEEBF0 for the page and lift surfaces in small steps: #F0F0F0, #F5F5F5, #FFFFFF.
- Do keep text in 4 levels: #242424, #1B1A19, #424242, #616161.
- Do let contrast carry emphasis; primary actions use #242424 on #EEEBF0.
- Do reuse the measured spacing steps (8px, 14px, 32px).
- Do use 2px corners on most elements; larger surfaces also use 8px, 4px and 22px.
- Don't introduce new font families beyond Segoe UI.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.1s, 0.3s, 0.15s, 0.25s. Longer ambient animations run 1.5s.

- **Easing:** `ease-in-out`, `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/fluent2.microsoft.design/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
