---
version: alpha
name: Figma
description: "Light monochrome interface measured from figma.com: figmaSans type, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  overlay: "#FFFFFF3D"
  overlay-strong: "#00000014"
  outline: "#FFFFFF29"
  outline-variant: "#00000029"
  primary: "#000000"
  on-primary: "#FFFFFF"
  secondary: "#00B6FF"
typography:
  headline-display:
    fontFamily: figmaSans
    fontSize: 72px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: figmaSans
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.015em
  body-md:
    fontFamily: figmaSans
    fontSize: 18px
    fontWeight: 330
    lineHeight: 1.4
  body-lg:
    fontFamily: figmaSans
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.022em
  body-sm:
    fontFamily: figmaSans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.45
  label-md:
    fontFamily: figmaSans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.15
  code:
    fontFamily: figmaMono
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0.03em
  headline-display-mobile:
    fontFamily: figmaSans
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.01em
rounded:
  sm: 2px
  md: 8px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 40px
  gutter: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 12px 22px
    height: 46px
  button-primary-hover:
    backgroundColor: "#000000D9"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 8px
  link:
    textColor: "{colors.on-primary}"
---

# Figma Design System

## Overview

Figma describes itself as: “Figma is the canvas where design, code, and AI come together. From first idea to shipped product — go from concept to production with your whole team, in one place.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **figmaSans**, with **figmaMono** for code. Headlines run large with tight negative tracking; body text is 18px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [figma.com](https://www.figma.com/) on November 20, 2026 at 1440×900 and 390×844 from 461 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **White (#FFFFFF):** Page background, seen 9 times. Token `background`, CSS `--global-statsig-overlay`.
- **Near Black (#000000):** Primary text and headings, seen 58 times. Token `on-surface`, CSS `--fig-theme-btn-primary-bg`.
- **White 24% (#FFFFFF3D):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Near Black 8% (#00000014):** Stronger translucent fill, seen 2 times. Token `overlay-strong`, CSS `--fig-theme-form-input-bg`.
- **White 16% (#FFFFFF29):** Borders and dividers, seen 1 time. Token `outline`.
- **Near Black 16% (#00000029):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Near Black (#000000):** Primary buttons and calls to action, seen 122 times. Token `primary`, CSS `--fig-theme-btn-primary-bg`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Cyan (#00B6FF):** Accent, seen 1 time. Token `secondary`.

## Typography

**figmaSans** and **figmaMono** (monospace) share the interface. Fallback stack: `figmaSans, figmaSans Fallback, SF Pro Display, system-ui`.

- **headline-display:** figmaSans 72px at weight 400, line height 1, tracking -0.02em (44px on mobile). Page title (h1).
- **headline-lg:** figmaSans 44px at weight 400, line height 1.1, tracking -0.015em. Section headings (h2).
- **body-md:** figmaSans 18px at weight 330, line height 1.4. Body text.
- **body-lg:** figmaSans 30px at weight 400, line height 1.2, tracking -0.022em. Lead paragraphs.
- **body-sm:** figmaSans 16px at weight 400, line height 1.45. Secondary and small text.
- **label-md:** figmaSans 14px at weight 400, line height 1.15. Buttons, navigation and labels.
- **code:** figmaMono 16px at weight 400, line height 1.3, tracking 0.03em, uppercase. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (79% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 8px, md 16px, lg 20px, xl 40px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 320px, 480px, 559px, 560px, 768px, 960px, 1024px, 1280px, 1440px, 1600px, 1920px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `oklch(0 0 none / 0.16) 0px 0px 0px 1px inset`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 68 elements.
- **sm (2px):** 64 elements.
- **md (8px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Register”):** #000000 fill, #FFFFFF text, 16px/400, 8px radius, padding 12px 22px.
- **button-primary-hover:** background #000000D9, text #FFFFFF on hover.
- **button-ghost (“Products”):** transparent fill, #000000 text, 18px/330, padding 8px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do let contrast carry emphasis; primary actions use #000000 on #FFFFFF.
- Do set headlines in figmaSans with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 2px corners.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond figmaSans and figmaMono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.18s, 0.25s, 0.2s, 0.4s. Longer ambient animations run 2s, 8s.

- **Easing:** `ease-out`, `ease-in-out`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/figma.com/), the free DESIGN.md generator (engine 2026.10.29+f0c146f7cdfd).
