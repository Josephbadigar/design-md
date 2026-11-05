---
version: alpha
name: Procreate
description: "Dark interface measured from procreate.com: system-ui type, vivid blue accents, tonal surfaces and 100px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#A8A8A8"
  on-surface-muted: "#A3A3A3"
  on-surface-subtle: "#808080"
  surface-container-low: "#0B0B0B"
  surface-container: "#141414"
  surface-container-high: "#262626"
  primary: "#0076FF"
  on-primary: "#FFFFFF"
  secondary: "#F7235B"
typography:
  headline-display:
    fontFamily: system-ui
    fontSize: 60px
    fontWeight: 600
    lineHeight: 1
  headline-lg:
    fontFamily: system-ui
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.005em
  headline-md:
    fontFamily: system-ui
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.005em
  headline-sm:
    fontFamily: system-ui
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: -0.005em
  body-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.15
  body-lg:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  label-lg:
    fontFamily: system-ui
    fontSize: 18px
    fontWeight: 600
    lineHeight: 0.98
    letterSpacing: 0.05em
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.025em
  label-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: 0.02em
rounded:
  sm: 12px
  md: 72px
  lg: 100px
spacing:
  xs: 4px
  sm: 6px
  md: 10px
  lg: 20px
  xl: 40px
  gutter: 25px
  section: 60px
  margin: 40px
  container: 1366px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 10px 20px
    height: 40px
  button-secondary:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 10px 20px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Procreate Design System

## Overview

Procreate describes itself as: “Powerful and easy-to-use drawing and animation apps, made for both creative professionals and aspiring artists. Pay once. No subscription.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Vivid Blue (#0076FF)** as the main accent.

Type is set in **system-ui**. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 100px.

Measured from [procreate.com](https://procreate.com/) on November 4, 2026 at 1440×900 and 390×844 from 182 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Near Black (#000000):** Page background. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 40 times. Token `on-surface`, CSS `--nav-logo-color`.
- **Gray (#A8A8A8):** Secondary text, seen 6 times. Token `on-surface-variant`, CSS `--nav-mobile-section-link-color`.
- **Gray (#A3A3A3):** Muted text and metadata, seen 25 times. Token `on-surface-muted`.
- **Gray (#808080):** Subtle text and placeholders, seen 2 times. Token `on-surface-subtle`.
- **Near Black (#0B0B0B):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Charcoal (#141414):** Cards and panels, seen 1 time. Token `surface-container`.
- **Graphite (#262626):** Hover and pressed fills, seen 9 times. Token `surface-container-high`, CSS `--neutral-800`.
- **Vivid Blue (#0076FF):** Primary buttons and calls to action, seen 5 times. Token `primary`, CSS `--resource-link-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Pink (#F7235B):** Accent, seen 2 times. Token `secondary`.

## Typography

**system-ui** carries the whole interface. Fallback stack: `system-ui, sans-serif`.

- **headline-display:** system-ui 60px at weight 600, line height 1. Page title (h1).
- **headline-lg:** system-ui 40px at weight 600, line height 1.1, tracking -0.005em. Section headings (h2).
- **headline-md:** system-ui 30px at weight 600, line height 1.1, tracking -0.005em. Sub-section headings.
- **headline-sm:** system-ui 24px at weight 600, line height 1.3, tracking -0.005em. Card and feature titles.
- **body-md:** system-ui 14px at weight 400, line height 1.15. Body text.
- **body-lg:** system-ui 16px at weight 400, line height 1.15. Lead paragraphs.
- **label-lg:** system-ui 18px at weight 600, line height 0.98, tracking 0.05em, uppercase. Large buttons and tabs.
- **label-md:** system-ui 16px at weight 600, line height 1, tracking -0.025em. Buttons, navigation and labels.
- **label-sm:** system-ui 14px at weight 600, line height 1.4, tracking 0.02em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 58% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 10px, lg 20px, xl 40px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 25px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1366px.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 360px, 420px, 480px, 600px, 700px, 823px, 1080px, 1240px, 1366px, 1764px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#0B0B0B → #141414 → #262626).

## Shapes

Most elements use 100px corners. Measured radii, most used first:

- **lg (100px):** 40 elements.
- **md (72px):** 12 elements.
- **sm (12px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Buy now”):** #0076FF fill, #FFFFFF text, 14px/600, 100px radius, padding 10px 20px.
- **button-secondary (“Learn more”):** #262626 fill, #FFFFFF text, 14px/600, 100px radius, padding 10px 20px.
- **button-ghost (“Apps”):** transparent fill, #FFFFFF text, 16px/500, padding 0px.
- **link:** transparent fill, #A3A3A3 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #0B0B0B, #141414, #262626.
- Do keep text in 4 levels: #FFFFFF, #A8A8A8, #A3A3A3, #808080.
- Do reserve #0076FF for primary actions and key highlights.
- Do reuse the measured spacing steps (6px, 10px, 20px).
- Do use 100px corners on most elements; larger surfaces also use 72px and 12px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond system-ui.
- Don't use #0076FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.1s, 0.2s, 0.15s, 0.3s. Longer ambient animations run 1s.

- **Easing:** `ease-out`, `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/procreate.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
