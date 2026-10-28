---
version: alpha
name: Savee
description: "Dark monochrome interface measured from savee.com: saveeFont type, tonal surfaces and square corners."
colors:
  background: "#0A0A0A"
  surface: "#0A0A0A"
  on-surface: "#D4D4D4"
  on-background: "#D4D4D4"
  on-surface-strong: "#FAFAFA"
  on-surface-variant: "#9C9C9C"
  on-surface-muted: "#737373"
  surface-container-low: "#151515"
  outline: "#1E1E1E"
  primary: "#FDFDFD"
  on-primary: "#0A0A0A"
typography:
  headline-display:
    fontFamily: saveeFont
    fontSize: 80px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: saveeFont
    fontSize: 60px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.055em
  body-md:
    fontFamily: saveeFont
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.02em
  label-md:
    fontFamily: saveeFont
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: -0.01em
  headline-display-mobile:
    fontFamily: saveeFont
    fontSize: 34px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.035em
  headline-lg-mobile:
    fontFamily: saveeFont
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.055em
rounded:
  none: 0px
spacing:
  xs: 2px
  sm: 6px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 32px
  section: 50px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    padding: 0px 20px
    height: 40px
  button-ghost:
    typography: "{typography.label-md}"
    padding: 16px 12px
  link:
    textColor: "{colors.on-surface}"
---

# Savee Design System

## Overview

Savee describes itself as: “Savee is a curated place for visual inspiration. Discover references chosen by designers, collect what matters, and build a sharper eye without ads or clutter.” The interface is dark, built on **Near Black (#0A0A0A)** with **Silver (#D4D4D4)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **saveeFont**. Headlines run large with tight negative tracking; body text is 36px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are square.

Measured from [savee.com](https://savee.com/) on October 21, 2026 at 1440×900 and 390×844 from 228 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **Near Black (#0A0A0A):** Page background, seen 2 times. Token `background`.
- **Silver (#D4D4D4):** Primary text and headings, seen 24 times. Token `on-surface`.
- **Snow (#FAFAFA):** Headings and emphasis, seen 45 times. Token `on-surface-strong`.
- **Gray (#9C9C9C):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Slate (#737373):** Muted text and metadata, seen 9 times. Token `on-surface-muted`.
- **Charcoal (#151515):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **Charcoal (#1E1E1E):** Borders and dividers, seen 4 times. Token `outline`.
- **Snow (#FDFDFD):** Primary buttons and calls to action, seen 4 times. Token `primary`.
- **Near Black (#0A0A0A):** Text and icons on primary. Token `on-primary`.

## Typography

**saveeFont** carries the whole interface. Fallback stack: `saveeFont, saveeFont Fallback`. Other loaded fonts: saveeFont Fallback.

- **headline-display:** saveeFont 80px at weight 500, line height 1.05, tracking -0.035em (34px on mobile). Page title (h1).
- **headline-lg:** saveeFont 60px at weight 500, line height 1, tracking -0.055em (36px on mobile). Section headings (h2).
- **body-md:** saveeFont 36px at weight 500, line height 1.11, tracking -0.02em. Body text.
- **label-md:** saveeFont 16px at weight 400, line height 1.38, tracking -0.01em. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 61% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 12px, lg 24px, xl 40px.
- **Sections:** 50px vertical padding between major sections.
- **Gaps:** 32px is the most common gap in flex and grid layouts.
- **Breakpoints:** 600px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#151515) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(64, 64, 64) 0px 0px 0px 1.25px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

## Shapes

Corners are square. Measured radii, most used first:

- **none (0px):** measured.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Join for free”):** #FDFDFD fill, #0A0A0A text, 16px/550, 3.35544e+07px radius, padding 0px 20px.
- **button-ghost (“Log in”):** transparent fill, 16px/550, 3.35544e+07px radius, padding 16px 12px.
- **link:** transparent fill, #D4D4D4 text, padding 0px.

## Do's and Don'ts

- Do use #0A0A0A for the page and lift surfaces in small steps: #151515.
- Do keep text in 4 levels: #D4D4D4, #FAFAFA, #9C9C9C, #737373.
- Do let contrast carry emphasis; primary actions use #FDFDFD on #0A0A0A.
- Do set headlines in saveeFont with tight tracking (-0.035em).
- Do reuse the measured spacing steps (6px, 12px, 24px).
- Don't use #737373 for body text; it reaches 4.2:1 on #0A0A0A. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond saveeFont.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.35s.

## Motion

Interface transitions are quick: 0.15s, 0.18s, 0.35s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/savee.com/), the free DESIGN.md generator.
