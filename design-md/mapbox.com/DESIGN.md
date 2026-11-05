---
version: alpha
name: Mapbox
description: "Light interface measured from mapbox.com: Cera pro type, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#333943"
  on-background: "#333943"
  on-surface-strong: "#0E1012"
  on-surface-variant: "#8B949E"
  surface-container-low: "#F7F9FC"
  overlay: "#0B0D1224"
  outline: "#E0E4EC"
  outline-variant: "#C8CED8"
  primary: "#007AFC"
  on-primary: "#FFFFFF"
  secondary: "#4C8DFF"
typography:
  headline-display:
    fontFamily: Cera pro
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Cera pro
    fontSize: 46px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Cera pro
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: -0.01em
  body-md:
    fontFamily: Cera pro
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.4
  body-lg:
    fontFamily: Cera pro
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.65
  body-sm:
    fontFamily: Cera pro
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-lg:
    fontFamily: Cera pro
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.65
  label-md:
    fontFamily: Cera pro
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.4
  label-sm:
    fontFamily: Cera pro
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0.1em
  headline-display-mobile:
    fontFamily: Cera pro
    fontSize: 34px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Cera pro
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.35
    letterSpacing: -0.01em
rounded:
  sm: 2px
  md: 4px
  lg: 6px
  full: 9999px
spacing:
  xs: 3px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 100px
    padding: 8px 16px
    height: 38px
  button-primary-hover:
    backgroundColor: "#3195FF"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.lg}"
    padding: 10px 12px
    height: 41px
  button-outline-hover:
    backgroundColor: "#EFF7FF"
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 8px 10px
    height: 35px
  card:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "#BBC2CE"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 48px 43.2px
  link:
    textColor: "{colors.on-surface}"
---

# Mapbox Design System

## Overview

Mapbox describes itself as: “APIs and SDKs for AI-powered maps, location search, turn-by-turn navigation, and geospatial data in mobile or web apps. Get started for free.” The interface is light, built on **White (#FFFFFF)** with **Cool Graphite (#333943)** text, and **Vivid Blue (#007AFC)** as the main accent.

Type is set in **Cera pro**. Headlines run large with tight negative tracking; body text is 15px. The surface language is flat. Controls are pill-shaped.

Measured from [mapbox.com](https://www.mapbox.com/) on November 4, 2026 at 1440×900 and 390×844 from 345 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`, CSS `--nav--light-bg`.
- **Cool Graphite (#333943):** Primary text and headings, seen 7 times. Token `on-surface`.
- **Charcoal (#0E1012):** Headings and emphasis, seen 27 times. Token `on-surface-strong`, CSS `--_colors---utility--neutral95`.
- **Cool Gray (#8B949E):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Snow (#F7F9FC):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`, CSS `--text-colors--text-neutral-light-01<deleted|variable-527b2f28-1179-6a07-e736-c12080612a03>`.
- **Cool Charcoal 14% (#0B0D1224):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Cool Mist (#E0E4EC):** Borders and dividers, seen 12 times. Token `outline`.
- **Cool Silver (#C8CED8):** Secondary dividers, seen 11 times. Token `outline-variant`, CSS `--_color-mode---neutral--cm_neutral25`.
- **Vivid Blue (#007AFC):** Primary buttons and calls to action, seen 2 times. Token `primary`, CSS `--text-colors--text-primary50<deleted|variable-2c11adc1-e274-343d-8a1c-5015124e16ae>`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#4C8DFF):** Accent in text, fills and borders, seen 3 times. Token `secondary`.

## Typography

**Cera pro** carries the whole interface. Fallback stack: `Cera pro, Trebuchet MS, sans-serif`.

- **headline-display:** Cera pro 56px at weight 700, line height 1.25, tracking -0.01em (34px on mobile). Page title (h1).
- **headline-lg:** Cera pro 46px at weight 700, line height 1.25, tracking -0.01em (28px on mobile). Section headings (h2).
- **headline-md:** Cera pro 36px at weight 700, line height 1.3, tracking -0.01em. Sub-section headings.
- **body-md:** Cera pro 15px at weight 400, line height 1.4. Body text.
- **body-lg:** Cera pro 18px at weight 400, line height 1.65. Lead paragraphs.
- **body-sm:** Cera pro 14px at weight 400, line height 1.43. Secondary and small text.
- **label-lg:** Cera pro 16px at weight 400, line height 1.65. Large buttons and tabs.
- **label-md:** Cera pro 15px at weight 500, line height 1.4. Buttons, navigation and labels.
- **label-sm:** Cera pro 14px at weight 500, line height 1, tracking 0.1em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 57% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 8px, md 12px, lg 24px, xl 48px.
- **Gaps:** 48px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 425px, 426px, 479px, 500px, 550px, 600px, 767px, 768px, 769px, 890px, 896px, 897px, 991px, 1023px, 1024px, 1280px, 1920px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F7F9FC) and #E0E4EC borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 56 elements.
- **sm (2px):** 52 elements.
- **lg (6px):** 16 elements.
- **md (4px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #007AFC fill, #FFFFFF text, 15px/500, 100px radius, padding 8px 16px, border 1px solid #007AFC.
- **button-primary-hover:** background #3195FF, text #FFFFFF on hover.
- **button-outline (“ChatGPT”):** #F7F9FC fill, #0E1012 text, 14px/600, 6px radius, padding 10px 12px, border 1px solid #D5DAE2.
- **button-outline-hover:** background #EFF7FF, text #0E1012 on hover.
- **button-ghost (“EN”):** transparent fill, #0E1012 text, 15px/400, 6px radius, padding 8px 10px, border 1px solid #BBC2CE.
- **card:** #0E1012 fill, #BBC2CE text, 16px/400, padding 48px 43.2px.
- **link:** transparent fill, #333943 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F7F9FC.
- Do keep text in 3 levels: #333943, #0E1012, #8B949E.
- Do reserve #007AFC for primary actions and key highlights.
- Do set headlines in Cera pro with tight tracking (-0.01em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 2px corners.
- Don't use #8B949E for body text; it reaches 3.08:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Cera pro.
- Don't use #007AFC for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.2s, 0.4s, 0.5s, 0.6s. Longer ambient animations run 1s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mapbox.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
