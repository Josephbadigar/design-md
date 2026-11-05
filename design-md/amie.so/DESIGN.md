---
version: alpha
name: Amie
description: "Light interface measured from amie.so: Inter type, vivid blue accents, tonal surfaces and 8px corners."
colors:
  background: "#FAFAFA"
  surface: "#FAFAFA"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#5C5C5C"
  on-surface-muted: "#A0A0A0"
  surface-container-low: "#FFFFFF"
  surface-container: "#EBEBEB"
  overlay: "#00000033"
  overlay-strong: "#FF61541A"
  outline: "#0000000D"
  primary: "#11A8FF"
  on-primary: "#FFFFFF"
  secondary: "#FF6154"
  tertiary: "#2C76A0"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.36
    letterSpacing: -0.013em
  headline-lg:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: -0.025em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.75
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.32
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.75
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
rounded:
  sm: 4px
  md: 8px
  lg: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 6px 16px
    height: 32px
  button-primary-hover:
    backgroundColor: "#218FCD"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 12px 28px
    height: 50px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 6px 10px
  link:
    textColor: "{colors.on-surface}"
---

# Amie Design System

## Overview

Amie describes itself as: “Turn meeting notes into automated workflows. Handle meetings, summaries, todos and emails (soon) with your AI personal assistant.” The interface is light, built on **Snow (#FAFAFA)** with **Near Black (#000000)** text, and **Vivid Blue (#11A8FF)** as the main accent.

Type is set in **Inter**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [amie.so](https://amie.so/) on November 4, 2026 at 1440×900 and 390×844 from 297 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Snow (#FAFAFA):** Page background, seen 1 time. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 85 times. Token `on-surface`.
- **Slate (#5C5C5C):** Secondary text, seen 47 times. Token `on-surface-variant`.
- **Gray (#A0A0A0):** Muted text and metadata, seen 8 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--tw-ring-offset-color`.
- **Mist (#EBEBEB):** Cards and panels, seen 3 times. Token `surface-container`.
- **Near Black 20% (#00000033):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Red 10% (#FF61541A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Near Black 5% (#0000000D):** Borders and dividers, seen 3 times. Token `outline`.
- **Vivid Blue (#11A8FF):** Primary buttons and calls to action, seen 7 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Red (#FF6154):** Accent in the logo, seen 2 times. Token `secondary`.
- **Blue (#2C76A0):** Accent in text, fills and borders, seen 2 times. Token `tertiary`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, Inter Fallback`.

- **headline-display:** Inter 40px at weight 700, line height 1.36, tracking -0.013em. Page title (h1).
- **headline-lg:** Inter 20px at weight 600, line height 1.4, tracking -0.025em. Section headings (h2).
- **body-md:** Inter 16px at weight 400, line height 1.75. Body text.
- **body-sm:** Inter 14px at weight 400, line height 1.5. Secondary and small text.
- **caption:** Inter 12px at weight 400, line height 1.32. Captions and fine print.
- **label-md:** Inter 16px at weight 600, line height 1.75. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (81% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 12px, lg 20px, xl 40px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 640px, 768px, 1024px, 1280px, 1536px, 2000px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#FFFFFF → #EBEBEB):

- `rgb(255, 255, 255) 0px 0px 0px 0px inset, rgba(0, 0, 0, 0.05) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.06) 0px 0px 0px 1px, rgba(0, 0, 0, 0.06) 0px 1px 1px -0.5px, rgba(0, 0, 0, 0.06) 0px 3px 3px -1.5px`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 46 elements.
- **lg (12px):** 20 elements.
- **full (9999px):** 16 elements.
- **sm (4px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #11A8FF fill, #FFFFFF text, 14px/500, 8px radius, padding 6px 16px.
- **button-primary-hover:** background #218FCD, text #FFFFFF on hover.
- **button-outline (“Download”):** #FFFFFF fill, #5C5C5C text, 16px/600, 12px radius, padding 12px 28px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.06) 0px 0px 0px 1px, rgba(0, 0, 0, 0.06) 0px 1px 1px -0.5px, rgba(0, 0, 0, 0.06) 0px 3px 3px -1.5px`.
- **button-ghost (“Features”):** transparent fill, #000000 text, 14px/500, 8px radius, padding 6px 10px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FAFAFA for the page and lift surfaces in small steps: #FFFFFF, #EBEBEB.
- Do keep text in 3 levels: #000000, #5C5C5C, #A0A0A0.
- Do reserve #11A8FF for primary actions and key highlights.
- Do set headlines in Inter with tight tracking (-0.013em).
- Do reuse the measured spacing steps (6px, 12px, 20px).
- Do use 8px corners on most elements; larger surfaces also use 12px and 4px.
- Don't use #A0A0A0 for body text; it reaches 2.51:1 on #FAFAFA. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Inter.
- Don't use #11A8FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/amie.so/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
