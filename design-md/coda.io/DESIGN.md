---
version: alpha
name: Coda
description: "Light interface measured from coda.io: Calibre-R type with Inter, pale orange accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#141413"
  on-background: "#141413"
  on-surface-variant: "#292827"
  on-surface-muted: "#474543"
  on-surface-subtle: "#73716D"
  surface-container-low: "#FCFAF7"
  surface-container: "#FFF6EC"
  overlay: "#FFFFFFD9"
  outline: "#DEDBD5"
  outline-variant: "#0000001A"
  primary: "#FFE6C8"
  on-primary: "#000000"
  secondary: "#EE5A29"
  tertiary: "#F8AD40"
typography:
  headline-display:
    fontFamily: Calibre-R
    fontSize: 72px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.045em
  headline-lg:
    fontFamily: Calibre-R
    fontSize: 52px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.035em
  headline-md:
    fontFamily: Calibre-R
    fontSize: 38px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: -0.03em
  body-md:
    fontFamily: Super Sans VF
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.03em
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.38
    letterSpacing: -0.03em
  label-sm:
    fontFamily: Super Sans VF
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0.01em
  headline-display-mobile:
    fontFamily: Calibre-R
    fontSize: 52px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.035em
  headline-md-mobile:
    fontFamily: Calibre-R
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
rounded:
  sm: 8px
  md: 12px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 36px
  gutter: 12px
  section: 60px
  margin: 32px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px
    height: 40px
  button-primary-hover:
    backgroundColor: "{colors.on-surface-variant}"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px
    height: 62px
  button-outline-hover:
    backgroundColor: "#F7F6F2"
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px
    height: 40px
---

# Coda Design System

## Overview

Coda describes itself as: “Coda is an all-in-one platform that blends the flexibility of docs, structure of spreadsheets, power of applications, and intelligence of AI.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#141413)** text, and **Pale Orange (#FFE6C8)** as the main accent.

Type is set in **Calibre-R** and **Inter**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [coda.io](https://coda.io/) on October 29, 2026 at 1440×900 and 390×844 from 223 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`, CSS `--origin-color-fill-base-default`.
- **Charcoal (#141413):** Primary text and headings, seen 32 times. Token `on-surface`, CSS `--origin-color-text-selected-default`.
- **Graphite (#292827):** Secondary text, seen 38 times. Token `on-surface-variant`, CSS `--origin-color-fill-base-inverse`.
- **Graphite (#474543):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Warm Slate (#73716D):** Subtle text and placeholders, seen 18 times. Token `on-surface-subtle`, CSS `--origin-color-border-business-default`.
- **Snow (#FCFAF7):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--origin-color-spot-illustration-fill-secondary`.
- **Pale Orange (#FFF6EC):** Cards and panels, seen 1 time. Token `surface-container`.
- **White 85% (#FFFFFFD9):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Warm Silver (#DEDBD5):** Borders and dividers, seen 1 time. Token `outline`.
- **Near Black 10% (#0000001A):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Pale Orange (#FFE6C8):** Brand color in logos and imagery. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Red (#EE5A29):** Accent in the header. Token `secondary`.
- **Vivid Orange (#F8AD40):** Accent on large areas. Token `tertiary`.

## Typography

**Calibre-R**, **Inter** and **Super Sans VF** share the interface. Fallback stack: `Calibre-R, sans-serif`. Other loaded fonts: Tiempos-Headline.

- **headline-display:** Calibre-R 72px at weight 700, line height 1, tracking -0.045em (52px on mobile). Page title (h1).
- **headline-lg:** Calibre-R 52px at weight 700, line height 1.1, tracking -0.035em. Section headings (h2).
- **headline-md:** Calibre-R 38px at weight 700, line height 1.1, tracking -0.025em (24px on mobile). Sub-section headings.
- **headline-sm:** Inter 20px at weight 600, line height 1.5, tracking -0.03em. Card and feature titles.
- **body-md:** Super Sans VF 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Inter 16px at weight 400, line height 1.5, tracking -0.03em. Lead paragraphs.
- **label-md:** Inter 16px at weight 600, line height 1.38, tracking -0.03em. Buttons, navigation and labels.
- **label-sm:** Super Sans VF 13px at weight 600, line height 1.2, tracking 0.01em. Small labels and badges.

## Layout

Spacing follows a 4px grid: 100% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 36px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 460px, 480px, 500px, 600px, 699px, 700px, 769px, 920px, 1024px, 1150px, 1199px, 1440px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#FCFAF7 → #FFF6EC) and hairline rings:

- `rgb(41, 40, 39) 0px 0px 0px 1.5px inset`
- `rgb(224, 224, 224) 0px 0px 0px 1.5px inset`
- `rgb(222, 219, 213) 0px 0px 0px 1.5px inset`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 128 elements.
- **md (12px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #141413 fill, #FFFFFF text, 14px/400, 8px radius, padding 0px.
- **button-primary-hover:** background #292827, text #FFFFFF on hover.
- **button-outline (“Contact sales”):** #FFFFFFD9 fill, #474543 text, 14px/400, 12px radius, padding 0px.
- **button-outline-hover:** background #F7F6F2, text #474543 on hover.
- **button-ghost (“Request a demo”):** #FFFFFF fill, #292827 text, 14px/400, 8px radius, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FCFAF7, #FFF6EC.
- Do keep text in 4 levels: #141413, #292827, #474543, #73716D.
- Do use #FFE6C8 as the brand accent: header, logo and key highlights.
- Do set headlines in Calibre-R with tight tracking (-0.045em).
- Do keep spacing on the 4px grid.
- Do use 8px corners on most elements; larger surfaces also use 12px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Calibre-R, Inter and Super Sans VF.
- Don't use #FFE6C8 for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.15s, 0.05s, 0.25s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/coda.io/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
