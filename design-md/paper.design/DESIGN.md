---
version: alpha
name: Paper
description: "Light monochrome interface measured from paper.design: Matter type, tonal surfaces and 4px corners."
colors:
  background: "#EFEFE4"
  surface: "#EFEFE4"
  on-surface: "#181818"
  on-background: "#181818"
  on-surface-variant: "#30302E"
  on-surface-muted: "#666666"
  on-surface-subtle: "#909090"
  surface-container-low: "#FCFCF9"
  outline: "#D7D7D6"
  primary: "#181818"
  on-primary: "#FCFCF9"
  secondary: "#81ADEC"
typography:
  headline-display:
    fontFamily: Matter
    fontSize: 48px
    fontWeight: 360
    lineHeight: 1
    letterSpacing: -0.02em
  body-md:
    fontFamily: Matter
    fontSize: 18px
    fontWeight: 550
    lineHeight: 1.56
    letterSpacing: 0.01em
  label-md:
    fontFamily: Matter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Matter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 2
    letterSpacing: 0.05em
  headline-display-mobile:
    fontFamily: Matter
    fontSize: 30px
    fontWeight: 360
    lineHeight: 1
    letterSpacing: -0.02em
rounded:
  md: 4px
spacing:
  xs: 4px
  sm: 8px
  md: 14px
  lg: 24px
  xl: 40px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 6px 14px
    height: 40px
  button-secondary:
    textColor: "#FFFFFF"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 7px 18px
    height: 42px
  button-ghost:
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 7px 18px
---

# Paper Design System

## Overview

Paper describes itself as: “Paper is a modern and powerful design tool that helps you create, share, and ship your best work.” The interface is light, built on **Warm Mist (#EFEFE4)** with **Charcoal (#181818)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Matter**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [paper.design](https://paper.design/) on November 4, 2026 at 1440×900 and 390×844 from 281 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles, plus gradient stops #93B8F0, #6DA1EE.

- **Warm Mist (#EFEFE4):** Page background, seen 3 times. Token `background`.
- **Charcoal (#181818):** Primary text and headings, seen 73 times. Token `on-surface`.
- **Graphite (#30302E):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Slate (#666666):** Muted text and metadata, seen 9 times. Token `on-surface-muted`.
- **Gray (#909090):** Subtle text and placeholders, seen 14 times. Token `on-surface-subtle`.
- **Snow (#FCFCF9):** Raised areas one step from the page, seen 21 times. Token `surface-container-low`.
- **Silver (#D7D7D6):** Borders and dividers, seen 18 times. Token `outline`.
- **Charcoal (#181818):** Primary buttons and calls to action, seen 76 times. Token `primary`.
- **Snow (#FCFCF9):** Text and icons on primary. Token `on-primary`.
- **Light Blue (#81ADEC):** Accent in text, fills and borders, seen 11 times. Token `secondary`.

## Typography

**Matter** carries the whole interface. Fallback stack: `Matter, system-ui`. Other loaded fonts: Inter, paperMono.

- **headline-display:** Matter 48px at weight 360, line height 1, tracking -0.02em (30px on mobile). Page title (h1).
- **body-md:** Matter 18px at weight 550, line height 1.56, tracking 0.01em. Body text.
- **label-md:** Matter 18px at weight 400, line height 1.56, tracking 0.01em. Buttons, navigation and labels.
- **label-sm:** Matter 14px at weight 500, line height 2, tracking 0.05em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (77% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 14px, lg 24px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 480px, 600px, 640px, 699px, 700px, 800px, 899px, 900px, 1079px, 1080px, 1140px, 1471px, 1600px, 1800px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.08) 0px 1px 0px 0px`
- `rgba(0, 0, 0, 0.12) 0px 16px 32px -16px, rgba(0, 0, 0, 0.08) 0px 8px 16px -8px, rgba(0, 0, 0, 0.04) 0px 4px 8px -4px, rgba(0, 0, 0, 0.02) 0px 2px 4px 0px, rgba(0, 0, 0, 0.08) 0px 0px 0px 1px`

Hairline rings and inset highlights also appear: `rgba(255, 255, 255, 0.12) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.12) 0px -1px 0px 0px inset`.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“download Paper”):** #181818 fill, #FCFCF9 text, 18px/480, 4px radius, padding 6px 14px.
- **button-secondary (“download for Linux”):** transparent fill, #FFFFFF text, 18px/480, 4px radius, padding 7px 18px, shadow `rgba(255, 255, 255, 0.12) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.12) 0px -1px 0px 0px inset`.
- **button-ghost (“download for Linux”):** transparent fill, 18px/480, 4px radius, padding 7px 18px, shadow `rgba(255, 255, 255, 0.12) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.12) 0px -1px 0px 0px inset`.

## Do's and Don'ts

- Do use #EFEFE4 for the page and lift surfaces in small steps: #FCFCF9.
- Do keep text in 4 levels: #181818, #30302E, #666666, #909090.
- Do let contrast carry emphasis; primary actions use #181818 on #EFEFE4.
- Do set headlines in Matter with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 14px, 24px).
- Do use 4px corners on most elements.
- Don't use #909090 for body text; it reaches 2.76:1 on #EFEFE4. Keep it for large text or metadata.
- Don't introduce new font families beyond Matter.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s, 0.1s.

- **Easing:** `ease`, `ease-out`, `cubic-bezier(0.16, 1, 0.3, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/paper.design/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
