---
version: alpha
name: Perplexity AI
description: "Dark interface measured from perplexity.ai: pplxSans type, dark cyan accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#15191D"
  surface: "#15191D"
  on-surface: "#DADFE3"
  on-background: "#DADFE3"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#959A9E"
  surface-container-low: "#081F22"
  surface-container: "#1A1E21"
  surface-container-high: "#100E12"
  overlay: "#4E99A317"
  overlay-strong: "#DADFE30F"
  outline: "#DADFE324"
  primary: "#016A71"
  on-primary: "#FFFFFF"
  secondary: "#7989E7"
typography:
  body-md:
    fontFamily: pplxSans
    fontSize: 16px
    fontWeight: 360
    lineHeight: 1.5
  body-sm:
    fontFamily: pplxSans
    fontSize: 12px
    fontWeight: 470
    lineHeight: 2
  label-md:
    fontFamily: pplxSans
    fontSize: 14px
    fontWeight: 470
    lineHeight: 2
rounded:
  sm: 6px
  md: 8px
  lg: 11px
  xl: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  gutter: 16px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 12px
    height: 32px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 0px 8px
  card:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 16px
---

# Perplexity AI Design System

## Overview

Perplexity AI describes itself as: “Perplexity is a free AI-powered answer engine that provides accurate, trusted, and real-time answers to any question.” The interface is dark, built on **Cool Charcoal (#15191D)** with **Cool Silver (#DADFE3)** text, and **Dark Cyan (#016A71)** as the main accent.

Type is set in **pplxSans**. Headlines run large; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [perplexity.ai](https://www.perplexity.ai/) on October 21, 2026 at 1440×900 and 390×844 from 104 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Cool Charcoal (#15191D):** Page background, seen 1 time. Token `background`.
- **Cool Silver (#DADFE3):** Primary text and headings, seen 11 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 2 times. Token `on-surface-strong`.
- **Cool Gray (#959A9E):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Deep Cyan (#081F22):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Cool Charcoal (#1A1E21):** Cards and panels, seen 2 times. Token `surface-container`.
- **Charcoal (#100E12):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Cyan 9% (#4E99A317):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Cool Silver 6% (#DADFE30F):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Cool Silver 14% (#DADFE324):** Borders and dividers, seen 1 time. Token `outline`.
- **Dark Cyan (#016A71):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Indigo (#7989E7):** Brand accent (CSS variable), seen 12 times. Token `secondary`.

## Typography

**pplxSans** carries the whole interface. Fallback stack: `pplxSans, ui-sans-serif, system-ui, -apple-system`.

- **body-md:** pplxSans 16px at weight 360, line height 1.5. Body text.
- **body-sm:** pplxSans 12px at weight 470, line height 2. Secondary and small text.
- **label-md:** pplxSans 14px at weight 470, line height 2. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (79% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#081F22 → #1A1E21 → #100E12) and #DADFE324 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 56 elements.
- **md (8px):** 44 elements.
- **sm (6px):** 8 elements.
- **lg (11px):** 8 elements.
- **xl (16px):** 6 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Got it”):** #DADFE3 fill, #15191D text, 14px/470, 8px radius, padding 0px 12px.
- **button-ghost (“View plans”):** transparent fill, #DADFE3 text, 12px/470, 9999px radius, padding 0px 8px.
- **card:** #016A71 fill, #FFFFFF text, 16px/360, 11px radius, padding 16px.

## Do's and Don'ts

- Do use #15191D for the page and lift surfaces in small steps: #081F22, #1A1E21, #100E12.
- Do keep text in 3 levels: #DADFE3, #FFFFFF, #959A9E.
- Do reserve #016A71 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px).
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond pplxSans.
- Don't use #016A71 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.075s.

- **Easing:** `cubic-bezier(0, 0, 0.2, 1)`, `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/perplexity.ai/), the free DESIGN.md generator.
