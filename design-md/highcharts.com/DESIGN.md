---
version: alpha
name: Highcharts
description: "Light interface measured from highcharts.com: IBM Plex Sans type with IBM Plex Sans Variable, indigo accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#18171C"
  on-background: "#18171C"
  on-surface-strong: "#000000"
  surface-container-low: "#F0F1FF"
  surface-container: "#F2F1F4"
  outline: "#0000001F"
  outline-variant: "#E3E3E8"
  primary: "#626BD0"
  on-primary: "#FFFFFF"
  inverse-surface: "#2F2E38"
  secondary: "#047857"
  tertiary: "#8087E8"
  success: "#065F46"
typography:
  headline-display:
    fontFamily: IBM Plex Sans
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.3
  headline-lg:
    fontFamily: IBM Plex Sans
    fontSize: 42.5px
    fontWeight: 700
    lineHeight: 1.3
  headline-md:
    fontFamily: IBM Plex Sans
    fontSize: 25px
    fontWeight: 700
    lineHeight: 1.3
  headline-sm:
    fontFamily: IBM Plex Sans Variable
    fontSize: 22px
    fontWeight: 600
    lineHeight: 1.3
  body-md:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.3
  body-lg:
    fontFamily: IBM Plex Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  body-sm:
    fontFamily: IBM Plex Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.3
  label-lg:
    fontFamily: IBM Plex Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.3
  label-md:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.3
  label-sm:
    fontFamily: IBM Plex Sans
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.3
  headline-display-mobile:
    fontFamily: IBM Plex Sans
    fontSize: 42px
    fontWeight: 700
    lineHeight: 1.3
rounded:
  sm: 6px
  md: 8px
  lg: 10px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 9px
  lg: 20px
  xl: 36px
  gutter: 10px
  margin: 20px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 7px
    height: 32px
  button-primary-hover:
    backgroundColor: "#8791FF"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 7px
    height: 32px
  button-secondary-hover:
    backgroundColor: "#059669"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 9px
  input-field:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 24px
  link:
    textColor: "#474554"
---

# Highcharts Design System

## Overview

Highcharts describes itself as: “Highcharts JavaScript charting library: Core, Stock, Maps, Gantt, Grid and Dashboards. Build interactive data visualizations with modern frameworks like React.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#18171C)** text, and **Indigo (#626BD0)** as the main accent.

Type is set in **IBM Plex Sans** and **IBM Plex Sans Variable**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [highcharts.com](https://www.highcharts.com/) on November 4, 2026 at 1440×900 and 390×844 from 433 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #C61F25A6, #7F1D1DA6, #4A55C9.

- **White (#FFFFFF):** Page background, seen 6 times. Token `background`, CSS `--button-colors-attention-text-default`.
- **Charcoal (#18171C):** Primary text and headings, seen 38 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 3 times. Token `on-surface-strong`, CSS `--solo-default-placeholder-focused`.
- **Cool Snow (#F0F1FF):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Mist (#F2F1F4):** Cards and panels, seen 7 times. Token `surface-container`.
- **Near Black 12% (#0000001F):** Borders and dividers, seen 14 times. Token `outline`.
- **Mist (#E3E3E8):** Secondary dividers, seen 3 times. Token `outline-variant`, CSS `--HS-surface-ui-border-100`.
- **Indigo (#626BD0):** Brand color in the header, seen 7 times. Token `primary`, CSS `--icon-color-blue`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Cool Graphite (#2F2E38):** High-contrast fills, seen 3 times. Token `inverse-surface`, CSS `--radiobox-text-default`.
- **Dark Teal (#047857):** Secondary buttons, seen 1 time. Token `secondary`.
- **Light Indigo (#8087E8):** Accent in the logo, seen 2 times. Token `tertiary`.
- **Deep Teal (#065F46):** Success and positive states, seen 1 time. Token `success`.

## Typography

**IBM Plex Sans** and **IBM Plex Sans Variable** share the interface. Fallback stack: `IBM Plex Sans, sans-serif`.

- **headline-display:** IBM Plex Sans 56px at weight 700, line height 1.3 (42px on mobile). Page title (h1).
- **headline-lg:** IBM Plex Sans 42.5px at weight 700, line height 1.3. Section headings (h2).
- **headline-md:** IBM Plex Sans 25px at weight 700, line height 1.3. Sub-section headings.
- **headline-sm:** IBM Plex Sans Variable 22px at weight 600, line height 1.3. Card and feature titles.
- **body-md:** IBM Plex Sans 14px at weight 400, line height 1.3. Body text.
- **body-lg:** IBM Plex Sans 16px at weight 400, line height 1.15. Lead paragraphs.
- **body-sm:** IBM Plex Sans 12px at weight 400, line height 1.3. Secondary and small text.
- **label-lg:** IBM Plex Sans 16px at weight 500, line height 1.3. Large buttons and tabs.
- **label-md:** IBM Plex Sans 14px at weight 500, line height 1.3. Buttons, navigation and labels.
- **label-sm:** IBM Plex Sans 12px at weight 500, line height 1.3. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 48% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 9px, lg 20px, xl 36px.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 375px, 781px, 782px, 850px, 1000px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 0px 1px 0px, rgba(0, 0, 0, 0.09) 0px 1px 1px 0px, rgba(0, 0, 0, 0.05) 0px 3px 2px 0px, rgba(0, 0, 0, 0.01) 0px 6px 2px 0px`
- `rgba(0, 0, 0, 0.1) 0px 2px 8px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 100 elements.
- **sm (6px):** 64 elements.
- **full (9999px):** 20 elements.
- **lg (10px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try for Free”):** #626BD0 fill, #FFFFFF text, 14px/500, 8px radius, padding 7px, border 1px solid #4A55C9.
- **button-primary-hover:** background #8791FF, text #FFFFFF on hover.
- **button-secondary (“Buy Now”):** #047857 fill, #FFFFFF text, 14px/500, 8px radius, padding 7px, border 1px solid #065F46.
- **button-secondary-hover:** background #059669, text #FFFFFF on hover.
- **button-ghost (“Products”):** transparent fill, #18171C text, 16px/500, 8px radius, padding 9px.
- **input-field (“Email address”):** transparent fill, #000000 text, 14px/400, padding 0px.
- **card:** #FFFFFF fill, #18171C text, 16px/400, 8px radius, padding 24px, border 1px solid #E3E3E8.
- **link:** transparent fill, #474554 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F0F1FF, #F2F1F4.
- Do keep text in 2 levels: #18171C, #000000.
- Do use #626BD0 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 9px, 20px).
- Do use 8px corners on most elements; larger surfaces also use 6px and 10px.
- Don't introduce new font families beyond IBM Plex Sans and IBM Plex Sans Variable.
- Don't use #626BD0 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.2s, 0.1s, 0.4s, 0.3s.

- **Easing:** `cubic-bezier(0.075, 0.82, 0.165, 1)`, `cubic-bezier(0.6, 1, 0.2, 1.2)`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/highcharts.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
