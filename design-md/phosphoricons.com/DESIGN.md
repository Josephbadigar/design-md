---
version: alpha
name: Phosphor Icons
description: "Light interface measured from phosphoricons.com: Manrope type with Arial, lime accents, tonal surfaces and 16px corners."
colors:
  background: "#EEEAE3"
  surface: "#EEEAE3"
  on-surface: "#656461"
  on-background: "#656461"
  on-surface-strong: "#3C402B"
  surface-container-low: "#FFFFFF"
  surface-container: "#BCADAF"
  overlay: "#FFFFFF0D"
  overlay-strong: "#FFFFFF4D"
  primary: "#C4E456"
  on-primary: "#000000"
  secondary: "#A4B55B"
  warning: "#D6971E"
typography:
  headline-display:
    fontFamily: Manrope
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.3
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: 400
  body-sm:
    fontFamily: Arial
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  headline-display-mobile:
    fontFamily: Manrope
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.43
rounded:
  sm: 8px
  md: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 12px
  lg: 32px
  xl: 56px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px 32px 0px 28px
    height: 56px
  button-ghost:
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: 1px 6px
  input-field:
    textColor: "{colors.surface-container-low}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-strong}"
---

# Phosphor Icons Design System

## Overview

Phosphor Icons describes itself as: “A flexible icon family for interfaces, diagrams, presentations — whatever, really.” The interface is light, built on **Warm Mist (#EEEAE3)** with **Slate (#656461)** text, and **Lime (#C4E456)** as the main accent.

Type is set in **Manrope** and **Arial**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 16px.

Measured from [phosphoricons.com](https://phosphoricons.com/) on November 4, 2026 at 1440×900 and 390×844 from 331 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Warm Mist (#EEEAE3):** Page background, seen 2 times. Token `background`, CSS `--vellum`.
- **Slate (#656461):** Primary text and headings, seen 43 times. Token `on-surface`, CSS `--foreground-secondary`.
- **Deep Lime (#3C402B):** Headings and emphasis, seen 20 times. Token `on-surface-strong`, CSS `--foreground-card`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Warm Gray (#BCADAF):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--sand`.
- **White 5% (#FFFFFF0D):** Translucent fill for cards and controls, seen 3 times. Token `overlay`, CSS `--scrim`.
- **White 30% (#FFFFFF4D):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Lime (#C4E456):** Brand color in the header, seen 1 time. Token `primary`, CSS `--acid`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Lime (#A4B55B):** Accent on large areas. Token `secondary`.
- **Orange (#D6971E):** Warnings and highlights, seen 6 times. Token `warning`, CSS `--mustard`.

## Typography

**Manrope** and **Arial** share the interface. Fallback stack: `Manrope, -apple-system, BlinkMacSystemFont, Segoe UI`. Other loaded fonts: IBM Plex Mono.

- **headline-display:** Manrope 40px at weight 400, line height 1.3 (28px on mobile). Page title (h1).
- **body-md:** Manrope 16px at weight 400. Body text.
- **body-sm:** Arial 12px at weight 400, line height 1.33. Secondary and small text.

## Layout

Spacing is mostly on a 4px grid (73% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 12px, lg 32px, xl 56px.
- **Breakpoints:** 536px, 558px, 719px, 720px, 858px, 1100px, 1239px, 1240px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(60, 64, 43, 0.2) 2px 2px 0px 0px`
- `rgba(60, 64, 43, 0.2) 0px 2px 0px 0px`

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **md (16px):** 392 elements.
- **sm (8px):** 24 elements.
- **full (9999px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Get started”):** #FFFFFF fill, #3C402B text, 16px/600, 8px radius, padding 0px 32px 0px 28px, border 1px solid #3C402B, shadow `rgba(60, 64, 43, 0.2) 2px 2px 0px 0px`.
- **button-ghost (“acorn”):** transparent fill, #000000 text, 13.3333px/400, 16px radius, padding 1px 6px.
- **input-field (“Search”):** transparent fill, #FFFFFF text, 16px/400, padding 0px.
- **link:** transparent fill, #3C402B text, padding 0px.

## Do's and Don'ts

- Do use #EEEAE3 for the page and lift surfaces in small steps: #FFFFFF, #BCADAF.
- Do keep text in 2 levels: #656461, #3C402B.
- Do use #C4E456 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (6px, 12px, 32px).
- Do use 16px corners on most elements; larger surfaces also use 8px.
- Don't introduce new font families beyond Manrope and Arial.
- Don't use #C4E456 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/phosphoricons.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
