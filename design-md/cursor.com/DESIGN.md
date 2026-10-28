---
version: alpha
name: Cursor
description: "Dark interface measured from cursor.com: CursorGothic type with EB Garamond, vivid orange accents, tonal surfaces and 4px corners."
colors:
  background: "#14120B"
  surface: "#14120B"
  on-surface: "#EDECEC"
  on-background: "#EDECEC"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#969592"
  surface-container-low: "#1B1913"
  surface-container: "#201E18"
  surface-container-high: "#26241E"
  surface-container-highest: "#2B2923"
  overlay: "#EDECEC1A"
  overlay-strong: "#EDECEC33"
  outline: "#EDECEC06"
  outline-variant: "#EDECEC1A"
  primary: "#F54E00"
  on-primary: "#000000"
  secondary: "#CF2D56"
  tertiary: "#8BC4F8"
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
    fontFamily: EB Garamond
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.35
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
  lg: 12px
spacing:
  xs: 2px
  sm: 6px
  md: 10px
  lg: 17.5px
  xl: 44.8px
  gutter: 10px
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
    backgroundColor: "#D7D6D5"
  button-outline:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
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

Cursor describes itself as: “Built to make you extraordinarily productive, agents turn ideas into code. Accelerate development by handing off tasks to Cursor.” The interface is dark, built on **Warm Charcoal (#14120B)** with **Mist (#EDECEC)** text, and **Vivid Orange (#F54E00)** as the main accent.

Type is set in **CursorGothic** and **EB Garamond**, with **berkeleyMono** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [cursor.com](https://cursor.com/) on October 21, 2026 at 1440×900 and 390×844 from 439 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles.

- **Warm Charcoal (#14120B):** Page background, seen 15 times. Token `background`.
- **Mist (#EDECEC):** Primary text and headings, seen 101 times. Token `on-surface`, CSS `--color-theme-button-bg`.
- **White (#FFFFFF):** Headings and emphasis, seen 2 times. Token `on-surface-strong`, CSS `--color-white`.
- **Gray (#969592):** Secondary text, seen 15 times. Token `on-surface-variant`.
- **Warm Charcoal (#1B1913):** Raised areas one step from the page, seen 34 times. Token `surface-container-low`, CSS `--color-theme-product-editor`.
- **Warm Charcoal (#201E18):** Cards and panels, seen 7 times. Token `surface-container`.
- **Warm Charcoal (#26241E):** Hover and pressed fills, seen 6 times. Token `surface-container-high`.
- **Warm Graphite (#2B2923):** Highest raised elements, seen 4 times. Token `surface-container-highest`.
- **Mist 10% (#EDECEC1A):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Mist 20% (#EDECEC33):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Mist 2% (#EDECEC06):** Borders and dividers, seen 38 times. Token `outline`.
- **Mist 10% (#EDECEC1A):** Secondary dividers, seen 6 times. Token `outline-variant`.
- **Vivid Orange (#F54E00):** Brand accent (CSS variable), seen 8 times. Token `primary`, CSS `--color-accent`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Pink (#CF2D56):** Most used accent color, seen 5 times. Token `secondary`.
- **Light Blue (#8BC4F8):** Most used accent color, seen 3 times. Token `tertiary`.
- **Dark Teal (#1F8A65):** Success and positive states, seen 5 times. Token `success`.

## Typography

**CursorGothic**, **EB Garamond**, **system-ui**, **Lato** and **berkeleyMono** (monospace) share the interface. Fallback stack: `CursorGothic, CursorGothic Fallback, system-ui, Helvetica Neue`. Other loaded fonts: CursorGothic Fallback, CursorIcons16.

- **headline-display:** CursorGothic 26px at weight 400, line height 1.25, tracking -0.013em (24.5px on mobile). Page title (h1).
- **headline-lg:** CursorGothic 22px at weight 400, line height 1.3, tracking -0.005em (15px on mobile). Section headings (h2).
- **body-md:** CursorGothic 14px at weight 400, line height 1.5, tracking 0.01em. Body text.
- **body-lg:** EB Garamond 17px at weight 400, line height 1.35. Lead paragraphs.
- **body-sm:** system-ui 12px at weight 400, line height 1.33. Secondary and small text.
- **caption:** system-ui 11px at weight 400, line height 1.27, tracking 0.004em. Captions and fine print.
- **label-lg:** CursorGothic 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** system-ui 14px at weight 600, line height 1.55. Buttons, navigation and labels.
- **label-sm:** Lato 12px at weight 600, line height 1.27, tracking 0.004em. Small labels and badges.
- **code:** berkeleyMono 12px at weight 400, line height 1.67. Code and technical values.

## Layout

Spacing does not follow a strict grid: 23% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 10px, lg 17.5px, xl 44.8px.
- **Sections:** 67.2px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 360px, 420px, 640px, 660px, 767px, 768px, 900px, 1140px, 1380px, 1470px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `oklab(0.943853 0.00107113 0.000336707 / 0.1) 0px 0px 0px 1px, rgba(0, 0, 0, 0.28) 0px 18px 36px -18px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 220 elements.
- **md (8px):** 56 elements.
- **lg (12px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Download”):** #EDECEC fill, #14120B text, 14px/400, 3.35544e+07px radius, padding 5.6px 10.5px 5.88px 10.5px, border 1px solid #EDECEC.
- **button-primary-hover:** background #D7D6D5, text #14120B on hover.
- **button-outline (“Request a demo →”):** #26241E fill, #EDECEC text, 16px/400, 3.35544e+07px radius, padding 12.48px 21.6px 12.8px 21.6px.
- **button-outline-hover:** background #2B2923, text #EDECEC on hover.
- **button-ghost (“Contact sales”):** transparent fill, #EDECEC text, 14px/400, 3.35544e+07px radius, padding 5.6px 10.5px 5.88px 10.5px, border 1px solid #EDECEC33.
- **input-field (“Plan, search, build anything...”):** transparent fill, #EDECEC text, 13px/400, padding 8px 8px 6px 8px.
- **link:** transparent fill, #EDECEC text, padding 0px.

## Do's and Don'ts

- Do use #14120B for the page and lift surfaces in small steps: #1B1913, #201E18, #26241E, #2B2923.
- Do keep text in 3 levels: #EDECEC, #FFFFFF, #969592.
- Do use #F54E00 as the brand accent: header, logo and key highlights.
- Do set headlines in CursorGothic with tight tracking (-0.013em).
- Do reuse the measured spacing steps (6px, 10px, 17.5px).
- Do use 4px corners on most elements; larger surfaces also use 8px and 12px.
- Don't introduce new font families beyond CursorGothic, EB Garamond, system-ui, Lato and berkeleyMono.
- Don't use #F54E00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s. Longer ambient animations run 2.5s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `linear`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cursor.com/), the free DESIGN.md generator.
