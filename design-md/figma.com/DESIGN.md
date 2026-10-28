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
  overlay-strong: "#0000000A"
  outline: "#FFFFFF29"
  outline-variant: "#00000029"
  primary: "#000000"
  on-primary: "#FFFFFF"
  secondary: "#00B6FF"
  success: "#24CB71"
  error: "#FF3737"
typography:
  headline-display:
    fontFamily: figmaSans
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.022em
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
  label-md:
    fontFamily: figmaSans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.45
  code:
    fontFamily: figmaMono
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0.03em
  headline-display-mobile:
    fontFamily: figmaSans
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.035em
  headline-lg-mobile:
    fontFamily: figmaSans
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.021em
rounded:
  sm: 2px
  md: 8px
  lg: 16px
  xl: 24px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 32px
  section: 80px
  container: 650px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px 22px
    height: 46px
  button-primary-hover:
    backgroundColor: "#000000D9"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 12px 22px
    height: 46px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-primary}"
---

# Figma Design System

## Overview

Figma describes itself as: “Figma is the canvas where design, code, and AI come together. From first idea to shipped product — go from concept to production with your whole team, in one place.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **figmaSans**, with **figmaMono** for code. Headlines run large with tight negative tracking; body text is 18px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [figma.com](https://www.figma.com/) on October 21, 2026 at 1440×900 and 390×844 from 423 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 11 times. Token `background`, CSS `--global-statsig-overlay`.
- **Near Black (#000000):** Primary text and headings, seen 53 times. Token `on-surface`, CSS `--fig-theme-btn-primary-bg`.
- **White 24% (#FFFFFF3D):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Near Black 4% (#0000000A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White 16% (#FFFFFF29):** Borders and dividers, seen 1 time. Token `outline`.
- **Near Black 16% (#00000029):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Near Black (#000000):** Primary buttons and calls to action, seen 98 times. Token `primary`, CSS `--fig-theme-btn-primary-bg`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Cyan (#00B6FF):** Accent, seen 1 time. Token `secondary`.
- **Green (#24CB71):** Success and positive states, seen 1 time. Token `success`.
- **Vivid Red (#FF3737):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**figmaSans** and **figmaMono** (monospace) share the interface. Fallback stack: `figmaSans, figmaSans Fallback, SF Pro Display, system-ui`. Other loaded fonts: figmaSans Fallback, figmaMono Fallback.

- **headline-display:** figmaSans 56px at weight 400, line height 1, tracking -0.022em (36px on mobile). Page title (h1).
- **headline-lg:** figmaSans 44px at weight 400, line height 1.1, tracking -0.015em (32px on mobile). Section headings (h2).
- **body-md:** figmaSans 18px at weight 330, line height 1.4. Body text.
- **body-lg:** figmaSans 30px at weight 400, line height 1.2, tracking -0.022em. Lead paragraphs.
- **label-md:** figmaSans 16px at weight 400, line height 1.45. Buttons, navigation and labels.
- **code:** figmaMono 16px at weight 400, line height 1.3, tracking 0.03em. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (76% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 8px, md 12px, lg 20px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 32px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 650px.
- **Breakpoints:** 320px, 480px, 559px, 560px, 768px, 960px, 1024px, 1280px, 1440px, 1600px, 1920px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `oklch(0 0 none / 0.16) 0px 0px 0px 1px inset`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (2px):** 60 elements.
- **full (9999px):** 28 elements.
- **md (8px):** 16 elements.
- **lg (16px):** 4 elements.
- **xl (24px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started for free”):** #000000 fill, #FFFFFF text, 18px/330, 8px radius, padding 12px 22px.
- **button-primary-hover:** background #000000D9, text #FFFFFF on hover.
- **button-outline (“Allow all cookies”):** #FFFFFF fill, #000000 text, 16px/400, 8px radius, padding 12px 22px.
- **button-ghost (“Cookies settings”):** transparent fill, #FFFFFF text, 18px/330, padding 0px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do let contrast carry emphasis; primary actions use #000000 on #FFFFFF.
- Do set headlines in figmaSans with tight tracking (-0.022em).
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 2px corners.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond figmaSans and figmaMono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.18s, 0.25s, 0.4s.

- **Easing:** `ease-out`, `ease`, `cubic-bezier(0.8, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/figma.com/), the free DESIGN.md generator.
