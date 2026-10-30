---
version: alpha
name: Are.na
description: "Light interface measured from are.na: areal type, deep indigo accents, tonal surfaces and 3px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#333333"
  on-surface-muted: "#696969"
  on-surface-subtle: "#999999"
  surface-container-low: "#F7F7F7"
  overlay: "#F7F7F799"
  outline: "#DEDEDE"
  outline-variant: "#EDEDED"
  primary: "#00075F"
  on-primary: "#FFFFFF"
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
  sm: 3px
  md: 10px
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
    rounded: "{rounded.sm}"
    padding: 0px 15px
    height: 34px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
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
    rounded: "{rounded.sm}"
    padding: 0px 20px 0px 45px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Are.na Design System

## Overview

Are.na describes itself as: “Are.na is a platform for connecting ideas and building knowledge.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Deep Indigo (#00075F)** as the main accent.

Type is set in **areal**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 3px.

Measured from [are.na](https://www.are.na/) on October 29, 2026 at 1440×900 and 390×844 from 225 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`, CSS `--colors-gray0`.
- **Near Black (#000000):** Primary text and headings, seen 28 times. Token `on-surface`, CSS `--colors-gray7`.
- **Graphite (#333333):** Secondary text, seen 30 times. Token `on-surface-variant`, CSS `--colors-link`.
- **Slate (#696969):** Muted text and metadata, seen 18 times. Token `on-surface-muted`, CSS `--colors-slate`.
- **Gray (#999999):** Subtle text and placeholders, seen 10 times. Token `on-surface-subtle`.
- **Snow (#F7F7F7):** Raised areas one step from the page, seen 25 times. Token `surface-container-low`, CSS `--colors-channelClosed1`.
- **Snow 60% (#F7F7F799):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Silver (#DEDEDE):** Borders and dividers, seen 4 times. Token `outline`, CSS `--colors-gray3`.
- **Mist (#EDEDED):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--colors-gray2`.
- **Deep Indigo (#00075F):** Primary buttons and calls to action, seen 3 times. Token `primary`, CSS `--colors-blue3`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**areal** carries the whole interface. Fallback stack: `areal, areal Fallback, Arial, Helvetica`.

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

- `color(srgb 0 0 0 / 0.05) 0px 0px 34px 0px`

## Shapes

Most elements use 3px corners. Measured radii, most used first:

- **sm (3px):** 128 elements.
- **md (10px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #00075F fill, #FFFFFF text, 14.4px/700, 3px radius, padding 0px 15px.
- **button-primary-hover:** background #000000, text #FFFFFF on hover.
- **button-outline (“Log in”):** #F7F7F7 fill, #333333 text, 12.5px/700, 3px radius, padding 0px 10px.
- **button-outline-hover:** background #F7F7F7, text #000000 on hover.
- **button-ghost (“Capture Save photos, notes, file”):** transparent fill, #000000 text, 16px/400, padding 0px.
- **input-field (“Search Are.na”):** #F7F7F799 fill, #333333 text, 19.2px/400, 3px radius, padding 0px 20px 0px 45px, border 1px solid #DEDEDE, shadow `color(srgb 0 0 0 / 0.05) 0px 0px 34px 0px`.
- **link:** transparent fill, #333333 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F7F7F7.
- Do keep text in 4 levels: #000000, #333333, #696969, #999999.
- Do reserve #00075F for primary actions and key highlights.
- Do reuse the measured spacing steps (6px, 15px, 25px).
- Do use 3px corners on most elements; larger surfaces also use 10px.
- Don't use #999999 for body text; it reaches 2.85:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond areal.
- Don't use #00075F for large backgrounds or body text.
- Don't make interface transitions slower than 0.24s.

## Motion

Interface transitions are quick: 0.18s, 0.15s, 0.24s, 0.2s.

- **Easing:** `ease`, `cubic-bezier(0.16, 1, 0.3, 1)`, `cubic-bezier(0.22, 1, 0.36, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/are.na/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
