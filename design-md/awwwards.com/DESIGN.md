---
version: alpha
name: Awwwards
description: "Light monochrome interface measured from awwwards.com: Inter Tight type, tonal surfaces and 8px corners."
colors:
  background: "#E9E9E9"
  surface: "#E9E9E9"
  on-surface: "#222222"
  on-background: "#222222"
  surface-container-low: "#F8F8F8"
  surface-container: "#FFFFFFE6"
  surface-container-high: "#FFFFFF"
  overlay: "#FFFFFF33"
  outline: "#F8F8F8"
  outline-variant: "#FFFFFF"
  primary: "#222222"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: Inter Tight
    fontSize: 127px
    fontWeight: 600
    lineHeight: 1
  headline-lg:
    fontFamily: Inter Tight
    fontSize: 42px
    fontWeight: 600
    lineHeight: 1.2
  headline-md:
    fontFamily: Inter Tight
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.17
  headline-sm:
    fontFamily: Inter Tight
    fontSize: 22px
    fontWeight: 300
    lineHeight: 1.27
  title-lg:
    fontFamily: Inter Tight
    fontSize: 20.5px
    fontWeight: 600
    lineHeight: 1.36
  body-md:
    fontFamily: Inter Tight
    fontSize: 14px
    fontWeight: 300
    lineHeight: 2
  body-lg:
    fontFamily: Inter Tight
    fontSize: 18px
    fontWeight: 400
    lineHeight: 0.93
  body-sm:
    fontFamily: Inter Tight
    fontSize: 13px
    fontWeight: 300
    lineHeight: 2.15
  label-md:
    fontFamily: Inter Tight
    fontSize: 14px
    fontWeight: 400
    lineHeight: 2
  headline-display-mobile:
    fontFamily: Inter Tight
    fontSize: 42px
    fontWeight: 600
    lineHeight: 1
  title-lg-mobile:
    fontFamily: Inter Tight
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.56
rounded:
  sm: 4px
  md: 8px
  lg: 14px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 33.51px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 20px
    height: 42px
  button-primary-hover:
    backgroundColor: "#383838"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 0px 15.6px
    height: 60px
  button-ghost:
    textColor: "#DEDEDE"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 0px 12px
    height: 48px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px 0px 0px 38px
  link:
    textColor: "{colors.primary}"
---

# Awwwards Design System

## Overview

Awwwards describes itself as: “Awwwards are the Website Awards that recognize and promote the talent and effort of the best developers, designers and web agencies in the world.” The interface is light, built on **Mist (#E9E9E9)** with **Charcoal (#222222)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Inter Tight**. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 8px.

Measured from [awwwards.com](https://www.awwwards.com/) on October 29, 2026 at 1440×900 and 390×844 from 293 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Mist (#E9E9E9):** Page background, seen 1 time. Token `background`, CSS `--ch-bg`.
- **Charcoal (#222222):** Primary text and headings, seen 70 times. Token `on-surface`, CSS `--border-table`.
- **Snow (#F8F8F8):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--bg-primary`.
- **White 90% (#FFFFFFE6):** Cards and panels, seen 3 times. Token `surface-container`.
- **White (#FFFFFF):** Hover and pressed fills, seen 4 times. Token `surface-container-high`, CSS `--check-toggle-color-ball`.
- **White 20% (#FFFFFF33):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Snow (#F8F8F8):** Borders and dividers, seen 3 times. Token `outline`, CSS `--bg-primary`.
- **White (#FFFFFF):** Secondary dividers, seen 2 times. Token `outline-variant`, CSS `--check-toggle-color-ball`.
- **Charcoal (#222222):** Primary buttons and calls to action, seen 79 times. Token `primary`, CSS `--border-table`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**Inter Tight** carries the whole interface. Fallback stack: `Inter Tight`.

- **headline-display:** Inter Tight 127px at weight 600, line height 1, uppercase (42px on mobile). Page title (h1).
- **headline-lg:** Inter Tight 42px at weight 600, line height 1.2. Section headings (h2).
- **headline-md:** Inter Tight 24px at weight 600, line height 1.17. Sub-section headings.
- **headline-sm:** Inter Tight 22px at weight 300, line height 1.27. Card and feature titles.
- **title-lg:** Inter Tight 20.5px at weight 600, line height 1.36 (18px on mobile). Small titles.
- **body-md:** Inter Tight 14px at weight 300, line height 2. Body text.
- **body-lg:** Inter Tight 18px at weight 400, line height 0.93. Lead paragraphs.
- **body-sm:** Inter Tight 13px at weight 300, line height 2.15. Secondary and small text.
- **label-md:** Inter Tight 14px at weight 400, line height 2. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 63% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 12px, lg 20px, xl 33.51px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 576px, 700px, 768px, 1000px, 1024px, 1100px, 1168px, 1184px, 1270px, 1280px, 1360px, 1490px, 1556px, 1578px, 1600px, 1780px, 2291px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F8F8F8 → #FFFFFFE6 → #FFFFFF) and #F8F8F8 borders.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 60 elements.
- **lg (14px):** 12 elements.
- **full (9999px):** 12 elements.
- **sm (4px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Be Pro”):** #222222 fill, #FFFFFF text, 14px/500, 8px radius, padding 0px 20px.
- **button-primary-hover:** background #383838, text #FFFFFF on hover.
- **button-outline (“Visit Sotd.”):** #E9E9E9 fill, #222222 text, 13px/600, 8px radius, padding 0px 15.6px.
- **button-ghost (“Nominees”):** transparent fill, #DEDEDE text, 13px/400, 8px radius, padding 0px 12px, border 1px solid #4E4E4E.
- **input-field (“Search by Inspiration”):** transparent fill, #222222 text, 13.3px/400, padding 0px 0px 0px 38px.
- **link:** transparent fill, #222222 text, padding 0px.

## Do's and Don'ts

- Do use #E9E9E9 for the page and lift surfaces in small steps: #F8F8F8, #FFFFFFE6, #FFFFFF.
- Do let contrast carry emphasis; primary actions use #222222 on #E9E9E9.
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 8px corners on most elements; larger surfaces also use 14px and 4px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Inter Tight.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/awwwards.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
