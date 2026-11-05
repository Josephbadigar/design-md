---
version: alpha
name: Icons8
description: "Light monochrome interface measured from icons8.com: Inter type, tonal surfaces and 16px corners."
colors:
  background: "#F7F7F7"
  surface: "#F7F7F7"
  on-surface: "#191919"
  on-background: "#191919"
  on-surface-strong: "#000000"
  surface-container-low: "#FCFCFC"
  surface-container: "#FFFFFF"
  overlay: "#0000001A"
  overlay-strong: "#00000047"
  outline: "#0000000D"
  primary: "#1A1A1A"
  on-primary: "#FFFFFF"
  secondary: "#0000EE"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.015em
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.004em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.021em
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.019em
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.006em
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
    letterSpacing: -0.007em
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.019em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.6
    letterSpacing: -0.005em
rounded:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 12px
  xl: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 18px
  xl: 64px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 8px 20px 8px 16px
    height: 48px
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "#FFFFFFE5"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 6px 15px
    height: 30px
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 4px 8px
    height: 26px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
  input-field:
    textColor: "{colors.on-surface}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 18px
  link:
    textColor: "{colors.on-surface}"
---

# Icons8 Design System

## Overview

Icons8 describes itself as: “Icons8: 1.5M+ free icons, illustrations and 3D for designers. SVG and PNG, in consistent styles by our own designers. MCP server for AI agents.” The interface is light, built on **Snow (#F7F7F7)** with **Charcoal (#191919)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Inter**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 16px.

Measured from [icons8.com](https://icons8.com/) on November 4, 2026 at 1440×900 and 390×844 from 348 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Snow (#F7F7F7):** Page background. Token `background`.
- **Charcoal (#191919):** Primary text and headings. Token `on-surface`, CSS `--c-text`.
- **Near Black (#000000):** Headings and emphasis, seen 2 times. Token `on-surface-strong`.
- **Snow (#FCFCFC):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **White (#FFFFFF):** Cards and panels, seen 32 times. Token `surface-container`.
- **Near Black 10% (#0000001A):** Translucent fill for cards and controls, seen 3 times. Token `overlay`, CSS `--i8-border-base-default`.
- **Near Black 28% (#00000047):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Near Black 5% (#0000000D):** Borders and dividers, seen 12 times. Token `outline`, CSS `--i8-border-primary-tertiary-hover`.
- **Charcoal (#1A1A1A):** Primary buttons and calls to action, seen 72 times. Token `primary`, CSS `--c-text`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#0000EE):** Accent in text, fills and borders, seen 51 times. Token `secondary`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, -apple-system, BlinkMacSystemFont, Segoe UI`.

- **headline-display:** Inter 40px at weight 600, line height 1.2, tracking -0.015em (32px on mobile). Page title (h1).
- **headline-lg:** Inter 24px at weight 600, line height 1.33, tracking -0.004em (20px on mobile). Section headings (h2).
- **body-md:** Inter 14px at weight 400, line height 1.5, tracking -0.021em. Body text.
- **body-lg:** Inter 16px at weight 400, line height 1.5, tracking -0.019em. Lead paragraphs.
- **body-sm:** Inter 12px at weight 400, line height 1.33. Secondary and small text.
- **label-md:** Inter 16px at weight 500, line height 1.5, tracking -0.006em. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 600, line height 1.43, tracking -0.007em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (77% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 18px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 380px, 480px, 500px, 639px, 768px, 800px, 1023px, 1024px, 1025px, 1200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 1px 1px 0px, rgba(0, 0, 0, 0.2) 0px 0px 1px 0px`
- `rgba(25, 24, 18, 0.08) 0px 2px 4px 0px`

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **xl (16px):** 96 elements.
- **sm (8px):** 88 elements.
- **full (9999px):** 44 elements.
- **xs (4px):** 12 elements.
- **md (10px):** 12 elements.
- **lg (12px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Connect your AI agent”):** #1A1A1A fill, #FFFFFF text, 14px/500, 8px radius, padding 8px 20px 8px 16px.
- **button-secondary (“Sign in”):** #1A1A1A fill, #FFFFFFE5 text, 14px/600, 8px radius, padding 6px 15px, border 1px solid #1A1A1A.
- **button-outline (“Free”):** #FFFFFF fill, #000000E5 text, 12px/400, 9999px radius, padding 4px 8px.
- **button-ghost (“Icons”):** transparent fill, #000000E5 text, 14px/600, 8px radius, padding 0px 12px.
- **input-field (“Search icons...”):** transparent fill, #000000E5 text, 18px/700, padding 0px.
- **card:** #FFFFFF fill, #000000E5 text, 14px/400, 16px radius, padding 18px, shadow `rgba(0, 0, 0, 0.1) 0px 1px 1px 0px, rgba(0, 0, 0, 0.2) 0px 0px 1px 0px`.
- **link:** transparent fill, #000000E5 text, padding 0px.

## Do's and Don'ts

- Do use #F7F7F7 for the page and lift surfaces in small steps: #FCFCFC, #FFFFFF.
- Do keep text in 2 levels: #191919, #000000.
- Do let contrast carry emphasis; primary actions use #1A1A1A on #F7F7F7.
- Do set headlines in Inter with tight tracking (-0.015em).
- Do reuse the measured spacing steps (8px, 16px, 18px).
- Do use 16px corners on most elements; larger surfaces also use 8px, 4px and 10px.
- Don't introduce new font families beyond Inter.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.1s, 0.15s, 0.16s.

- **Easing:** `ease-out`, `ease`, `cubic-bezier(0.23, 1, 0.32, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/icons8.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
