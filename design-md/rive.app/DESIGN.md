---
version: alpha
name: Rive
description: "Dark monochrome interface measured from rive.app: Orbitron type with Inter, flat surfaces and 1.5px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#D9D9D9"
  on-surface-muted: "#CCCCCC"
  on-surface-subtle: "#BFBFBF"
  overlay: "#FFFFFF0D"
  overlay-strong: "#FFFFFF4D"
  outline: "#FFFFFF1A"
  outline-variant: "#FFFFFF4D"
  primary: "#E6E6E6"
  on-primary: "#000000"
  inverse-surface: "#FFFFFFE6"
  secondary: "#71FF19"
typography:
  headline-display:
    fontFamily: Orbitron
    fontSize: 48px
    fontWeight: 900
    lineHeight: 1.02
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Orbitron
    fontSize: 34px
    fontWeight: 900
    lineHeight: 1.08
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.55
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.55
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.2
  label-md:
    fontFamily: Tomorrow
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.2
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: 0.08em
  headline-display-mobile:
    fontFamily: Orbitron
    fontSize: 32px
    fontWeight: 900
    lineHeight: 1.02
    letterSpacing: -0.03em
  headline-lg-mobile:
    fontFamily: Orbitron
    fontSize: 26px
    fontWeight: 900
    lineHeight: 1.08
    letterSpacing: -0.01em
rounded:
  sm: 1.5px
  md: 4px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 20px
  xl: 60px
  gutter: 16px
  section: 60px
  margin: 40px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 5px 9px 6px 9px
    height: 29px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 5px 9px 6px 9px
    height: 27px
  button-secondary-hover:
    backgroundColor: "#DFE0E3"
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 0px
  input-field:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 14px
  link:
    textColor: "#999999"
---

# Rive Design System

## Overview

Rive describes itself as: “Behind Duolingo and Spotify Wrapped. Build games, UI, and interactive animation in the Rive Editor or with your coding agent and the Rive CLI.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Orbitron** and **Inter**. Headlines run large with tight negative tracking; body text is 15px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 1.5px.

Measured from [rive.app](https://rive.app/) on October 29, 2026 at 1440×900 and 390×844 from 371 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #F30058, #FF483C, #FFA41C, #71FF19.

- **Near Black (#000000):** Page background, seen 2 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 79 times. Token `on-surface`.
- **Silver (#D9D9D9):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Silver (#CCCCCC):** Muted text and metadata, seen 11 times. Token `on-surface-muted`.
- **Silver (#BFBFBF):** Subtle text and placeholders, seen 5 times. Token `on-surface-subtle`.
- **White 5% (#FFFFFF0D):** Translucent fill for cards and controls, seen 20 times. Token `overlay`.
- **White 30% (#FFFFFF4D):** Stronger translucent fill, seen 12 times. Token `overlay-strong`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 22 times. Token `outline`.
- **White 30% (#FFFFFF4D):** Secondary dividers, seen 22 times. Token `outline-variant`.
- **Mist (#E6E6E6):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **White 90% (#FFFFFFE6):** High-contrast fills, seen 3 times. Token `inverse-surface`.
- **Vivid Green (#71FF19):** Accent, seen 1 time. Token `secondary`.

## Typography

**Orbitron**, **Inter** and **Tomorrow** share the interface. Fallback stack: `Orbitron, Orbitron Placeholder, sans-serif`. Other loaded fonts: PragmataPro VF Variable Regular.

- **headline-display:** Orbitron 48px at weight 900, line height 1.02, tracking -0.03em, uppercase (32px on mobile). Page title (h1).
- **headline-lg:** Orbitron 34px at weight 900, line height 1.08, tracking -0.01em, uppercase (26px on mobile). Section headings (h2).
- **headline-md:** Inter 24px at weight 500, line height 1.25, tracking -0.01em. Sub-section headings.
- **body-md:** Inter 15px at weight 400, line height 1.55. Body text.
- **body-lg:** Inter 16px at weight 400, line height 1.55. Lead paragraphs.
- **label-lg:** Inter 16px at weight 500, line height 1.2. Large buttons and tabs.
- **label-md:** Tomorrow 14px at weight 500, line height 1.2. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 500, line height 1.3, tracking 0.08em, uppercase. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 39% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 16px, lg 20px, xl 60px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 389px, 600px, 639px, 640px, 640.98px, 641px, 949px, 949.98px, 1280px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgba(255, 255, 255, 0.1) 0px 0px 0px 1px inset`
- `rgba(236, 237, 240, 0.7) 0px 1px 0px 0px inset`
- `rgba(255, 255, 255, 0.15) 0px 0px 0px 1px inset`

## Shapes

Most elements use 1.5px corners. Measured radii, most used first:

- **sm (1.5px):** 140 elements.
- **md (4px):** 100 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“COPY”):** #FFFFFFE6 fill, #000000 text, 12px/500, 4px radius, padding 5px 9px 6px 9px, border 1px solid #FFFFFF.
- **button-primary-hover:** background #FFFFFF, text #000000 on hover.
- **button-secondary (“GET STARTED”):** #FFFFFF fill, #000000 text, 12px/500, 4px radius, padding 5px 9px 6px 9px, shadow `rgba(255, 255, 255, 0.1) 0px 0px 0px 1px inset`.
- **button-secondary-hover:** background #DFE0E3, text #000000 on hover.
- **button-ghost (“PRODUCTS”):** transparent fill, #FFFFFFD9 text, 12px/500, padding 0px.
- **input-field (“email@rive.app”):** #FFFFFF0D fill, #FFFFFF text, 15px/400, 4px radius, padding 0px 14px, shadow `rgba(255, 255, 255, 0.15) 0px 0px 0px 1px inset`.
- **link:** transparent fill, #999999 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page.
- Do keep text in 4 levels: #FFFFFF, #D9D9D9, #CCCCCC, #BFBFBF.
- Do let contrast carry emphasis; primary actions use #E6E6E6 on #000000.
- Do set headlines in Orbitron with tight tracking (-0.03em).
- Do reuse the measured spacing steps (6px, 16px, 20px).
- Do use 1.5px corners on most elements; larger surfaces also use 4px.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond Orbitron, Inter and Tomorrow.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.25s, 0.3s. Longer ambient animations run 6s, 1.4s.

- **Easing:** `ease`, `linear`, `cubic-bezier(0.44, 0, 0.56, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/rive.app/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
