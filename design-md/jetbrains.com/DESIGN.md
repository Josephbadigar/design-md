---
version: alpha
name: JetBrains
description: "Dark interface measured from jetbrains.com: JetBrains Sans type, indigo accents, tonal surfaces and 8px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#B3B3B3"
  on-surface-muted: "#999999"
  surface-container-low: "#19191C"
  surface-container: "#303033"
  overlay: "#FFFFFF4D"
  overlay-strong: "#6B57FF80"
  outline: "#FFFFFF33"
  outline-variant: "#FFFFFF4D"
  primary: "#6B57FF"
  on-primary: "#FFFFFF"
  secondary: "#6F61D2"
  tertiary: "#F001A0"
typography:
  headline-display:
    fontFamily: JetBrains Sans
    fontSize: 72px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.005em
  headline-lg:
    fontFamily: JetBrains Sans
    fontSize: 43px
    fontWeight: 600
    lineHeight: 1.14
    letterSpacing: -0.001em
  headline-md:
    fontFamily: JetBrains Sans
    fontSize: 35px
    fontWeight: 600
    lineHeight: 1.2
  headline-sm:
    fontFamily: JetBrains Sans
    fontSize: 29px
    fontWeight: 300
    lineHeight: 1.34
  title-lg:
    fontFamily: JetBrains Sans
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
  body-md:
    fontFamily: JetBrains Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  body-sm:
    fontFamily: JetBrains Sans
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.54
    letterSpacing: 0.005em
  label-md:
    fontFamily: JetBrains Sans
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: JetBrains Sans
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.54
  headline-sm-mobile:
    fontFamily: JetBrains Sans
    fontSize: 23px
    fontWeight: 300
    lineHeight: 1.3
  headline-md-mobile:
    fontFamily: JetBrains Sans
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.14
rounded:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 26px
spacing:
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 96px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 20px
    padding: 8px 24px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.title-lg}"
    rounded: 0px
    padding: 0px 10px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.background}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
  link:
    textColor: "{colors.on-surface-variant}"
---

# JetBrains Design System

## Overview

JetBrains describes itself as: “JetBrains is a cutting-edge software vendor specializing in the creation of intelligent development tools, including IntelliJ IDEA – the leading Java IDE, and the Kotlin programming language.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Indigo (#6B57FF)** as the main accent.

Type is set in **JetBrains Sans**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [jetbrains.com](https://www.jetbrains.com/) on November 4, 2026 at 1440×900 and 390×844 from 429 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #5A1FD0, #39013E99.

- **Near Black (#000000):** Page background, seen 1 time. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 135 times. Token `on-surface`.
- **Gray (#B3B3B3):** Secondary text, seen 55 times. Token `on-surface-variant`, CSS `--rs-color-white-t70`.
- **Gray (#999999):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Charcoal (#19191C):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`, CSS `--wt-site-header-bg`.
- **Graphite (#303033):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--rs-color-grey-90`.
- **White 30% (#FFFFFF4D):** Translucent fill for cards and controls, seen 4 times. Token `overlay`, CSS `--rs-color-white-t30`.
- **Indigo 50% (#6B57FF80):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White 20% (#FFFFFF33):** Borders and dividers, seen 5 times. Token `outline`.
- **White 30% (#FFFFFF4D):** Secondary dividers, seen 4 times. Token `outline-variant`, CSS `--rs-color-white-t30`.
- **Indigo (#6B57FF):** Primary buttons and calls to action, seen 1 time. Token `primary`, CSS `--rs-color-primary-light-theme`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Indigo (#6F61D2):** Accent (CSS variable). Token `secondary`.
- **Vivid Pink (#F001A0):** Accent in the logo, seen 1 time. Token `tertiary`.

## Typography

**JetBrains Sans** carries the whole interface. Fallback stack: `JetBrains Sans, Inter, system-ui, -apple-system`. Other loaded fonts: JetBrains Modul.

- **headline-display:** JetBrains Sans 72px at weight 600, line height 1, tracking -0.005em. Page title (h1).
- **headline-lg:** JetBrains Sans 43px at weight 600, line height 1.14, tracking -0.001em. Section headings (h2).
- **headline-md:** JetBrains Sans 35px at weight 600, line height 1.2 (28px on mobile). Sub-section headings.
- **headline-sm:** JetBrains Sans 29px at weight 300, line height 1.34 (23px on mobile). Card and feature titles.
- **title-lg:** JetBrains Sans 20px at weight 400, line height 1.4. Small titles.
- **body-md:** JetBrains Sans 16px at weight 400, line height 1. Body text.
- **body-sm:** JetBrains Sans 13px at weight 400, line height 1.54, tracking 0.005em. Secondary and small text.
- **label-md:** JetBrains Sans 16px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** JetBrains Sans 13px at weight 600, line height 1.54. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (77% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** sm 8px, md 12px, lg 24px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#19191C → #303033) and hairline rings:

- `rgba(255, 255, 255, 0.1) 0px 0px 0px 1px inset`
- `rgba(255, 255, 255, 0.05) 0px 0px 0px 1px inset`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 68 elements.
- **md (16px):** 40 elements.
- **xl (26px):** 24 elements.
- **xs (4px):** 16 elements.
- **lg (24px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Explore Air”):** #19191C fill, #FFFFFF text, 16px/400, 20px radius, padding 8px 24px.
- **button-ghost (“Products”):** transparent fill, #FFFFFF text, 20px/400, padding 0px 10px.
- **card:** #303033 fill, #000000 text, 13.3333px/400, 8px radius, padding 12px 16px, shadow `rgba(255, 255, 255, 0.05) 0px 0px 0px 1px inset`.
- **link:** transparent fill, #FFFFFFB3 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #19191C, #303033.
- Do keep text in 3 levels: #FFFFFF, #B3B3B3, #999999.
- Do reserve #6B57FF for primary actions and key highlights.
- Do set headlines in JetBrains Sans with tight tracking (-0.005em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 16px, 26px and 4px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond JetBrains Sans.
- Don't use #6B57FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.1s, 0.15s, 0.2s.

- **Easing:** `ease`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/jetbrains.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
