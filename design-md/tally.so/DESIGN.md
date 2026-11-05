---
version: alpha
name: Tally
description: "Light interface measured from tally.so: Inter type, vivid blue accents, flat surfaces and 7px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#37352F"
  on-background: "#37352F"
  on-surface-strong: "#000000"
  on-surface-variant: "#45433E"
  on-surface-muted: "#777672"
  outline: "#37352F17"
  primary: "#0070D7"
  on-primary: "#FFFFFF"
  secondary: "#F81CE5"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 64px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.031em
  headline-lg:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.15
  headline-md:
    fontFamily: Inter
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.25
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 800
    lineHeight: 1.15
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.8
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 26px
    fontWeight: 700
    lineHeight: 1.2
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.15
rounded:
  sm: 5px
  md: 7px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 64px
  gutter: 8.4px
  section: 100px
  margin: 20px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 0px 9.8px
    height: 28px
  link:
    textColor: "{colors.on-surface}"
---

# Tally Design System

## Overview

Tally describes itself as: “The simplest way to create beautiful, professional forms in seconds. Unlimited forms, unlimited submissions, forever free. Just start typing - no coding needed.” The interface is light, built on **White (#FFFFFF)** with **Warm Graphite (#37352F)** text, and **Vivid Blue (#0070D7)** as the main accent.

Type is set in **Inter**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 7px.

Measured from [tally.so](https://tally.so/) on November 4, 2026 at 1440×900 and 390×844 from 298 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles, plus gradient stops #8A46FF, #F81CE0.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`.
- **Warm Graphite (#37352F):** Primary text and headings, seen 101 times. Token `on-surface`, CSS `--tally-builder-text`.
- **Near Black (#000000):** Headings and emphasis, seen 33 times. Token `on-surface-strong`.
- **Warm Graphite (#45433E):** Secondary text, seen 31 times. Token `on-surface-variant`.
- **Slate (#777672):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Warm Graphite 9% (#37352F17):** Borders and dividers, seen 1 time. Token `outline`.
- **Vivid Blue (#0070D7):** Primary buttons and calls to action, seen 4 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Purple (#F81CE5):** Accent, seen 74 times. Token `secondary`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, Inter Fallback, sans-serif`.

- **headline-display:** Inter 64px at weight 700, line height 1, tracking -0.031em (26px on mobile). Page title (h1).
- **headline-lg:** Inter 36px at weight 700, line height 1.15 (20px on mobile). Section headings (h2).
- **headline-md:** Inter 22px at weight 500, line height 1.25. Sub-section headings.
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Inter 18px at weight 800, line height 1.15. Lead paragraphs.
- **body-sm:** Inter 14px at weight 400, line height 1. Secondary and small text.
- **label-lg:** Inter 16px at weight 600, line height 1.5. Large buttons and tabs.
- **label-md:** Inter 15px at weight 400, line height 1.8. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 65% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 64px.
- **Sections:** 100px vertical padding between major sections.
- **Gaps:** 8.4px is the most common gap in flex and grid layouts.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 450px, 576px, 758px, 992px, 1024px, 1200px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #37352F17 borders.

## Shapes

Most elements use 7px corners. Measured radii, most used first:

- **md (7px):** 32 elements.
- **sm (5px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Create form”):** #0070D7 fill, #FFFFFF text, 14px/400, 7px radius, padding 0px 9.8px.
- **link:** transparent fill, #37352F text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 4 levels: #37352F, #000000, #45433E, #777672.
- Do reserve #0070D7 for primary actions and key highlights.
- Do set headlines in Inter with tight tracking (-0.031em).
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do use 7px corners on most elements; larger surfaces also use 5px.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Inter.
- Don't use #0070D7 for large backgrounds or body text.
- Don't make interface transitions slower than 0.1s.

## Motion

Interface transitions are quick: 0.1s.

- **Easing:** `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/tally.so/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
