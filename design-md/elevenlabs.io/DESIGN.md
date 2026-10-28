---
version: alpha
name: ElevenLabs
description: "Light monochrome interface measured from elevenlabs.io: Waldenburg type with Inter, tonal surfaces and pill-shaped controls."
colors:
  background: "#F5F3F1"
  surface: "#F5F3F1"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#777169"
  on-surface-muted: "#A59F97"
  surface-container-low: "#FDFCFC"
  surface-container: "#FFFFFF"
  primary: "#000000"
  on-primary: "#FFFFFF"
  secondary: "#0A59D2"
  tertiary: "#052F70"
  error: "#F41A2F"
typography:
  headline-display:
    fontFamily: Waldenburg
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.08
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Waldenburg
    fontSize: 36px
    fontWeight: 300
    lineHeight: 1.17
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.35
  body-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.47
    letterSpacing: 0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.01em
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.01em
  caption:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.38
  label-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.6
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.47
    letterSpacing: 0.01em
  headline-display-mobile:
    fontFamily: Waldenburg
    fontSize: 36px
    fontWeight: 300
    lineHeight: 1.17
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Waldenburg
    fontSize: 30px
    fontWeight: 300
    lineHeight: 1.2
rounded:
  sm: 2px
  md: 4px
  lg: 20px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 20px
  xl: 48px
  gutter: 8px
  section: 128px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 0px 16px
    height: 40px
  button-primary-hover:
    backgroundColor: "#44403B"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.caption}"
    rounded: "{rounded.full}"
    padding: 0px 12px
    height: 32px
  button-outline-hover:
    backgroundColor: "{colors.surface-container-low}"
  input-field:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 16px
    padding: 0px
  link:
    textColor: "{colors.primary}"
---

# ElevenLabs Design System

## Overview

ElevenLabs describes itself as: “Create lifelike speech with our AI voice generator and voice agents platform. Access 17,500+ voices in 90+ languages with secure APIs and SDKs.” The interface is light, built on **Mist (#F5F3F1)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Waldenburg** and **Inter**. Headlines run large with tight negative tracking; body text is 15px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [elevenlabs.io](https://elevenlabs.io/) on October 21, 2026 at 1440×900 and 401×868 from 453 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Mist (#F5F3F1):** Page background, seen 3 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 78 times. Token `on-surface`.
- **Warm Slate (#777169):** Secondary text, seen 37 times. Token `on-surface-variant`.
- **Warm Gray (#A59F97):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Snow (#FDFCFC):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **White (#FFFFFF):** Cards and panels, seen 20 times. Token `surface-container`.
- **Near Black (#000000):** Primary buttons and calls to action, seen 116 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0A59D2):** Most used accent color, seen 14 times. Token `secondary`.
- **Dark Blue (#052F70):** Most used accent color, seen 12 times. Token `tertiary`.
- **Vivid Red (#F41A2F):** Errors and destructive states, seen 9 times. Token `error`.

## Typography

**Waldenburg** and **Inter** share the interface. Fallback stack: `Waldenburg, Waldenburg Fallback`. Other loaded fonts: Inter Fallback, Geist Mono.

- **headline-display:** Waldenburg 48px at weight 300, line height 1.08, tracking -0.02em (36px on mobile). Page title (h1).
- **headline-lg:** Waldenburg 36px at weight 300, line height 1.17 (30px on mobile). Section headings (h2).
- **headline-md:** Inter 20px at weight 400, line height 1.35. Sub-section headings.
- **body-md:** Inter 15px at weight 400, line height 1.47, tracking 0.01em. Body text.
- **body-lg:** Inter 16px at weight 400, line height 1.5, tracking 0.01em. Lead paragraphs.
- **body-sm:** Inter 14px at weight 400, line height 1.5, tracking 0.01em. Secondary and small text.
- **caption:** Inter 13px at weight 400, line height 1.38. Captions and fine print.
- **label-lg:** Inter 18px at weight 400, line height 1.6. Large buttons and tabs.
- **label-md:** Inter 16px at weight 500, line height 1.5, tracking 0.01em. Buttons, navigation and labels.
- **label-sm:** Inter 15px at weight 500, line height 1.47, tracking 0.01em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 68% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 16px, lg 20px, xl 48px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgb(255, 255, 255) 0px 0px 0px 0px, rgba(0, 0, 0, 0.125) 0px 0px 0px 0.5px, rgba(0, 0, 0, 0.04) 0px 1px 1px 0px, rgba(0, 0, 0, 0.04) 0px 2px 4px 0px`
- `rgba(0, 0, 0, 0.1) 0px 0px 0px 0.5px, rgba(0, 0, 0, 0.04) 0px 1px 1px 0px, rgba(0, 0, 0, 0.04) 0px 2px 4px 0px`

Hairline rings and inset highlights also appear: `rgb(255, 255, 255) 0px 0px 0px 0px inset, rgb(215, 210, 204) 0px 0px 0px 0.5px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 140 elements.
- **md (4px):** 132 elements.
- **sm (2px):** 40 elements.
- **lg (20px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Accept all cookies”):** #000000 fill, #FFFFFF text, 15px/400, 9999px radius, padding 0px 16px.
- **button-primary-hover:** background #44403B, text #FFFFFF on hover.
- **button-outline (“Discover”):** #FFFFFF fill, #000000 text, 13px/400, 9999px radius, padding 0px 12px, shadow `rgb(255, 255, 255) 0px 0px 0px 0px, rgba(0, 0, 0, 0.125) 0px 0px 0px 0.5px, rgba(0, 0, 0, 0.04) 0px 1px 1px 0px, rgba(0, 0, 0, 0.04) 0px 2px 4px 0px`.
- **button-outline-hover:** background #FDFCFC, text #000000 on hover.
- **input-field:** #FFFFFF fill, #000000 text, 18px/400, padding 0px.
- **card:** #FFFFFF fill, #000000 text, 18px/400, 16px radius, padding 0px, shadow `rgb(255, 255, 255) 0px 0px 0px 0px, rgba(0, 0, 0, 0.125) 0px 0px 0px 0.5px, rgba(0, 0, 0, 0.04) 0px 1px 1px 0px, rgba(0, 0, 0, 0.04) 0px 2px 4px 0px`.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #F5F3F1 for the page and lift surfaces in small steps: #FDFCFC, #FFFFFF.
- Do keep text in 3 levels: #000000, #777169, #A59F97.
- Do let contrast carry emphasis; primary actions use #000000 on #F5F3F1.
- Do set headlines in Waldenburg with tight tracking (-0.02em).
- Do reuse the measured spacing steps (6px, 16px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't use #777169 for body text; it reaches 4.4:1 on #F5F3F1. Keep it for large text or metadata.
- Don't use #A59F97 for body text; it reaches 2.4:1 on #F5F3F1. Keep it for large text or metadata.
- Don't introduce new font families beyond Waldenburg and Inter.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/elevenlabs.io/), the free DESIGN.md generator.
