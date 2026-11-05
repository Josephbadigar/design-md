---
version: alpha
name: Replit
description: "Light interface measured from replit.com: Replit Diatype type, vivid red accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FAF6F1"
  surface: "#FAF6F1"
  on-surface: "#4B5563"
  on-background: "#4B5563"
  on-surface-strong: "#312E2E"
  on-surface-variant: "#37383C"
  on-surface-muted: "#4B4D53"
  surface-container-low: "#F7F7F6"
  surface-container: "#F3F3F1"
  surface-container-high: "#FCFCFB"
  surface-container-highest: "#EFEEEC"
  overlay: "#FFFFFF59"
  outline: "#C5C5C599"
  outline-variant: "#D8D5CF"
  primary: "#FF3C00"
  on-primary: "#FFFFFF"
  inverse-surface: "#181818"
  secondary: "#F9AA8B"
  tertiary: "#DEA483"
  error: "#FFB199"
typography:
  headline-display:
    fontFamily: Replit Diatype
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.06em
  headline-lg:
    fontFamily: Replit Diatype
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Replit Diatype
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.04em
  body-md:
    fontFamily: Replit Diatype
    fontSize: 14px
    fontWeight: 450
  body-lg:
    fontFamily: Replit Diatype
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.03em
  label-md:
    fontFamily: Replit Diatype
    fontSize: 14px
    fontWeight: 400
  code:
    fontFamily: Replit Diatype Mono
    fontSize: 13px
    fontWeight: 500
    letterSpacing: 0.12em
  headline-display-mobile:
    fontFamily: Replit Diatype
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.06em
  headline-lg-mobile:
    fontFamily: Replit Diatype
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.03em
rounded:
  sm: 6px
  md: 8px
  lg: 16px
  xl: 100px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 17px
  xl: 64px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 38px
  button-outline:
    backgroundColor: "#F1F0EE"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px
    height: 48px
  button-ghost:
    backgroundColor: "{colors.surface-container-highest}"
    textColor: "#212225"
    typography: "{typography.code}"
    rounded: "{rounded.sm}"
    padding: 0px 8px
    height: 32px
  input-field:
    textColor: "#18191B"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 6px 6px 0px 6px
  link:
    textColor: "{colors.on-surface}"
---

# Replit Design System

## Overview

Replit describes itself as: “Describe what you want. Replit builds it. Get a working app or website in minutes. No coding required.” The interface is light, built on **Warm Snow (#FAF6F1)** with **Dark Blue (#4B5563)** text, and **Vivid Red (#FF3C00)** as the main accent.

Type is set in **Replit Diatype**, with **Replit Diatype Mono** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [replit.com](https://replit.com/) on November 4, 2026 at 1440×900 and 390×844 from 352 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 18 roles.

- **Warm Snow (#FAF6F1):** Page background, seen 2 times. Token `background`.
- **Dark Blue (#4B5563):** Primary text and headings, seen 30 times. Token `on-surface`.
- **Graphite (#312E2E):** Headings and emphasis, seen 22 times. Token `on-surface-strong`.
- **Graphite (#37383C):** Secondary text, seen 23 times. Token `on-surface-variant`.
- **Cool Slate (#4B4D53):** Muted text and metadata, seen 14 times. Token `on-surface-muted`.
- **Snow (#F7F7F6):** Raised areas one step from the page, seen 13 times. Token `surface-container-low`.
- **Mist (#F3F3F1):** Cards and panels, seen 1 time. Token `surface-container`.
- **Snow (#FCFCFB):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Mist (#EFEEEC):** Highest raised elements, seen 4 times. Token `surface-container-highest`.
- **White 35% (#FFFFFF59):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Silver 60% (#C5C5C599):** Borders and dividers, seen 8 times. Token `outline`.
- **Warm Silver (#D8D5CF):** Secondary dividers, seen 6 times. Token `outline-variant`.
- **Vivid Red (#FF3C00):** Primary buttons and calls to action, seen 15 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#181818):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Light Orange (#F9AA8B):** Accent on large areas. Token `secondary`.
- **Orange (#DEA483):** Accent (CSS variable). Token `tertiary`.
- **Light Red (#FFB199):** Errors and destructive states, seen 6 times. Token `error`.

## Typography

**Replit Diatype** and **Replit Diatype Mono** (monospace) share the interface. Fallback stack: `Replit Diatype, sans-serif`.

- **headline-display:** Replit Diatype 64px at weight 400, line height 1, tracking -0.06em (32px on mobile). Page title (h1).
- **headline-lg:** Replit Diatype 36px at weight 400, line height 1, tracking -0.03em (22px on mobile). Section headings (h2).
- **headline-md:** Replit Diatype 32px at weight 400, line height 1, tracking -0.04em. Sub-section headings.
- **body-md:** Replit Diatype 14px at weight 450. Body text.
- **body-lg:** Replit Diatype 26px at weight 400, line height 1.2, tracking -0.03em. Lead paragraphs.
- **label-md:** Replit Diatype 14px at weight 400. Buttons, navigation and labels.
- **code:** Replit Diatype Mono 13px at weight 500, tracking 0.12em, uppercase. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (85% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 8px, md 12px, lg 17px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 480px, 512px, 640px, 768px, 769px, 800px, 900px, 1024px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F7F7F6 → #F3F3F1 → #FCFCFB → #EFEEEC) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(219, 217, 211) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.02) 0px 1px 2px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(216, 224, 228) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(210, 208, 201) 0px 0px 0px 0px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.02) 0px 2px 2px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (6px):** 48 elements.
- **md (8px):** 40 elements.
- **full (9999px):** 40 elements.
- **lg (16px):** 32 elements.
- **xl (100px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #FF3C00 fill, #FFFFFF text, 14px/500, 8px radius, padding 8px 12px.
- **button-outline (“Website”):** #F1F0EE fill, #37383C text, 14px/400, 16px radius, padding 0px.
- **button-ghost (“Weekly meal planner”):** #EFEEEC fill, #212225 text, 13.3333px/400, 6px radius, padding 0px 8px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(219, 217, 211) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.02) 0px 1px 2px 0px`.
- **input-field (“Create a mobile app that…”):** transparent fill, #18191B text, 14px/400, 6px radius, padding 6px 6px 0px 6px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(210, 208, 201) 0px 0px 0px 0px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.02) 0px 2px 2px 0px`.
- **link:** transparent fill, #4B5563 text, padding 0px.

## Do's and Don'ts

- Do use #FAF6F1 for the page and lift surfaces in small steps: #F7F7F6, #F3F3F1, #FCFCFB, #EFEEEC.
- Do keep text in 4 levels: #4B5563, #312E2E, #37383C, #4B4D53.
- Do reserve #FF3C00 for primary actions and key highlights.
- Do set headlines in Replit Diatype with tight tracking (-0.06em).
- Do reuse the measured spacing steps (8px, 12px, 17px).
- Do make buttons and chips fully rounded (9999px); most other elements use 6px corners.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Replit Diatype and Replit Diatype Mono.
- Don't use #FF3C00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.12s, 0.15s, 0.2s, 0.25s. Longer ambient animations run 2.4s.

- **Easing:** `ease`, `ease-out`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/replit.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
