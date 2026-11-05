---
version: alpha
name: Visual Studio Code
description: "Light interface measured from code.visualstudio.com: system-ui type, blue accents, tonal surfaces and 8px corners."
colors:
  background: "#F0F0F0"
  surface: "#F0F0F0"
  on-surface: "#1B1B1D"
  on-background: "#1B1B1D"
  on-surface-variant: "#242424"
  on-surface-muted: "#545458"
  on-surface-subtle: "#68686D"
  surface-container-low: "#FFFFFF"
  overlay: "#E0E0E3CC"
  overlay-strong: "#F0F0F0E0"
  primary: "#0069CC"
  on-primary: "#FFFFFF"
  inverse-surface: "#191A1B"
  secondary: "#2F6FB8"
  tertiary: "#7CC4AE"
  warning: "#FFD700"
  error: "#FF7B72"
typography:
  headline-display:
    fontFamily: system-ui
    fontSize: 36px
    fontWeight: 560
    lineHeight: 1.06
    letterSpacing: -0.022em
  headline-lg:
    fontFamily: system-ui
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.52
    letterSpacing: -0.021em
  body-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: system-ui
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.33
  body-sm:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.4
  caption:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: system-ui
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.43
  label-md:
    fontFamily: system-ui
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.4
  label-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: -0.005em
rounded:
  sm: 2px
  md: 6px
  lg: 8px
spacing:
  xs: 3px
  sm: 8px
  md: 12px
  lg: 18px
  xl: 40px
  gutter: 8px
  section: 135px
components:
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface-subtle}"
---

# Visual Studio Code Design System

## Overview

Visual Studio Code describes itself as: “Code with precision, collaborate with agents, orchestrate a team of them, and continue your work wherever you are with Visual Studio Code.” The interface is light, built on **Mist (#F0F0F0)** with **Charcoal (#1B1B1D)** text, and **Blue (#0069CC)** as the main accent.

Type is set in **system-ui**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 8px.

Measured from [code.visualstudio.com](https://code.visualstudio.com/?_exp_home=e855cfac50) on November 4, 2026 at 1440×900 from 276 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **Mist (#F0F0F0):** Page background, seen 2 times. Token `background`, CSS `--bg`.
- **Charcoal (#1B1B1D):** Primary text and headings, seen 19 times. Token `on-surface`, CSS `--ink`.
- **Graphite (#242424):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Slate (#545458):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Slate (#68686D):** Subtle text and placeholders, seen 16 times. Token `on-surface-subtle`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--button-primary-foreground`.
- **Mist 80% (#E0E0E3CC):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Mist 88% (#F0F0F0E0):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Blue (#0069CC):** Most used accent color, seen 25 times. Token `primary`, CSS `--link`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#191A1B):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Blue (#2F6FB8):** Accent (CSS variable). Token `secondary`.
- **Teal (#7CC4AE):** Accent in text, fills and borders, seen 6 times. Token `tertiary`.
- **Vivid Amber (#FFD700):** Warnings and highlights, seen 7 times. Token `warning`.
- **Light Red (#FF7B72):** Errors and destructive states, seen 3 times. Token `error`.

## Typography

**system-ui** carries the whole interface. Fallback stack: `-apple-system, BlinkMacSystemFont, SF Pro Display, Segoe WPC`. Other loaded fonts: codicon, codicon-vscode, dl-seti.

- **headline-display:** system-ui 36px at weight 560, line height 1.06, tracking -0.022em. Page title (h1).
- **headline-lg:** system-ui 28px at weight 700, line height 1.52, tracking -0.021em. Section headings (h2).
- **body-md:** system-ui 14px at weight 400, line height 1.43. Body text.
- **body-lg:** system-ui 15px at weight 400, line height 1.33. Lead paragraphs.
- **body-sm:** system-ui 13px at weight 400, line height 1.4. Secondary and small text.
- **caption:** system-ui 12px at weight 400, line height 1.5. Captions and fine print.
- **label-lg:** system-ui 20px at weight 600, line height 1.43. Large buttons and tabs.
- **label-md:** system-ui 15px at weight 500, line height 1.4. Buttons, navigation and labels.
- **label-sm:** system-ui 14px at weight 500, line height 1.43, tracking -0.005em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 40% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 8px, md 12px, lg 18px, xl 40px.
- **Sections:** 135px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 680px, 767px, 768px, 991px, 992px, 999.98px, 1000px, 1099.98px, 1100px, 1199px, 1200px, 1399px, 1400px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF).

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **lg (8px):** 156 elements.
- **sm (2px):** 136 elements.
- **md (6px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Features”):** transparent fill, #242424 text, 14px/500, 8px radius, padding 0px.
- **link:** transparent fill, #68686D text, padding 0px.

## Do's and Don'ts

- Do use #F0F0F0 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 4 levels: #1B1B1D, #242424, #545458, #68686D.
- Do reserve #0069CC for primary actions and key highlights.
- Do set headlines in system-ui with tight tracking (-0.022em).
- Do reuse the measured spacing steps (8px, 12px, 18px).
- Do use 8px corners on most elements; larger surfaces also use 2px and 6px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond system-ui.
- Don't use #0069CC for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.25s. Longer ambient animations run 0.7s.

- **Easing:** `ease`, `cubic-bezier(0.2, 0.7, 0.1, 1)`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/code.visualstudio.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
