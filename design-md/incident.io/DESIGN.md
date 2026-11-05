---
version: alpha
name: incident.io
description: "Light interface measured from incident.io: STKBureauSerif type with STKBureauSans, vivid red accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#161618"
  on-background: "#161618"
  on-surface-strong: "#000000"
  on-surface-variant: "#111827"
  on-surface-muted: "#6D6D70"
  surface-container-low: "#F8F5F0"
  surface-container: "#F3F3F4"
  surface-container-high: "#E8E8EA"
  surface-container-highest: "#D6D6D8"
  overlay: "#F25533B3"
  overlay-strong: "#0000000D"
  outline: "#F1EBE2"
  outline-variant: "#E8E8EA"
  primary: "#F25533"
  on-primary: "#F7F7F8"
  secondary: "#3A5BD9"
  tertiary: "#FF5F57"
  error: "#9B1C1C"
typography:
  headline-display:
    fontFamily: STKBureauSerif
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: STKBureauSerif
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-md:
    fontFamily: STKBureauSerif
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: -0.025em
  headline-sm:
    fontFamily: STKBureauSans
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: -0.01em
  body-md:
    fontFamily: STKBureauSans
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: -0.01em
  body-sm:
    fontFamily: STKBureauSans
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.01em
  caption:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: STKBureauSans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: STKBureauSans
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: -0.01em
  label-sm:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: 600
    lineHeight: 1.48
  headline-display-mobile:
    fontFamily: STKBureauSerif
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: -0.025em
rounded:
  sm: 6px
  md: 8px
  lg: 12px
spacing:
  xs: 3px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 48px
  gutter: 8px
  section: 96px
  container: 1192px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    padding: 12px 20px
    height: 49px
  button-primary-hover:
    backgroundColor: "#DD340D"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    padding: 8px 16px
    height: 38px
  button-outline-hover:
    backgroundColor: "{colors.outline}"
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 8px 12px
  link:
    textColor: "{colors.on-surface-variant}"
---

# incident.io Design System

## Overview

incident.io describes itself as: “incident.io is a software reliability platform unifying on-call, agentic root cause analysis, incident response, and status pages – helping teams resolve issues faster.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#161618)** text, and **Vivid Red (#F25533)** as the main accent.

Type is set in **STKBureauSerif** and **STKBureauSans**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [incident.io](https://incident.io/) on November 4, 2026 at 1440×900 and 390×844 from 371 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 18 roles.

- **White (#FFFFFF):** Page background, seen 13 times. Token `background`, CSS `--color-white`.
- **Charcoal (#161618):** Primary text and headings, seen 41 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 9 times. Token `on-surface-strong`.
- **Deep Blue (#111827):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Slate (#6D6D70):** Muted text and metadata, seen 9 times. Token `on-surface-muted`.
- **Warm Snow (#F8F5F0):** Raised areas one step from the page, seen 13 times. Token `surface-container-low`, CSS `--color-surface-secondary`.
- **Mist (#F3F3F4):** Cards and panels, seen 2 times. Token `surface-container`.
- **Mist (#E8E8EA):** Hover and pressed fills, seen 3 times. Token `surface-container-high`.
- **Silver (#D6D6D8):** Highest raised elements, seen 5 times. Token `surface-container-highest`.
- **Vivid Red 70% (#F25533B3):** Translucent fill for cards and controls, seen 12 times. Token `overlay`.
- **Near Black 5% (#0000000D):** Stronger translucent fill, seen 5 times. Token `overlay-strong`.
- **Warm Mist (#F1EBE2):** Borders and dividers, seen 5 times. Token `outline`, CSS `--color-surface-tertiary`.
- **Mist (#E8E8EA):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Vivid Red (#F25533):** Primary buttons and calls to action, seen 20 times. Token `primary`, CSS `--color-orange-600`.
- **Snow (#F7F7F8):** Text and icons on primary. Token `on-primary`.
- **Blue (#3A5BD9):** Accent in text, fills and borders, seen 3 times. Token `secondary`.
- **Red (#FF5F57):** Accent in text, fills and borders, seen 2 times. Token `tertiary`.
- **Dark Red (#9B1C1C):** Errors and destructive states, seen 5 times. Token `error`.

## Typography

**STKBureauSerif**, **STKBureauSans** and **Inter** share the interface. Fallback stack: `STKBureauSerif, STKBureauSerif Fallback`. Other loaded fonts: Geist Mono, Lato.

- **headline-display:** STKBureauSerif 80px at weight 400, line height 1, tracking -0.04em (36px on mobile). Page title (h1).
- **headline-lg:** STKBureauSerif 44px at weight 400, line height 1.1, tracking -0.03em. Section headings (h2).
- **headline-md:** STKBureauSerif 36px at weight 400, line height 1.15, tracking -0.025em. Sub-section headings.
- **headline-sm:** STKBureauSans 24px at weight 500, line height 1.3, tracking -0.01em. Card and feature titles.
- **body-md:** STKBureauSans 18px at weight 500, line height 1.4, tracking -0.01em. Body text.
- **body-sm:** STKBureauSans 13px at weight 400, line height 1.4, tracking -0.01em. Secondary and small text.
- **caption:** Inter 10px at weight 400, line height 1.5. Captions and fine print.
- **label-lg:** STKBureauSans 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** STKBureauSans 13px at weight 500, line height 1.4, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** Inter 10px at weight 600, line height 1.48. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (88% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 3px, sm 8px, md 12px, lg 20px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1192px.
- **Breakpoints:** 350px, 768px, 1024px, 2400px, 2561px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.08) 0px 2px 10px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(22, 22, 24, 0.16) 0px 20px 50px -12px, rgba(22, 22, 24, 0.04) 0px 4px 6px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 56 elements.
- **lg (12px):** 20 elements.
- **sm (6px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get a demo”):** #F25533 fill, #F7F7F8 text, 18px/500, 3.35544e+07px radius, padding 12px 20px.
- **button-primary-hover:** background #DD340D, text #F7F7F8 on hover.
- **button-outline (“Login”):** #F8F5F0 fill, #161618 text, 16px/500, 3.35544e+07px radius, padding 8px 16px.
- **button-outline-hover:** background #F1EBE2, text #161618 on hover.
- **button-ghost (“Products”):** transparent fill, #111827 text, 16px/500, padding 8px 12px.
- **link:** transparent fill, #111827 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8F5F0, #F3F3F4, #E8E8EA, #D6D6D8.
- Do keep text in 4 levels: #161618, #000000, #111827, #6D6D70.
- Do reserve #F25533 for primary actions and key highlights.
- Do set headlines in STKBureauSerif with tight tracking (-0.04em).
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 8px corners on most elements; larger surfaces also use 12px and 6px.
- Don't introduce new font families beyond STKBureauSerif, STKBureauSans and Inter.
- Don't use #F25533 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`, `cubic-bezier(0.2, 0, 0, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/incident.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
