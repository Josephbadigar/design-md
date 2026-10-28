---
version: alpha
name: React
description: "Dark interface measured from react.dev: Optimistic Display type with Optimistic Text, cyan accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#23272F"
  surface: "#23272F"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#F6F7F9"
  on-surface-muted: "#EBECF0"
  on-surface-subtle: "#99A1B3"
  surface-container-low: "#23272FF2"
  surface-container: "#343A46"
  overlay: "#78839B33"
  outline: "#FFFFFF0D"
  primary: "#58C4DC"
  on-primary: "#23272F"
  secondary: "#77B7D7"
  tertiary: "#0074A6"
  warning: "#DFAB5C"
  error: "#C64640"
typography:
  headline-display:
    fontFamily: Optimistic Display
    fontSize: 52px
    fontWeight: 600
    lineHeight: 1.15
  headline-lg:
    fontFamily: Optimistic Text
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.25
  headline-md:
    fontFamily: Optimistic Text
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.38
  body-md:
    fontFamily: Optimistic Text
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Optimistic Text
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.38
  label-lg:
    fontFamily: Optimistic Text
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Optimistic Text
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.25
  label-sm:
    fontFamily: Optimistic Text
    fontSize: 13px
    fontWeight: 500
  headline-display-mobile:
    fontFamily: Optimistic Display
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.15
rounded:
  sm: 8px
  md: 16px
  full: 9999px
spacing:
  xs: 2px
  sm: 6px
  md: 16px
  lg: 20px
  xl: 64px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.full}"
    padding: 12px 24px
    height: 47px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.full}"
    padding: 12px 24px
  input-field:
    backgroundColor: "{colors.on-surface-muted}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 16px 0px 16px 44px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "#FFFFFF80"
---

# React Design System

## Overview

React describes itself as: “React is the library for web and native user interfaces. Build user interfaces out of individual pieces called components written in JavaScript. React is designed to let you seamlessly combine components written by indep” The interface is dark, built on **Cool Graphite (#23272F)** with **White (#FFFFFF)** text, and **Cyan (#58C4DC)** as the main accent.

Type is set in **Optimistic Display** and **Optimistic Text**. Headlines run large; body text is 20px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [react.dev](https://react.dev/) on October 21, 2026 at 1440×900 and 390×844 from 372 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles, plus gradient stops #404756, #C76A15, #2B3491, #087EA4.

- **Cool Graphite (#23272F):** Page background, seen 5 times. Token `background`, CSS `--docsearch-hit-background`.
- **White (#FFFFFF):** Primary text and headings, seen 62 times. Token `on-surface`, CSS `--docsearch-footer-background`.
- **Snow (#F6F7F9):** Secondary text, seen 19 times. Token `on-surface-variant`.
- **Mist (#EBECF0):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Blue (#99A1B3):** Subtle text and placeholders, seen 6 times. Token `on-surface-subtle`.
- **Cool Graphite 95% (#23272FF2):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Dark Blue (#343A46):** Cards and panels, seen 4 times. Token `surface-container`.
- **Blue 20% (#78839B33):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White 5% (#FFFFFF0D):** Borders and dividers, seen 4 times. Token `outline`.
- **Cyan (#58C4DC):** Primary buttons and calls to action, seen 20 times. Token `primary`.
- **Cool Graphite (#23272F):** Text and icons on primary. Token `on-primary`.
- **Blue (#77B7D7):** Most used accent color, seen 15 times. Token `secondary`.
- **Dark Cyan (#0074A6):** Brand accent (CSS variable), seen 12 times. Token `tertiary`.
- **Orange (#DFAB5C):** Warnings and highlights, seen 8 times. Token `warning`.
- **Red (#C64640):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**Optimistic Display** and **Optimistic Text** share the interface. Fallback stack: `Optimistic Display, -apple-system, ui-sans-serif, system-ui`. Other loaded fonts: Source Code Pro.

- **headline-display:** Optimistic Display 52px at weight 600, line height 1.15 (40px on mobile). Page title (h1).
- **headline-lg:** Optimistic Text 32px at weight 600, line height 1.25. Section headings (h2).
- **headline-md:** Optimistic Text 28px at weight 600, line height 1.38. Sub-section headings.
- **body-md:** Optimistic Text 20px at weight 400, line height 1.5. Body text.
- **body-sm:** Optimistic Text 13px at weight 400, line height 1.38. Secondary and small text.
- **label-lg:** Optimistic Text 17px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** Optimistic Text 15px at weight 700, line height 1.25. Buttons, navigation and labels.
- **label-sm:** Optimistic Text 13px at weight 500. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 58% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 16px, lg 20px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 374px, 640px, 680px, 768px, 1023px, 1024px, 1280px, 1536px, 1919px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#23272FF2 → #343A46) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.08) 0px 0px 0px 1px inset`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(78, 87, 105) 0px 0px 0px 1px inset`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 172 elements.
- **sm (8px):** 112 elements.
- **md (16px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Learn React”):** #58C4DC fill, #23272F text, 17px/700, 9999px radius, padding 12px 24px.
- **button-ghost (“API Reference”):** transparent fill, #F6F7F9 text, 17px/700, 9999px radius, padding 12px 24px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(78, 87, 105) 0px 0px 0px 1px inset`.
- **input-field (“Search”):** #EBECF0 fill, #23272F text, 15px/400, 9999px radius, padding 16px 0px 16px 44px.
- **card:** #343A46 fill, #F6F7F9 text, 17px/400, 16px radius, padding 0px.
- **link:** transparent fill, #FFFFFF80 text, padding 0px.

## Do's and Don'ts

- Do use #23272F for the page and lift surfaces in small steps: #23272FF2, #343A46.
- Do keep text in 4 levels: #FFFFFF, #F6F7F9, #EBECF0, #99A1B3.
- Do reserve #58C4DC for primary actions and key highlights.
- Do reuse the measured spacing steps (6px, 16px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Optimistic Display and Optimistic Text.
- Don't use #58C4DC for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.1s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.4, 0, 1, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/react.dev/), the free DESIGN.md generator.
