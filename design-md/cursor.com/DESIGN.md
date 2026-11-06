---
version: alpha
name: Cursor
description: "Light interface measured from cursor.com: CursorGothic type with system-ui, vivid orange accents, tonal surfaces and 4px corners."
colors:
  background: "#F7F7F4"
  surface: "#F7F7F4"
  on-surface: "#26251E"
  on-background: "#26251E"
  on-surface-variant: "#7A7974"
  surface-container-low: "#F2F1ED"
  surface-container: "#EBEAE5"
  surface-container-high: "#E6E5E0"
  surface-container-highest: "#E1E0DB"
  overlay: "#26251E1A"
  overlay-strong: "#26251E33"
  outline: "#26251E06"
  outline-variant: "#26251E1A"
  primary: "#F54E00"
  on-primary: "#000000"
  secondary: "#C08532"
  tertiary: "#CF2D56"
  success: "#1F8A65"
typography:
  headline-display:
    fontFamily: CursorGothic
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.013em
  headline-lg:
    fontFamily: CursorGothic
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.005em
  body-md:
    fontFamily: CursorGothic
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.01em
  body-lg:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  caption:
    fontFamily: system-ui
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.27
    letterSpacing: 0.004em
  label-lg:
    fontFamily: CursorGothic
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.55
  label-sm:
    fontFamily: Lato
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1.27
    letterSpacing: 0.004em
  code:
    fontFamily: berkeleyMono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.67
  headline-display-mobile:
    fontFamily: CursorGothic
    fontSize: 24.5px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.013em
  headline-lg-mobile:
    fontFamily: CursorGothic
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.005em
rounded:
  sm: 4px
  md: 8px
  lg: 10px
  xl: 12px
  full: 9999px
spacing:
  xs: 2px
  sm: 6px
  md: 10px
  lg: 17.5px
  xl: 44.8px
  gutter: 8px
  section: 67.2px
  margin: 20px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    padding: 5.6px 10.5px 5.88px 10.5px
    height: 27px
  button-primary-hover:
    backgroundColor: "#3B3A33"
  button-outline:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    padding: 12.48px 21.6px 12.8px 21.6px
    height: 43px
  button-outline-hover:
    backgroundColor: "{colors.surface-container-highest}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    padding: 5.6px 10.5px 5.88px 10.5px
    height: 27px
  input-field:
    textColor: "{colors.on-surface}"
    rounded: 0px
    padding: 8px 8px 6px 8px
  link:
    textColor: "{colors.on-surface}"
---

# Cursor Design System

## Overview

Cursor describes itself as: “Built to make you extraordinarily productive, agents turn ideas into code. Accelerate development by handing off tasks to Cursor.” The interface is light, built on **Snow (#F7F7F4)** with **Warm Charcoal (#26251E)** text, and **Vivid Orange (#F54E00)** as the main accent.

Type is set in **CursorGothic** and **system-ui**, with **berkeleyMono** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [cursor.com](https://cursor.com/) on November 5, 2026 at 1440×900 and 390×844 from 442 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles.

- **Snow (#F7F7F4):** Page background, seen 14 times. Token `background`, CSS `--color-theme-product-editor`.
- **Warm Charcoal (#26251E):** Primary text and headings, seen 85 times. Token `on-surface`, CSS `--color-theme-button-bg`.
- **Warm Slate (#7A7974):** Secondary text, seen 16 times. Token `on-surface-variant`.
- **Mist (#F2F1ED):** Raised areas one step from the page, seen 34 times. Token `surface-container-low`.
- **Warm Mist (#EBEAE5):** Cards and panels, seen 9 times. Token `surface-container`.
- **Warm Mist (#E6E5E0):** Hover and pressed fills, seen 5 times. Token `surface-container-high`.
- **Warm Silver (#E1E0DB):** Highest raised elements, seen 4 times. Token `surface-container-highest`.
- **Warm Charcoal 10% (#26251E1A):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Warm Charcoal 20% (#26251E33):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Warm Charcoal 2% (#26251E06):** Borders and dividers, seen 36 times. Token `outline`.
- **Warm Charcoal 10% (#26251E1A):** Secondary dividers, seen 6 times. Token `outline-variant`.
- **Vivid Orange (#F54E00):** Brand accent (CSS variable), seen 7 times. Token `primary`, CSS `--color-accent`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Orange (#C08532):** Accent in text, fills and borders, seen 7 times. Token `secondary`.
- **Pink (#CF2D56):** Accent in text, fills and borders, seen 4 times. Token `tertiary`.
- **Dark Teal (#1F8A65):** Success and positive states, seen 5 times. Token `success`.

## Typography

**CursorGothic**, **system-ui**, **Lato** and **berkeleyMono** (monospace) share the interface. Fallback stack: `CursorGothic, CursorGothic Fallback, system-ui, Helvetica Neue`. Other loaded fonts: EB Garamond, CursorIcons16.

- **headline-display:** CursorGothic 26px at weight 400, line height 1.25, tracking -0.013em (24.5px on mobile). Page title (h1).
- **headline-lg:** CursorGothic 22px at weight 400, line height 1.3, tracking -0.005em (15px on mobile). Section headings (h2).
- **body-md:** CursorGothic 14px at weight 400, line height 1.5, tracking 0.01em. Body text.
- **body-lg:** system-ui 16px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** system-ui 12px at weight 400, line height 1.33. Secondary and small text.
- **caption:** system-ui 11px at weight 400, line height 1.27, tracking 0.004em. Captions and fine print.
- **label-lg:** CursorGothic 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** system-ui 14px at weight 600, line height 1.55. Buttons, navigation and labels.
- **label-sm:** Lato 12px at weight 600, line height 1.27, tracking 0.004em. Small labels and badges.
- **code:** berkeleyMono 12px at weight 400, line height 1.67. Code and technical values.

## Layout

Spacing does not follow a strict grid: 27% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 10px, lg 17.5px, xl 44.8px.
- **Sections:** 67.2px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 360px, 420px, 640px, 660px, 767px, 768px, 900px, 1140px, 1380px, 1470px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `oklab(0.263084 -0.00230259 0.0124794 / 0.1) 0px 0px 0px 1px, rgba(0, 0, 0, 0.28) 0px 18px 36px -18px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 232 elements.
- **md (8px):** 68 elements.
- **lg (10px):** 28 elements.
- **xl (12px):** 28 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Download”):** #26251E fill, #F7F7F4 text, 14px/400, 3.35544e+07px radius, padding 5.6px 10.5px 5.88px 10.5px, border 1px solid #26251E.
- **button-primary-hover:** background #3B3A33, text #F7F7F4 on hover.
- **button-outline (“Request a demo →”):** #E6E5E0 fill, #26251E text, 16px/400, 3.35544e+07px radius, padding 12.48px 21.6px 12.8px 21.6px.
- **button-outline-hover:** background #E1E0DB, text #26251E on hover.
- **button-ghost (“Contact sales”):** transparent fill, #26251E text, 14px/400, 3.35544e+07px radius, padding 5.6px 10.5px 5.88px 10.5px, border 1px solid #26251E33.
- **input-field (“Plan, search, build anything...”):** transparent fill, #26251E text, 13px/400, padding 8px 8px 6px 8px.
- **link:** transparent fill, #26251E text, padding 0px.

## Do's and Don'ts

- Do use #F7F7F4 for the page and lift surfaces in small steps: #F2F1ED, #EBEAE5, #E6E5E0, #E1E0DB.
- Do keep text in 2 levels: #26251E, #7A7974.
- Do use #F54E00 as the brand accent: header, logo and key highlights.
- Do set headlines in CursorGothic with tight tracking (-0.013em).
- Do reuse the measured spacing steps (6px, 10px, 17.5px).
- Do use 4px corners on most elements; larger surfaces also use 8px, 10px and 12px.
- Don't use #7A7974 for body text; it reaches 4.06:1 on #F7F7F4. Keep it for large text or metadata.
- Don't introduce new font families beyond CursorGothic, system-ui, Lato and berkeleyMono.
- Don't use #F54E00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.12s, 0.2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cursor.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
