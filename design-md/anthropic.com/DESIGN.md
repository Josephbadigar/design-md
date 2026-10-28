---
version: alpha
name: Anthropic
description: "Dark monochrome interface measured from anthropic.com: anthropicSerif type with anthropicSans, tonal surfaces and pill-shaped controls."
colors:
  background: "#141413"
  surface: "#141413"
  on-surface: "#FAF9F5"
  on-background: "#FAF9F5"
  on-surface-variant: "#E8E6DC"
  on-surface-muted: "#87867F"
  on-surface-subtle: "#5E5D59"
  surface-container-low: "#262624"
  surface-container: "#3B3B3B"
  overlay: "#1414134D"
  outline: "#3D3D3A"
  primary: "#E8E6DC"
  on-primary: "#30302E"
  inverse-surface: "#F5F4ED"
typography:
  headline-display:
    fontFamily: anthropicSerif
    fontSize: 41px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: anthropicSans
    fontSize: 21.5px
    fontWeight: 700
    lineHeight: 1.25
  body-md:
    fontFamily: anthropicSans
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: anthropicSans
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.54
    letterSpacing: 0.01em
  caption:
    fontFamily: anthropicSans
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.018em
  label-md:
    fontFamily: anthropicSans
    fontSize: 16.5px
    fontWeight: 400
    lineHeight: 1.53
  label-sm:
    fontFamily: anthropicSans
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.54
    letterSpacing: 0.01em
  headline-display-mobile:
    fontFamily: anthropicSerif
    fontSize: 25px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.01em
rounded:
  sm: 8px
  md: 10px
  lg: 16px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 48px
  gutter: 8px
  section: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 12px 20px 12px 24px
    height: 36px
  button-primary-hover:
    backgroundColor: "#DEDCD1"
    textColor: "{colors.background}"
  button-secondary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.outline}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 8px 16px
    height: 28px
  button-tertiary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
  input-field:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 16px 0px 36px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 224px 0px
  link:
    textColor: "{colors.on-surface-subtle}"
---

# Anthropic Design System

## Overview

Anthropic describes itself as: “Anthropic is an AI safety and research company that's working to build reliable, interpretable, and steerable AI systems.” The interface is dark, built on **Charcoal (#141413)** with **Snow (#FAF9F5)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **anthropicSerif** and **anthropicSans**. Headlines run large with tight negative tracking; body text is 15px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [anthropic.com](https://www.anthropic.com/) on October 21, 2026 at 1440×900 and 390×844 from 274 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Charcoal (#141413):** Page background, seen 4 times. Token `background`.
- **Snow (#FAF9F5):** Primary text and headings, seen 20 times. Token `on-surface`, CSS `--color-slate-050`.
- **Warm Mist (#E8E6DC):** Secondary text, seen 2 times. Token `on-surface-variant`, CSS `--color-slate-200`.
- **Warm Gray (#87867F):** Muted text and metadata, seen 10 times. Token `on-surface-muted`, CSS `--color-slate-500`.
- **Slate (#5E5D59):** Subtle text and placeholders, seen 9 times. Token `on-surface-subtle`.
- **Graphite (#262624):** Raised areas one step from the page, seen 10 times. Token `surface-container-low`.
- **Graphite (#3B3B3B):** Cards and panels, seen 1 time. Token `surface-container`.
- **Charcoal 30% (#1414134D):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Graphite (#3D3D3A):** Borders and dividers, seen 19 times. Token `outline`.
- **Warm Mist (#E8E6DC):** Primary buttons and calls to action, seen 17 times. Token `primary`, CSS `--color-slate-200`.
- **Graphite (#30302E):** Text and icons on primary. Token `on-primary`.
- **Warm Mist (#F5F4ED):** High-contrast fills, seen 12 times. Token `inverse-surface`, CSS `--color-gray-100`.

## Typography

**anthropicSerif** and **anthropicSans** share the interface. Fallback stack: `anthropicSerif, anthropicSerif Fallback, serif`. Other loaded fonts: anthropicSans Fallback, anthropicSerif Fallback.

- **headline-display:** anthropicSerif 41px at weight 400, line height 1.25, tracking -0.01em (25px on mobile). Page title (h1).
- **headline-lg:** anthropicSans 21.5px at weight 700, line height 1.25. Section headings (h2).
- **body-md:** anthropicSans 15px at weight 400, line height 1.5. Body text.
- **body-sm:** anthropicSans 13px at weight 400, line height 1.54, tracking 0.01em. Secondary and small text.
- **caption:** anthropicSans 11px at weight 400, line height 1.5, tracking 0.018em. Captions and fine print.
- **label-md:** anthropicSans 16.5px at weight 400, line height 1.53. Buttons, navigation and labels.
- **label-sm:** anthropicSans 13px at weight 700, line height 1.54, tracking 0.01em. Small labels and badges.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 440px, 567px, 700px, 768px, 992px, 1024px, 1100px, 1250px, 1280px, 1400px, 1512px, 1920px, 2160px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#262624 → #3B3B3B) and hairline rings:

- `rgb(250, 249, 245) 0px 0px 0px 2px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 68 elements.
- **sm (8px):** 36 elements.
- **md (10px):** 20 elements.
- **lg (16px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Read announcement”):** #E8E6DC fill, #30302E text, 16.3725px/400, 10px radius, padding 12px 20px 12px 24px, border 1px solid #DEDCD1.
- **button-primary-hover:** background #DEDCD1, text #141413 on hover.
- **button-secondary (“News”):** #F5F4ED fill, #3D3D3A text, 13px/400, 999999px radius, padding 8px 16px, border 1px solid #E8E6DC.
- **button-tertiary (“Accept all cookies”):** #FAF9F5 fill, #141413 text, 16.3725px/400, 8px radius, padding 8px 16px, border 1px solid #FAF9F5.
- **button-ghost (“Customize  cookie settings”):** transparent fill, #FAF9F5 text, 16.3725px/400, 8px radius, padding 8px 16px, border 1px solid #FAF9F5.
- **input-field (“Enter search...”):** #F5F4ED fill, #141413 text, 13px/400, 8px radius, padding 0px 16px 0px 36px, border 1px solid #E8E6DC.
- **card:** #141413 fill, #FAF9F5 text, 16.3725px/400, padding 224px 0px.
- **link:** transparent fill, #5E5D59 text, padding 0px.

## Do's and Don'ts

- Do use #141413 for the page and lift surfaces in small steps: #262624, #3B3B3B.
- Do keep text in 4 levels: #FAF9F5, #E8E6DC, #87867F, #5E5D59.
- Do let contrast carry emphasis; primary actions use #E8E6DC on #141413.
- Do set headlines in anthropicSerif with tight tracking (-0.01em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't use #5E5D59 for body text; it reaches 2.8:1 on #141413. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond anthropicSerif and anthropicSans.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.1s, 0.25s.

- **Easing:** `ease-in-out`, `ease`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/anthropic.com/), the free DESIGN.md generator.
