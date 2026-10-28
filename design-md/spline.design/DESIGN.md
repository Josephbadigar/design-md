---
version: alpha
name: Spline
description: "Dark monochrome interface measured from spline.design: Spline Sans type, flat surfaces and pill-shaped controls."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#999999"
  on-background: "#999999"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#E6E6E6"
  on-surface-muted: "#CCCCCC"
  overlay: "#FFFFFF1A"
  overlay-strong: "#FFFFFF26"
  outline: "#FFFFFF1A"
  outline-variant: "#FFFFFF0D"
  primary: "#999999"
  on-primary: "#000000"
  secondary: "#0062FF"
typography:
  headline-display:
    fontFamily: Spline Sans
    fontSize: 38.5px
    fontWeight: 500
    lineHeight: 1.25
  headline-lg:
    fontFamily: Spline Sans
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.22
  headline-md:
    fontFamily: Spline Sans
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.5
  headline-sm:
    fontFamily: Spline Sans
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.5
  body-md:
    fontFamily: Spline Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Spline Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-sm:
    fontFamily: Spline Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: Spline Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  label-sm:
    fontFamily: Spline Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.71
  headline-display-mobile:
    fontFamily: Spline Sans
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
  headline-lg-mobile:
    fontFamily: Spline Sans
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
rounded:
  sm: 8px
  md: 12px
  lg: 16px
  xl: 50px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 12px
  section: 180px
  container: 1080px
components:
  button-ghost:
    textColor: "#FFFFFFB3"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 10px 5px 10px 10px
  input-field:
    textColor: "{colors.on-surface-strong}"
    rounded: 0px
    padding: 2px 8px 0px 8px
---

# Spline Design System

## Overview

Spline describes itself as: “Spline is a free 3D design software with real-time collaboration to create web interactive experiences in the browser. Easy 3d modeling, animation, textures, and more.” The interface is dark, built on **Near Black (#000000)** with **Gray (#999999)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Spline Sans**. Headlines run large; body text is 14px. The surface language is flat. Controls are pill-shaped.

Measured from [spline.design](https://spline.design/) on October 21, 2026 at 1440×900 and 390×844 from 406 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Near Black (#000000):** Page background, seen 1 time. Token `background`, CSS `--color-bg`.
- **Gray (#999999):** Primary text and headings. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 17 times. Token `on-surface-strong`, CSS `--color-white`.
- **Mist (#E6E6E6):** Secondary text, seen 58 times. Token `on-surface-variant`, CSS `--color-white-090`.
- **Silver (#CCCCCC):** Muted text and metadata, seen 6 times. Token `on-surface-muted`, CSS `--color-white-080`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 29 times. Token `overlay`, CSS `--color-white-010`.
- **White 15% (#FFFFFF26):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 3 times. Token `outline`, CSS `--color-white-010`.
- **White 5% (#FFFFFF0D):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--color-btn-bg`.
- **Gray (#999999):** Primary actions (the main text color; the palette is monochrome). Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0062FF):** Most used accent color, seen 3 times. Token `secondary`, CSS `--color-blue`.

## Typography

**Spline Sans** carries the whole interface. Fallback stack: `Spline Sans, system-ui, -apple-system, BlinkMacSystemFont`. Other loaded fonts: Spline Sans Mono.

- **headline-display:** Spline Sans 38.5px at weight 500, line height 1.25 (32px on mobile). Page title (h1).
- **headline-lg:** Spline Sans 36px at weight 500, line height 1.22 (32px on mobile). Section headings (h2).
- **headline-md:** Spline Sans 24px at weight 400, line height 1.5. Sub-section headings.
- **headline-sm:** Spline Sans 20px at weight 500, line height 1.5. Card and feature titles.
- **body-md:** Spline Sans 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Spline Sans 18px at weight 400, line height 1.56. Lead paragraphs.
- **body-sm:** Spline Sans 12px at weight 400, line height 1.33. Secondary and small text.
- **label-md:** Spline Sans 16px at weight 400, line height 1.15. Buttons, navigation and labels.
- **label-sm:** Spline Sans 14px at weight 500, line height 1.71. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (73% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Sections:** 180px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1080px.
- **Breakpoints:** 400px, 500px, 530px, 600px, 625px, 720px, 768px, 780px, 800px, 820px, 850px, 870px, 960px, 1080px, 1160px, 1200px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #FFFFFF1A borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 104 elements.
- **md (12px):** 48 elements.
- **sm (8px):** 12 elements.
- **lg (16px):** 12 elements.
- **xl (50px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Products”):** transparent fill, #FFFFFFB3 text, 16px/400, padding 10px 5px 10px 10px.
- **input-field (“Describe what you want to create”):** transparent fill, #FFFFFF text, 15px/400, padding 2px 8px 0px 8px.

## Do's and Don'ts

- Do use #000000 for the page.
- Do keep text in 4 levels: #999999, #FFFFFF, #E6E6E6, #CCCCCC.
- Do let contrast carry emphasis; primary actions use #999999 on #000000.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 12px corners.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Spline Sans.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s.

- **Easing:** `ease`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/spline.design/), the free DESIGN.md generator.
