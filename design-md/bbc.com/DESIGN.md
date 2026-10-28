---
version: alpha
name: BBC
description: "Light monochrome interface measured from bbc.com: BBC Reith Serif type with BBC Reith Sans, tonal surfaces and pill-shaped controls."
colors:
  background: "#F8F8F8"
  surface: "#F8F8F8"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#202224"
  on-surface-muted: "#545658"
  on-surface-subtle: "#AFB1B4"
  surface-container-low: "#FFFFFF"
  surface-container: "#E6E8EA"
  outline: "#D2D4D6"
  outline-variant: "#E6E8EA"
  primary: "#000000"
  on-primary: "#FFFFFF"
  secondary: "#EB0000"
  error: "#E00000"
typography:
  headline-display:
    fontFamily: BBC Reith Serif
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.14
    letterSpacing: -0.02em
  body-md:
    fontFamily: BBC Reith Serif
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.22
    letterSpacing: -0.02em
  body-sm:
    fontFamily: BBC Reith Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.17
    letterSpacing: -0.01em
  label-lg:
    fontFamily: BBC Reith Sans
    fontSize: 15px
    fontWeight: 800
    lineHeight: 1.33
    letterSpacing: 0.05em
  label-md:
    fontFamily: BBC Reith Serif
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.29
    letterSpacing: -0.02em
  label-sm:
    fontFamily: BBC Reith Sans
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.17
rounded:
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 9.3px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: 0px
    padding: 6px 12px
    height: 34px
  button-primary-hover:
    backgroundColor: "#3A3C3E"
  button-ghost:
    textColor: "{colors.on-surface}"
    rounded: 0px
    padding: 6px 12px
  link:
    textColor: "{colors.primary}"
---

# BBC Design System

## Overview

BBC describes itself as: “Visit BBC for trusted reporting on the latest world and US news, sports, business, climate, innovation, culture and much more.” The interface is light, built on **Snow (#F8F8F8)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **BBC Reith Serif** and **BBC Reith Sans**. Headlines run large with tight negative tracking; body text is 18px. The surface language is flat. Controls are pill-shaped.

Measured from [bbc.com](https://www.bbc.com/) on October 21, 2026 at 1440×900 and 1028×2225 from 468 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Snow (#F8F8F8):** Page background. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 36 times. Token `on-surface`.
- **Charcoal (#202224):** Secondary text, seen 78 times. Token `on-surface-variant`.
- **Slate (#545658):** Muted text and metadata, seen 61 times. Token `on-surface-muted`.
- **Gray (#AFB1B4):** Subtle text and placeholders, seen 7 times. Token `on-surface-subtle`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 11 times. Token `surface-container-low`.
- **Mist (#E6E8EA):** Cards and panels, seen 1 time. Token `surface-container`.
- **Silver (#D2D4D6):** Borders and dividers, seen 12 times. Token `outline`.
- **Mist (#E6E8EA):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Near Black (#000000):** Primary buttons and calls to action, seen 101 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Red (#EB0000):** Accent, seen 1 time. Token `secondary`.
- **Vivid Red (#E00000):** Errors and destructive states, seen 2 times. Token `error`.

## Typography

**BBC Reith Serif** and **BBC Reith Sans** share the interface. Fallback stack: `BBC Reith Serif, BBCReithSerif-fallback, serif`. Other loaded fonts: BBCReithSans-fallback, BBCReithSerif-fallback.

- **headline-display:** BBC Reith Serif 28px at weight 500, line height 1.14, tracking -0.02em. Page title (h1).
- **body-md:** BBC Reith Serif 18px at weight 500, line height 1.22, tracking -0.02em. Body text.
- **body-sm:** BBC Reith Sans 12px at weight 400, line height 1.17, tracking -0.01em. Secondary and small text.
- **label-lg:** BBC Reith Sans 15px at weight 800, line height 1.33, tracking 0.05em. Large buttons and tabs.
- **label-md:** BBC Reith Serif 14px at weight 500, line height 1.29, tracking -0.02em. Buttons, navigation and labels.
- **label-sm:** BBC Reith Sans 12px at weight 500, line height 1.17. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (72% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 12px, lg 24px, xl 48px.
- **Gaps:** 9.3px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Breakpoints:** 399px, 400px, 599px, 600px, 650px, 721px, 767px, 900px, 985px, 1007px, 1008px, 1279px, 1280px, 8192px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF → #E6E8EA) and #D2D4D6 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 48 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Register”):** #000000 fill, #FFFFFF text, 16px/500, padding 6px 12px, border 2px solid #000000.
- **button-primary-hover:** background #3A3C3E, text #FFFFFF on hover.
- **button-ghost (“Sign In”):** transparent fill, #000000 text, 16px/500, padding 6px 12px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #F8F8F8 for the page and lift surfaces in small steps: #FFFFFF, #E6E8EA.
- Do keep text in 4 levels: #000000, #202224, #545658, #AFB1B4.
- Do let contrast carry emphasis; primary actions use #000000 on #F8F8F8.
- Do set headlines in BBC Reith Serif with tight tracking (-0.02em).
- Do reuse the measured spacing steps (6px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px).
- Don't use #AFB1B4 for body text; it reaches 2.0:1 on #F8F8F8. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond BBC Reith Serif and BBC Reith Sans.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.5s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/bbc.com/), the free DESIGN.md generator.
