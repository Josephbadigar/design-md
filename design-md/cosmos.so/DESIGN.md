---
version: alpha
name: Cosmos
description: "Light monochrome interface measured from cosmos.so: cosmosOracle type, tonal surfaces and pill-shaped controls."
colors:
  background: "#F7F5F3"
  surface: "#F7F5F3"
  on-surface: "#0D0D0D"
  on-background: "#0D0D0D"
  on-surface-variant: "#6E6A69"
  on-surface-muted: "#9A9796"
  surface-container-low: "#F2F1F0"
  surface-container: "#FCFBFA"
  surface-container-high: "#FFFFFF"
  surface-container-highest: "#E8E6E4"
  overlay: "#00000005"
  overlay-strong: "#FFFFFF66"
  outline: "#0D0D0D1F"
  outline-variant: "#FFFFFF"
  primary: "#0D0D0D"
  on-primary: "#FFFFFF"
  secondary: "#4694F6"
  error: "#A0213E"
  warning: "#EBB042"
typography:
  headline-display:
    fontFamily: cosmosOracle
    fontSize: 72px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: cosmosOracle
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.04em
  headline-md:
    fontFamily: cosmosOracle
    fontSize: 26px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.04em
  headline-sm:
    fontFamily: cosmosOracle
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.15
  body-md:
    fontFamily: cosmosOracle
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: cosmosOracle
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
  label-lg:
    fontFamily: cosmosOracle
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.02em
  label-md:
    fontFamily: cosmosOracle
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.47
    letterSpacing: -0.019em
  label-sm:
    fontFamily: cosmosOracle
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: -0.02em
  headline-display-mobile:
    fontFamily: cosmosOracle
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.04em
  headline-lg-mobile:
    fontFamily: cosmosOracle
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.04em
rounded:
  sm: 12px
  md: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  gutter: 8px
  margin: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    padding: 16px 24px
    height: 48px
  button-primary-hover:
    backgroundColor: "#232323"
  button-ghost:
    typography: "{typography.label-md}"
    padding: 16px 24px
  card:
    typography: "{typography.body-md}"
    padding: 0px 12px 0px 20px
  link:
    textColor: "#D0CDCD"
---

# Cosmos Design System

## Overview

Cosmos describes itself as: “Your space for inspiration” The interface is light, built on **Snow (#F7F5F3)** with **Charcoal (#0D0D0D)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **cosmosOracle**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [cosmos.so](https://www.cosmos.so/) on October 21, 2026 at 1440×900 and 390×844 from 354 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles.

- **Snow (#F7F5F3):** Page background, seen 3 times. Token `background`.
- **Charcoal (#0D0D0D):** Primary text and headings, seen 32 times. Token `on-surface`.
- **Slate (#6E6A69):** Secondary text, seen 9 times. Token `on-surface-variant`.
- **Gray (#9A9796):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Mist (#F2F1F0):** Raised areas one step from the page, seen 28 times. Token `surface-container-low`.
- **Snow (#FCFBFA):** Cards and panels, seen 2 times. Token `surface-container`.
- **White (#FFFFFF):** Hover and pressed fills, seen 35 times. Token `surface-container-high`.
- **Mist (#E8E6E4):** Highest raised elements, seen 1 time. Token `surface-container-highest`.
- **Near Black 2% (#00000005):** Translucent fill for cards and controls, seen 7 times. Token `overlay`.
- **White 40% (#FFFFFF66):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Charcoal 12% (#0D0D0D1F):** Borders and dividers, seen 18 times. Token `outline`.
- **White (#FFFFFF):** Secondary dividers, seen 11 times. Token `outline-variant`.
- **Charcoal (#0D0D0D):** Primary buttons and calls to action, seen 79 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#4694F6):** Accent, seen 1 time. Token `secondary`.
- **Dark Red (#A0213E):** Errors and destructive states, seen 1 time. Token `error`.
- **Vivid Orange (#EBB042):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**cosmosOracle** carries the whole interface. Fallback stack: `cosmosOracle, cosmosOracle Fallback`.

- **headline-display:** cosmosOracle 72px at weight 700, line height 1, tracking -0.04em (32px on mobile). Page title (h1).
- **headline-lg:** cosmosOracle 48px at weight 500, line height 1, tracking -0.04em (32px on mobile). Section headings (h2).
- **headline-md:** cosmosOracle 26px at weight 500, line height 1.15, tracking -0.04em. Sub-section headings.
- **headline-sm:** cosmosOracle 20px at weight 500, line height 1.15. Card and feature titles.
- **body-md:** cosmosOracle 16px at weight 400, line height 1.5. Body text.
- **body-sm:** cosmosOracle 14px at weight 400, line height 1.4. Secondary and small text.
- **label-lg:** cosmosOracle 16px at weight 500, line height 1.5, tracking -0.02em. Large buttons and tabs.
- **label-md:** cosmosOracle 15px at weight 500, line height 1.47, tracking -0.019em. Buttons, navigation and labels.
- **label-sm:** cosmosOracle 14px at weight 500, line height 1.43, tracking -0.02em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (83% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 720px, 768px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 8px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 3px 12px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.02) 0px 2px 12px 0px, rgba(0, 0, 0, 0.1) 0px 4px 16px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (16px):** 56 elements.
- **full (9999px):** 24 elements.
- **sm (12px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #0D0D0D fill, #FFFFFF text, 15px/500, 3.35544e+07px radius, padding 16px 24px.
- **button-primary-hover:** background #232323, text #FFFFFF on hover.
- **button-ghost (“Sign up”):** transparent fill, 15px/500, 3.35544e+07px radius, padding 16px 24px.
- **card:** transparent fill, 16px/400, 3.35544e+07px radius, padding 0px 12px 0px 20px.
- **link:** transparent fill, #D0CDCD text, padding 0px.

## Do's and Don'ts

- Do use #F7F5F3 for the page and lift surfaces in small steps: #F2F1F0, #FCFBFA, #FFFFFF, #E8E6E4.
- Do keep text in 3 levels: #0D0D0D, #6E6A69, #9A9796.
- Do let contrast carry emphasis; primary actions use #0D0D0D on #F7F5F3.
- Do set headlines in cosmosOracle with tight tracking (-0.04em).
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 16px corners.
- Don't use #9A9796 for body text; it reaches 2.7:1 on #F7F5F3. Keep it for large text or metadata.
- Don't introduce new font families beyond cosmosOracle.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.00001s.

## Motion

Interface transitions are quick: 1e-05s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cosmos.so/), the free DESIGN.md generator.
