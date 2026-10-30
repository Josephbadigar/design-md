---
version: alpha
name: Anthropic
description: "Light monochrome interface measured from anthropic.com: anthropicSans type with anthropicSerif, tonal surfaces and pill-shaped controls."
colors:
  background: "#F5F4ED"
  surface: "#F5F4ED"
  on-surface: "#141413"
  on-background: "#141413"
  on-surface-variant: "#30302E"
  on-surface-muted: "#5E5D59"
  on-surface-subtle: "#87867F"
  surface-container-low: "#FAF9F5"
  surface-container: "#FFFFFF"
  surface-container-high: "#E8E6DC"
  outline: "#DEDCD1"
  outline-variant: "#E8E6DC"
  primary: "#141413"
  on-primary: "#FAF9F5"
typography:
  display-hero:
    fontFamily: anthropicSans
    fontSize: 52px
    fontWeight: 600
    lineHeight: 1.08
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
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.53
  headline-display-mobile:
    fontFamily: anthropicSerif
    fontSize: 25px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.01em
  display-hero-mobile:
    fontFamily: anthropicSans
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.16
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
    padding: 12px 24px
    height: 36px
  button-outline:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 12px 20px 12px 24px
    height: 36px
  button-outline-hover:
    backgroundColor: "{colors.outline}"
    textColor: "{colors.on-surface}"
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "#3D3D3A"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 8px 16px
    height: 28px
  button-ghost-hover:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
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
    textColor: "{colors.on-surface-muted}"
---

# Anthropic Design System

## Overview

Anthropic describes itself as: “Anthropic is an AI safety and research company that's working to build reliable, interpretable, and steerable AI systems.” The interface is light, built on **Warm Mist (#F5F4ED)** with **Charcoal (#141413)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **anthropicSans** and **anthropicSerif**. Headlines run large with tight negative tracking; body text is 15px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [anthropic.com](https://www.anthropic.com/) on October 29, 2026 at 1440×900 and 390×844 from 257 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Warm Mist (#F5F4ED):** Page background, seen 14 times. Token `background`, CSS `--color-gray-100`.
- **Charcoal (#141413):** Primary text and headings, seen 19 times. Token `on-surface`.
- **Graphite (#30302E):** Secondary text, seen 6 times. Token `on-surface-variant`, CSS `--theme-foreground-secondary`.
- **Slate (#5E5D59):** Muted text and metadata, seen 18 times. Token `on-surface-muted`.
- **Warm Gray (#87867F):** Subtle text and placeholders, seen 10 times. Token `on-surface-subtle`, CSS `--color-slate-500`.
- **Snow (#FAF9F5):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`, CSS `--color-slate-050`.
- **White (#FFFFFF):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--color-slate-000`.
- **Warm Mist (#E8E6DC):** Hover and pressed fills, seen 10 times. Token `surface-container-high`, CSS `--color-slate-200`.
- **Warm Silver (#DEDCD1):** Borders and dividers, seen 11 times. Token `outline`.
- **Warm Mist (#E8E6DC):** Secondary dividers, seen 10 times. Token `outline-variant`, CSS `--color-slate-200`.
- **Charcoal (#141413):** Primary buttons and calls to action, seen 32 times. Token `primary`.
- **Snow (#FAF9F5):** Text and icons on primary. Token `on-primary`.

## Typography

**anthropicSans** and **anthropicSerif** share the interface. Fallback stack: `anthropicSans, anthropicSans Fallback, sans-serif`.

- **display-hero:** anthropicSans 52px at weight 600, line height 1.08 (32px on mobile). Oversized hero statements.
- **headline-display:** anthropicSerif 41px at weight 400, line height 1.25, tracking -0.01em (25px on mobile). Page title (h1).
- **headline-lg:** anthropicSans 21.5px at weight 700, line height 1.25. Section headings (h2).
- **body-md:** anthropicSans 15px at weight 400, line height 1.5. Body text.
- **body-sm:** anthropicSans 13px at weight 400, line height 1.54, tracking 0.01em. Secondary and small text.
- **caption:** anthropicSans 11px at weight 400, line height 1.5, tracking 0.018em. Captions and fine print.
- **label-md:** anthropicSans 17px at weight 400, line height 1.53. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 440px, 455px, 567px, 640px, 700px, 768px, 992px, 1024px, 1250px, 1280px, 1400px, 1512px, 1920px, 2160px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#FAF9F5 → #FFFFFF → #E8E6DC) and hairline rings:

- `rgb(250, 249, 245) 0px 0px 0px 2px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 56 elements.
- **md (10px):** 20 elements.
- **sm (8px):** 12 elements.
- **lg (16px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Learn more”):** #141413 fill, #FAF9F5 text, 16.6863px/400, 10px radius, padding 12px 24px, border 1px solid #141413.
- **button-outline (“Read announcement”):** #E8E6DC fill, #30302E text, 16.6863px/400, 10px radius, padding 12px 20px 12px 24px, border 1px solid #DEDCD1.
- **button-outline-hover:** background #DEDCD1, text #141413 on hover.
- **button-ghost (“News”):** #F5F4ED fill, #3D3D3A text, 13px/400, 999999px radius, padding 8px 16px, border 1px solid #E8E6DC.
- **button-ghost-hover:** background #E8E6DC, text #141413 on hover.
- **input-field (“Enter search...”):** #F5F4ED fill, #141413 text, 13px/400, 8px radius, padding 0px 16px 0px 36px, border 1px solid #E8E6DC.
- **card:** #F5F4ED fill, #141413 text, 16.6863px/400, padding 224px 0px.
- **link:** transparent fill, #5E5D59 text, padding 0px.

## Do's and Don'ts

- Do use #F5F4ED for the page and lift surfaces in small steps: #FAF9F5, #FFFFFF, #E8E6DC.
- Do keep text in 4 levels: #141413, #30302E, #5E5D59, #87867F.
- Do let contrast carry emphasis; primary actions use #141413 on #F5F4ED.
- Do set headlines in anthropicSans with tight tracking (-0.01em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 10px corners.
- Don't use #87867F for body text; it reaches 3.31:1 on #F5F4ED. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond anthropicSans and anthropicSerif.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.25s, 0.1s, 0.15s.

- **Easing:** `ease-in-out`, `ease`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/anthropic.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
