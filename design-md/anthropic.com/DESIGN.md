---
version: alpha
name: Anthropic
description: "Dark monochrome interface measured from anthropic.com: anthropicSerif type with anthropicSans, tonal surfaces and pill-shaped controls."
colors:
  background: "#141413"
  surface: "#141413"
  on-surface: "#87867F"
  on-background: "#87867F"
  on-surface-strong: "#FAF9F5"
  on-surface-variant: "#B0AEA5"
  on-surface-muted: "#5E5D59"
  surface-container-low: "#262624"
  surface-container: "#30302E"
  overlay: "#1414134D"
  outline: "#3D3D3A"
  outline-variant: "#30302E"
  primary: "#E8E6DC"
  on-primary: "#30302E"
  inverse-surface: "#F5F4ED"
typography:
  headline-display:
    fontFamily: anthropicSerif
    fontSize: 70px
    fontWeight: 500
    lineHeight: 1
  headline-lg:
    fontFamily: anthropicSerif
    fontSize: 41px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.01em
  headline-md:
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
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.53
  headline-lg-mobile:
    fontFamily: anthropicSerif
    fontSize: 25px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.01em
  headline-display-mobile:
    fontFamily: anthropicSerif
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.12
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
  gutter: 16px
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
  button-secondary-hover:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.background}"
  button-tertiary:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 12px 24px
    height: 36px
  input-field:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 16px 0px 36px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 224px 0px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Anthropic Design System

## Overview

Anthropic describes itself as: “Anthropic is an AI safety and research company that's working to build reliable, interpretable, and steerable AI systems.” The interface is dark, built on **Charcoal (#141413)** with **Warm Gray (#87867F)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **anthropicSerif** and **anthropicSans**. Headlines run large; body text is 15px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [anthropic.com](https://www.anthropic.com/) on November 16, 2026 at 1440×900 and 390×844 from 268 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Charcoal (#141413):** Page background, seen 3 times. Token `background`.
- **Warm Gray (#87867F):** Primary text and headings, seen 10 times. Token `on-surface`, CSS `--color-slate-500`.
- **Snow (#FAF9F5):** Headings and emphasis, seen 9 times. Token `on-surface-strong`, CSS `--color-slate-050`.
- **Warm Gray (#B0AEA5):** Secondary text, seen 2 times. Token `on-surface-variant`, CSS `--color-gray-400`.
- **Slate (#5E5D59):** Muted text and metadata, seen 18 times. Token `on-surface-muted`.
- **Graphite (#262624):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Graphite (#30302E):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--theme-foreground-secondary`.
- **Charcoal 30% (#1414134D):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Graphite (#3D3D3A):** Borders and dividers, seen 10 times. Token `outline`.
- **Graphite (#30302E):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--theme-foreground-secondary`.
- **Warm Mist (#E8E6DC):** Primary buttons and calls to action, seen 19 times. Token `primary`, CSS `--color-slate-200`.
- **Graphite (#30302E):** Text and icons on primary. Token `on-primary`.
- **Warm Mist (#F5F4ED):** High-contrast fills, seen 12 times. Token `inverse-surface`, CSS `--color-gray-100`.

## Typography

**anthropicSerif** and **anthropicSans** share the interface. Fallback stack: `anthropicSerif, anthropicSerif Fallback, serif`.

- **headline-display:** anthropicSerif 70px at weight 500, line height 1 (48px on mobile). Page title (h1).
- **headline-lg:** anthropicSerif 41px at weight 400, line height 1.25, tracking -0.01em (25px on mobile). Section headings (h2).
- **headline-md:** anthropicSans 21.5px at weight 700, line height 1.25. Sub-section headings.
- **body-md:** anthropicSans 15px at weight 400, line height 1.5. Body text.
- **body-sm:** anthropicSans 13px at weight 400, line height 1.54, tracking 0.01em. Secondary and small text.
- **caption:** anthropicSans 11px at weight 400, line height 1.5, tracking 0.018em. Captions and fine print.
- **label-md:** anthropicSans 17px at weight 400, line height 1.53. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 440px, 455px, 567px, 640px, 700px, 768px, 992px, 1024px, 1250px, 1280px, 1512px, 1920px, 2160px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#262624 → #30302E) and hairline rings:

- `rgb(250, 249, 245) 0px 0px 0px 2px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 56 elements.
- **md (10px):** 24 elements.
- **sm (8px):** 12 elements.
- **lg (16px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Read announcement”):** #E8E6DC fill, #30302E text, 16.6863px/400, 10px radius, padding 12px 20px 12px 24px, border 1px solid #DEDCD1.
- **button-primary-hover:** background #DEDCD1, text #141413 on hover.
- **button-secondary (“News”):** #F5F4ED fill, #3D3D3A text, 13px/400, 999999px radius, padding 8px 16px, border 1px solid #E8E6DC.
- **button-secondary-hover:** background #E8E6DC, text #141413 on hover.
- **button-tertiary (“Read more”):** #FAF9F5 fill, #141413 text, 16.6863px/400, 10px radius, padding 12px 24px, border 1px solid #FAF9F5.
- **input-field (“Enter search...”):** #F5F4ED fill, #141413 text, 13px/400, 8px radius, padding 0px 16px 0px 36px, border 1px solid #E8E6DC.
- **card:** #141413 fill, #FAF9F5 text, 16.6863px/400, padding 224px 0px.
- **link:** transparent fill, #5E5D59 text, padding 0px.

## Do's and Don'ts

- Do use #141413 for the page and lift surfaces in small steps: #262624, #30302E.
- Do keep text in 4 levels: #87867F, #FAF9F5, #B0AEA5, #5E5D59.
- Do let contrast carry emphasis; primary actions use #E8E6DC on #141413.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 10px corners.
- Don't use #5E5D59 for body text; it reaches 2.80:1 on #141413. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond anthropicSerif and anthropicSans.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.25s, 0.1s. Longer ambient animations run 0.7s.

- **Easing:** `ease`, `ease-out`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/anthropic.com/), the free DESIGN.md generator (engine 2026.10.29+f0c146f7cdfd).
