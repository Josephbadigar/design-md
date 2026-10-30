---
version: alpha
name: Family
description: "Light interface measured from family.co: Family type with Inter, vivid blue accents, tonal surfaces and 12px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#474645"
  on-background: "#474645"
  on-surface-strong: "#121212"
  on-surface-variant: "#343433"
  on-surface-muted: "#7E7D7C"
  surface-container-low: "#FBFAF9"
  surface-container: "#F6F4EF"
  primary: "#0090FF"
  on-primary: "#000000"
  inverse-surface: "#171717"
  secondary: "#FFCD6C"
  tertiary: "#64C6FF"
  warning: "#D48F00"
  error: "#FF3E00"
  success: "#00C978"
typography:
  headline-display:
    fontFamily: Family
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.09
    letterSpacing: -0.031em
  headline-lg:
    fontFamily: Inter
    fontSize: 23px
    fontWeight: 500
    lineHeight: 1.09
    letterSpacing: -0.019em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
  body-lg:
    fontFamily: Inter
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.53
    letterSpacing: -0.013em
  body-sm:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.47
    letterSpacing: -0.009em
  caption:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: -0.006em
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
  label-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.47
    letterSpacing: -0.009em
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
    letterSpacing: -0.006em
  headline-display-mobile:
    fontFamily: Family
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.09
    letterSpacing: -0.022em
rounded:
  sm: 6px
  md: 12px
  lg: 32px
spacing:
  xs: 2px
  sm: 6px
  md: 12px
  lg: 32px
  xl: 58px
  gutter: 15px
  section: 96px
components:
  button-primary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px 14px
    height: 32px
  button-primary-hover:
    backgroundColor: "{colors.on-surface-strong}"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 0px
    height: 32px
  button-outline-hover:
    backgroundColor: "#EAE6DD"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "#22222266"
---

# Family Design System

## Overview

Family describes itself as: “Your favorite crypto wallet.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#474645)** text, and **Vivid Blue (#0090FF)** as the main accent.

Type is set in **Family** and **Inter**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 12px.

Measured from [family.co](https://family.co/) on October 29, 2026 at 1440×900 and 390×844 from 396 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`.
- **Graphite (#474645):** Primary text and headings, seen 25 times. Token `on-surface`.
- **Charcoal (#121212):** Headings and emphasis, seen 36 times. Token `on-surface-strong`.
- **Graphite (#343433):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Slate (#7E7D7C):** Muted text and metadata, seen 5 times. Token `on-surface-muted`.
- **Snow (#FBFAF9):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Warm Mist (#F6F4EF):** Cards and panels, seen 2 times. Token `surface-container`.
- **Vivid Blue (#0090FF):** Main accent color, seen 1 time. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#171717):** High-contrast fills, seen 2 times. Token `inverse-surface`.
- **Light Orange (#FFCD6C):** Accent in the logo, seen 22 times. Token `secondary`.
- **Blue (#64C6FF):** Accent on large areas, seen 11 times. Token `tertiary`.
- **Amber (#D48F00):** Warnings and highlights, seen 7 times. Token `warning`.
- **Vivid Red (#FF3E00):** Errors and destructive states, seen 5 times. Token `error`.
- **Teal (#00C978):** Success and positive states, seen 4 times. Token `success`.

## Typography

**Family** and **Inter** share the interface. Fallback stack: `Family, -apple-system, BlinkMacSystemFont, Segoe UI`. Other loaded fonts: LFE Sans.

- **headline-display:** Family 44px at weight 500, line height 1.09, tracking -0.031em (32px on mobile). Page title (h1).
- **headline-lg:** Inter 23px at weight 500, line height 1.09, tracking -0.019em. Section headings (h2).
- **body-md:** Inter 16px at weight 400. Body text.
- **body-lg:** Inter 17px at weight 400, line height 1.53, tracking -0.013em. Lead paragraphs.
- **body-sm:** Inter 15px at weight 400, line height 1.47, tracking -0.009em. Secondary and small text.
- **caption:** Inter 14px at weight 400, line height 1.43, tracking -0.006em. Captions and fine print.
- **label-lg:** Inter 16px at weight 500. Large buttons and tabs.
- **label-md:** Inter 15px at weight 500, line height 1.47, tracking -0.009em. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 600, line height 1.43, tracking -0.006em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 51% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 12px, lg 32px, xl 58px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 15px is the most common gap in flex and grid layouts.
- **Breakpoints:** 390px, 410px, 420px, 580px, 720px, 768px, 880px, 920px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#FBFAF9 → #F6F4EF) and hairline rings:

- `color(display-p3 0.94902 0.941176 0.929412) 0px 0px 0px 0px inset`

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **md (12px):** 20 elements.
- **sm (6px):** 16 elements.
- **lg (32px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #171717 fill, #FFFFFF text, 15px/500, 32px radius, padding 0px 14px.
- **button-primary-hover:** background #121212, text #FFFFFF on hover.
- **button-outline (“Log In”):** #F6F4EF fill, #121212 text, 16px/500, 32px radius, padding 0px.
- **button-outline-hover:** background #EAE6DD, text #121212 on hover.
- **button-ghost (“Log In”):** transparent fill, #474645 text, 16px/500, padding 0px.
- **link:** transparent fill, #22222266 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FBFAF9, #F6F4EF.
- Do keep text in 4 levels: #474645, #121212, #343433, #7E7D7C.
- Do reserve #0090FF for primary actions and key highlights.
- Do set headlines in Family with tight tracking (-0.031em).
- Do reuse the measured spacing steps (6px, 12px, 32px).
- Do use 12px corners on most elements; larger surfaces also use 6px and 32px.
- Don't use #7E7D7C for body text; it reaches 4.11:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Family and Inter.
- Don't use #0090FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.1s.

- **Easing:** `ease-out`, `ease-in-out`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/family.co/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
