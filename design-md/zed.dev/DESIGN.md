---
version: alpha
name: Zed
description: "Light interface measured from zed.dev: plexSerif type with writer, vivid blue accents, tonal surfaces and 4px corners."
colors:
  background: "#EEE7E7"
  surface: "#EEE7E7"
  on-surface: "#242529"
  on-background: "#242529"
  on-surface-strong: "#0A0A0A"
  on-surface-variant: "#525252"
  on-surface-muted: "#58585A"
  surface-container-low: "#EBEBEC"
  surface-container: "#E5E5E5"
  surface-container-high: "#DFDFE0"
  surface-container-highest: "#FAFAFA"
  overlay: "#CFCDC533"
  overlay-strong: "#FFFFFFCC"
  outline: "#D4D4D4"
  outline-variant: "#A1A1A180"
  primary: "#1348DC"
  on-primary: "#FFFFFF"
  secondary: "#BF3C27"
  tertiary: "#5C78E2"
typography:
  headline-display:
    fontFamily: plexSerif
    fontSize: 25.5px
    fontWeight: 390
    lineHeight: 1.25
  body-md:
    fontFamily: writer
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: plexSerif
    fontSize: 18.5px
    fontWeight: 410
    lineHeight: 1.2
  body-sm:
    fontFamily: writer
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  caption:
    fontFamily: writer
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.025em
  label-md:
    fontFamily: writer
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.5
  code:
    fontFamily: ui-monospace
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
rounded:
  sm: 2px
  md: 4px
  lg: 16px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 20px
  xl: 40px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: 6px 4px
    height: 34px
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "#262626"
    rounded: "{rounded.md}"
    padding: 6px 4px
    height: 34px
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: 6px 4px
    height: 34px
  button-ghost:
    rounded: "{rounded.md}"
    padding: 6px 4px
  link:
    textColor: "{colors.on-surface-strong}"
---

# Zed Design System

## Overview

Zed describes itself as: “Zed is a high-performance, multiplayer code editor from the creators of Atom and Tree-sitter.” The interface is light, built on **Warm Mist (#EEE7E7)** with **Graphite (#242529)** text, and **Vivid Blue (#1348DC)** as the main accent.

Type is set in **plexSerif** and **writer**, with **ui-monospace** for code. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [zed.dev](https://zed.dev/) on November 4, 2026 at 1440×900 and 390×844 from 289 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles.

- **Warm Mist (#EEE7E7):** Page background. Token `background`.
- **Graphite (#242529):** Primary text and headings, seen 20 times. Token `on-surface`.
- **Near Black (#0A0A0A):** Headings and emphasis, seen 10 times. Token `on-surface-strong`.
- **Slate (#525252):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Slate (#58585A):** Muted text and metadata, seen 11 times. Token `on-surface-muted`.
- **Mist (#EBEBEC):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Mist (#E5E5E5):** Cards and panels, seen 2 times. Token `surface-container`.
- **Silver (#DFDFE0):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Snow (#FAFAFA):** Highest raised elements, seen 3 times. Token `surface-container-highest`.
- **Warm Silver 20% (#CFCDC533):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White 80% (#FFFFFFCC):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Silver (#D4D4D4):** Borders and dividers, seen 8 times. Token `outline`.
- **Gray 50% (#A1A1A180):** Secondary dividers, seen 4 times. Token `outline-variant`.
- **Vivid Blue (#1348DC):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Red (#BF3C27):** Secondary buttons, seen 1 time. Token `secondary`.
- **Blue (#5C78E2):** Accent in text, fills and borders, seen 7 times. Token `tertiary`.

## Typography

**plexSerif**, **writer** and **ui-monospace** (monospace) share the interface. Fallback stack: `plexSerif, plexSerif Fallback`.

- **headline-display:** plexSerif 25.5px at weight 390, line height 1.25. Page title (h1).
- **body-md:** writer 16px at weight 400, line height 1.5. Body text.
- **body-lg:** plexSerif 18.5px at weight 410, line height 1.2. Lead paragraphs.
- **body-sm:** writer 12px at weight 400, line height 1.33. Secondary and small text.
- **caption:** writer 10px at weight 400, line height 1.5, tracking -0.025em. Captions and fine print.
- **label-md:** writer 11px at weight 400, line height 1.5. Buttons, navigation and labels.
- **code:** ui-monospace 16px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing does not follow a strict grid: 65% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 16px, lg 20px, xl 40px.
- **Breakpoints:** 639px, 640px, 768px, 820px, 1024px, 1280px, 1536px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgb(209, 209, 209) 0px -2px 0px 0px inset, rgb(242, 242, 242) 0px 1px 3px 0px`
- `rgb(127, 39, 26) 0px -2px 0px 0px inset, rgb(251, 236, 234) 0px 1px 3px 0px`
- `rgb(5, 55, 148) 0px -2px 0px 0px inset, rgb(230, 239, 254) 0px 1px 3px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 96 elements.
- **sm (2px):** 32 elements.
- **lg (16px):** 6 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Download”):** #1348DC fill, #FFFFFF text, 13px/400, 4px radius, padding 6px 4px, border 1px solid #2B7FFF66, shadow `rgb(5, 55, 148) 0px -2px 0px 0px inset, rgb(230, 239, 254) 0px 1px 3px 0px`.
- **button-outline (“Learn More”):** #E5E5E5 fill, #262626 text, 13px/400, 4px radius, padding 6px 4px, border 1px solid #A1A1A180, shadow `rgb(209, 209, 209) 0px -2px 0px 0px inset, rgb(242, 242, 242) 0px 1px 3px 0px`.
- **button-secondary (“Download”):** #BF3C27 fill, #FFFFFF text, 13px/400, 4px radius, padding 6px 4px, border 1px solid #BE3B2799, shadow `rgb(127, 39, 26) 0px -2px 0px 0px inset, rgb(251, 236, 234) 0px 1px 3px 0px`.
- **button-ghost (“Learn More”):** transparent fill, 13px/400, 4px radius, padding 6px 4px, shadow `rgb(209, 209, 209) 0px -2px 0px 0px inset, rgb(242, 242, 242) 0px 1px 3px 0px`.
- **link:** transparent fill, #0A0A0A text, padding 0px.

## Do's and Don'ts

- Do use #EEE7E7 for the page and lift surfaces in small steps: #EBEBEC, #E5E5E5, #DFDFE0, #FAFAFA.
- Do keep text in 4 levels: #242529, #0A0A0A, #525252, #58585A.
- Do reserve #1348DC for primary actions and key highlights.
- Do reuse the measured spacing steps (6px, 16px, 20px).
- Do use 4px corners on most elements; larger surfaces also use 2px and 16px.
- Don't introduce new font families beyond plexSerif, writer and ui-monospace.
- Don't use #1348DC for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s. Longer ambient animations run 1.75s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/zed.dev/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
