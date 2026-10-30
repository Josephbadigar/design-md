---
version: alpha
name: Obsidian
description: "Dark interface measured from obsidian.md: system-ui type, light violet accents, tonal surfaces and 6px corners."
colors:
  background: "#0F0F0F"
  surface: "#0F0F0F"
  on-surface: "#EEEEEE"
  on-background: "#EEEEEE"
  on-surface-variant: "#BCBCBC"
  on-surface-muted: "#B3B3B3"
  on-surface-subtle: "#A3A3A3"
  surface-container-low: "#1F1F1F"
  surface-container: "#404040"
  overlay: "#8A5CF526"
  overlay-strong: "#00000080"
  primary: "#A88BFA"
  on-primary: "#000000"
  secondary: "#7C3AED"
  tertiary: "#8A5CF5"
typography:
  headline-display:
    fontFamily: system-ui
    fontSize: 60px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.02em
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.25
  body-lg:
    fontFamily: system-ui
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: system-ui
    fontSize: 6px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.25
  label-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: system-ui
    fontSize: 44px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.02em
rounded:
  xs: 2px
  sm: 4px
  md: 6px
  lg: 8px
  xl: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 24px
  section: 96px
components:
  button-primary:
    backgroundColor: "{colors.secondary}"
    textColor: "#FFFFFF"
    typography: "{typography.body-lg}"
    rounded: "{rounded.lg}"
    padding: 16px 24px
    height: 60px
  button-ghost:
    textColor: "#A78BFA"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Obsidian Design System

## Overview

Obsidian describes itself as: “The free and flexible app for your private thoughts.” The interface is dark, built on **Charcoal (#0F0F0F)** with **Mist (#EEEEEE)** text, and **Light Violet (#A88BFA)** as the main accent.

Type is set in **system-ui**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 6px.

Measured from [obsidian.md](https://obsidian.md/) on October 29, 2026 at 1440×900 and 390×844 from 347 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Charcoal (#0F0F0F):** Page background, seen 1 time. Token `background`.
- **Mist (#EEEEEE):** Primary text and headings, seen 58 times. Token `on-surface`.
- **Silver (#BCBCBC):** Secondary text, seen 33 times. Token `on-surface-variant`.
- **Gray (#B3B3B3):** Muted text and metadata, seen 25 times. Token `on-surface-muted`.
- **Gray (#A3A3A3):** Subtle text and placeholders, seen 7 times. Token `on-surface-subtle`, CSS `--color-gray-400`.
- **Charcoal (#1F1F1F):** Raised areas one step from the page, seen 8 times. Token `surface-container-low`.
- **Graphite (#404040):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--star-color`.
- **Violet 15% (#8A5CF526):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Near Black 50% (#00000080):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Light Violet (#A88BFA):** Most used accent color, seen 21 times. Token `primary`, CSS `--color-accent-400`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Violet (#7C3AED):** Secondary buttons, seen 2 times. Token `secondary`, CSS `--color-violet-600`.
- **Violet (#8A5CF5):** Accent (CSS variable), seen 2 times. Token `tertiary`.

## Typography

**system-ui** carries the whole interface. Fallback stack: `ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont`.

- **headline-display:** system-ui 60px at weight 600, line height 1, tracking -0.02em (44px on mobile). Page title (h1).
- **body-md:** system-ui 16px at weight 400, line height 1.25. Body text.
- **body-lg:** system-ui 20px at weight 400, line height 1.4. Lead paragraphs.
- **body-sm:** system-ui 6px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** system-ui 16px at weight 500, line height 1.25. Buttons, navigation and labels.
- **label-sm:** system-ui 14px at weight 400, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (76% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Breakpoints:** 640px, 768px, 1024px, 1280px, 1536px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#1F1F1F → #404040):

- `rgb(255, 255, 255) 0px 0px 0px 0px inset, rgba(255, 255, 255, 0.05) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`
- `rgb(255, 255, 255) 0px 0px 0px 0px inset, rgba(255, 255, 255, 0.1) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

A few raised panels add a soft drop shadow: `rgb(255, 255, 255) 0px 0px 0px 0px inset, rgba(255, 255, 255, 0.1) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 60 elements.
- **sm (4px):** 44 elements.
- **lg (8px):** 40 elements.
- **xs (2px):** 36 elements.
- **xl (12px):** 28 elements.
- **full (9999px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Obsidian for Linux (AppImage”):** #7C3AED fill, #FFFFFF text, 20px/500, 8px radius, padding 16px 24px, shadow `rgb(255, 255, 255) 0px 0px 0px 0px inset, rgba(255, 255, 255, 0.1) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`.
- **button-ghost (“Download now”):** transparent fill, #A78BFA text, 24px/500, padding 0px.
- **card:** #1F1F1F fill, #EEEEEE text, 16px/400, 20% radius, padding 0px, shadow `rgba(255, 255, 255, 0.024) 0px 1px 0px 1px inset, rgba(0, 0, 0, 0.05) 0px 5px 10px 5px`.
- **link:** transparent fill, #EEEEEE text, padding 0px.

## Do's and Don'ts

- Do use #0F0F0F for the page and lift surfaces in small steps: #1F1F1F, #404040.
- Do keep text in 4 levels: #EEEEEE, #BCBCBC, #B3B3B3, #A3A3A3.
- Do reserve #A88BFA for primary actions and key highlights.
- Do set headlines in system-ui with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 6px corners on most elements; larger surfaces also use 4px, 8px and 2px.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond system-ui.
- Don't use #A88BFA for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.15s, 0.25s. Longer ambient animations run 1s, 2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/obsidian.md/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
