---
version: alpha
name: Are.na
description: "Dark monochrome interface measured from are.na: areal type, tonal surfaces and 3px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#E5E5E5"
  on-surface-muted: "#B2B2B2"
  on-surface-subtle: "#696969"
  surface-container-low: "#1A1A1A"
  surface-container: "#333333"
  overlay: "#1A1A1A99"
  outline: "#4F4F4F"
  outline-variant: "#333333"
  primary: "#E2DFE9"
  on-primary: "#000000"
typography:
  headline-display:
    fontFamily: areal
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.45
  body-md:
    fontFamily: areal
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  body-lg:
    fontFamily: areal
    fontSize: 19px
    fontWeight: 700
    lineHeight: 1.45
  body-sm:
    fontFamily: areal
    fontSize: 12.5px
    fontWeight: 400
    lineHeight: 1.35
  label-md:
    fontFamily: areal
    fontSize: 14.5px
    fontWeight: 700
  label-sm:
    fontFamily: areal
    fontSize: 12.5px
    fontWeight: 700
  headline-display-mobile:
    fontFamily: areal
    fontSize: 12.5px
    fontWeight: 400
    lineHeight: 1.35
rounded:
  md: 3px
spacing:
  xs: 2.5px
  sm: 6px
  md: 15px
  lg: 25px
  xl: 35px
  gutter: 15px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 15px
    height: 34px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 0px 10px
    height: 24px
  button-outline-hover:
    textColor: "{colors.on-surface}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  input-field:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.headline-display}"
    rounded: "{rounded.md}"
    padding: 0px 20px 0px 45px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Are.na Design System

## Overview

Are.na describes itself as: “Are.na is a platform for connecting ideas and building knowledge.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **areal**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 3px.

Measured from [are.na](https://www.are.na/) on October 21, 2026 at 1440×900 and 390×844 from 248 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Near Black (#000000):** Page background, seen 2 times. Token `background`, CSS `--colors-gray0`.
- **White (#FFFFFF):** Primary text and headings, seen 28 times. Token `on-surface`, CSS `--colors-gray7`.
- **Mist (#E5E5E5):** Secondary text, seen 31 times. Token `on-surface-variant`, CSS `--colors-link`.
- **Gray (#B2B2B2):** Muted text and metadata, seen 17 times. Token `on-surface-muted`, CSS `--colors-slate`.
- **Slate (#696969):** Subtle text and placeholders, seen 13 times. Token `on-surface-subtle`.
- **Charcoal (#1A1A1A):** Raised areas one step from the page, seen 54 times. Token `surface-container-low`, CSS `--colors-channelClosed1`.
- **Graphite (#333333):** Cards and panels, seen 30 times. Token `surface-container`, CSS `--colors-gray2`.
- **Charcoal 60% (#1A1A1A99):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Slate (#4F4F4F):** Borders and dividers, seen 4 times. Token `outline`, CSS `--colors-gray3`.
- **Graphite (#333333):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--colors-gray2`.
- **Cool Mist (#E2DFE9):** Primary buttons and calls to action, seen 3 times. Token `primary`, CSS `--colors-blue3`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.

## Typography

**areal** carries the whole interface. Fallback stack: `areal, areal Fallback, Arial, Helvetica`. Other loaded fonts: areal Fallback.

- **headline-display:** areal 19px at weight 400, line height 1.45 (12.5px on mobile). Page title (h1).
- **body-md:** areal 16px at weight 400, line height 1. Body text.
- **body-lg:** areal 19px at weight 700, line height 1.45. Lead paragraphs.
- **body-sm:** areal 12.5px at weight 400, line height 1.35. Secondary and small text.
- **label-md:** areal 14.5px at weight 700. Buttons, navigation and labels.
- **label-sm:** areal 12.5px at weight 700. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 1% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2.5px, sm 6px, md 15px, lg 25px, xl 35px.
- **Gaps:** 15px is the most common gap in flex and grid layouts.
- **Breakpoints:** 520px, 900px, 1200px, 1800px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `color(srgb 1 1 1 / 0.05) 0px 0px 34px 0px`

## Shapes

Most elements use 3px corners. Measured radii, most used first:

- **md (3px):** 244 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #E2DFE9 fill, #000000 text, 14.4px/700, 3px radius, padding 0px 15px.
- **button-primary-hover:** background #FFFFFF, text #000000 on hover.
- **button-outline (“Log in”):** #1A1A1A fill, #E5E5E5 text, 12.5px/700, 3px radius, padding 0px 10px.
- **button-outline-hover:** background #1A1A1A, text #FFFFFF on hover.
- **button-ghost (“Capture Save photos, notes, file”):** transparent fill, #FFFFFF text, 16px/400, padding 0px.
- **input-field (“Search Are.na”):** #1A1A1A99 fill, #E5E5E5 text, 19.2px/400, 3px radius, padding 0px 20px 0px 45px, border 1px solid #4F4F4F, shadow `color(srgb 1 1 1 / 0.05) 0px 0px 34px 0px`.
- **link:** transparent fill, #E5E5E5 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #1A1A1A, #333333.
- Do keep text in 4 levels: #FFFFFF, #E5E5E5, #B2B2B2, #696969.
- Do let contrast carry emphasis; primary actions use #E2DFE9 on #000000.
- Do reuse the measured spacing steps (6px, 15px, 25px).
- Do use 3px corners on most elements.
- Don't use #696969 for body text; it reaches 3.8:1 on #000000. Keep it for large text or metadata.
- Don't introduce new font families beyond areal.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.

Generated by [Sitepeel](https://sitepeel.dev/design-md/are.na/), the free DESIGN.md generator.
