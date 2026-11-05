---
version: alpha
name: Remix
description: "Dark interface measured from remix.run: Inter type, red accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#DEE2E6"
  on-background: "#DEE2E6"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#C2C2C2"
  on-surface-muted: "#B8B8B8"
  surface-container-low: "#1E2226"
  overlay: "#FFFFFF06"
  overlay-strong: "#FFFFFF33"
  outline: "#7A74A11D"
  outline-variant: "#FFFFFF1A"
  primary: "#FE4754"
  on-primary: "#FFFFFF"
  secondary: "#2DACF9"
  tertiary: "#7CE95A"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 84px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Inter
    fontSize: 50px
    fontWeight: 700
    lineHeight: 1.04
    letterSpacing: -0.02em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: -0.015em
  label-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1
  code:
    fontFamily: JetBrains Mono
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 42px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.03em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.04
    letterSpacing: -0.02em
rounded:
  md: 13px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 14px
  lg: 32px
  xl: 48px
  gutter: 8px
  section: 160px
  margin: 36px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: 0px
    padding: 0px 18px
    height: 58px
  button-primary-hover:
    backgroundColor: "#9B7191"
  button-secondary:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    rounded: 0px
    padding: 4px 6px
    height: 24px
  button-secondary-hover:
    textColor: "#ED4643"
  button-outline:
    backgroundColor: "#FE6F7E27"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px 14px 1px 14px
    height: 38px
  button-ghost:
    backgroundColor: "#FFFFFF09"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 12px
  input-field:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 0px 18px
  link:
    textColor: "{colors.on-surface}"
---

# Remix Design System

## Overview

Remix describes itself as: “The fully-stacked web framework” The interface is dark, built on **Near Black (#000000)** with **Cool Mist (#DEE2E6)** text, and **Red (#FE4754)** as the main accent.

Type is set in **Inter**, with **JetBrains Mono** for code. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [remix.run](https://remix.run/) on November 4, 2026 at 1440×900 and 390×844 from 141 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Near Black (#000000):** Page background, seen 2 times. Token `background`.
- **Cool Mist (#DEE2E6):** Primary text and headings, seen 23 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 23 times. Token `on-surface-strong`.
- **Silver (#C2C2C2):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Silver (#B8B8B8):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Cool Charcoal (#1E2226):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **White 2% (#FFFFFF06):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **White 20% (#FFFFFF33):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Indigo 11% (#7A74A11D):** Borders and dividers, seen 12 times. Token `outline`.
- **White 10% (#FFFFFF1A):** Secondary dividers, seen 6 times. Token `outline-variant`.
- **Red (#FE4754):** Primary buttons and calls to action, seen 6 times. Token `primary`, CSS `--brand-cycle`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#2DACF9):** Accent on large areas, seen 6 times. Token `secondary`.
- **Green (#7CE95A):** Accent on large areas, seen 2 times. Token `tertiary`.

## Typography

**Inter** and **JetBrains Mono** (monospace) share the interface. Fallback stack: `Inter, Inter Fallback, ui-sans-serif, system-ui`.

- **headline-display:** Inter 84px at weight 700, line height 1, tracking -0.03em (42px on mobile). Page title (h1).
- **headline-lg:** Inter 50px at weight 700, line height 1.04, tracking -0.02em (32px on mobile). Section headings (h2).
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Inter 18px at weight 700, line height 1.3, tracking -0.015em. Lead paragraphs.
- **label-md:** Inter 13px at weight 500, line height 1. Buttons, navigation and labels.
- **code:** JetBrains Mono 16px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing does not follow a strict grid: 69% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 14px, lg 32px, xl 48px.
- **Sections:** 160px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 36px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#1E2226) and #7A74A11D borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 52 elements.
- **md (13px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“SERVER”):** #FE4754 fill, #FFFFFF text, 12px/500, padding 0px 18px.
- **button-primary-hover:** background #9B7191, text #FFFFFF on hover.
- **button-secondary (“[D] DOCS”):** #1E2226 fill, #DEE2E6 text, 12px/400, padding 4px 6px.
- **button-secondary-hover:** background #1E2226, text #ED4643 on hover.
- **button-outline (“Request”):** #FE6F7E27 fill, #FFFFFF text, 13px/500, 999px radius, padding 0px 14px 1px 14px, border 1px solid #FE4A5C85.
- **button-ghost (“npm”):** #FFFFFF09 fill, #FFFFFF text, 13px/500, 13px 0px 0px 13px radius, padding 0px 12px.
- **input-field (“name@example.com”):** transparent fill, #FFFFFF text, 16px/400, 999px radius, padding 0px 18px, border 1px solid #FFFFFF2E.
- **link:** transparent fill, #DEE2E6 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #1E2226.
- Do keep text in 4 levels: #DEE2E6, #FFFFFF, #C2C2C2, #B8B8B8.
- Do reserve #FE4754 for primary actions and key highlights.
- Do set headlines in Inter with tight tracking (-0.03em).
- Do reuse the measured spacing steps (6px, 14px, 32px).
- Do make buttons and chips fully rounded (9999px); most other elements use 13px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Inter and JetBrains Mono.
- Don't use #FE4754 for large backgrounds or body text.
- Don't make interface transitions slower than 0.16s.

## Motion

Interface transitions are quick: 0.16s, 0.15s. Longer ambient animations run 10s.

- **Easing:** `ease`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/remix.run/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
