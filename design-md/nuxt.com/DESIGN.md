---
version: alpha
name: Nuxt
description: "Dark interface measured from nuxt.com: Outfit type with Inter, vivid teal accents, tonal surfaces and 6px corners."
colors:
  background: "#0A0A0A"
  surface: "#0A0A0A"
  on-surface: "#E5E5E5"
  on-background: "#E5E5E5"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#BABED8"
  on-surface-muted: "#A1A1A1"
  surface-container-low: "#171717"
  surface-container: "#262626"
  overlay: "#00DC821A"
  overlay-strong: "#0A0A0ABF"
  outline: "#262626"
  primary: "#00DC82"
  on-primary: "#171717"
  secondary: "#89DDFF"
  tertiary: "#F07178"
typography:
  headline-display:
    fontFamily: Outfit
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Outfit
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
  headline-display-mobile:
    fontFamily: Outfit
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
  headline-lg-mobile:
    fontFamily: Outfit
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.025em
rounded:
  md: 6px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 24px
  xl: 64px
  gutter: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 40px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 40px
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 6px 10px
    height: 32px
  input-field:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 8px 44px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Nuxt Design System

## Overview

Nuxt describes itself as: “Build fast, production-ready web apps with Vue. File-based routing, auto-imports, and server-side rendering — all configured out of the box.” The interface is dark, built on **Near Black (#0A0A0A)** with **Mist (#E5E5E5)** text, and **Vivid Teal (#00DC82)** as the main accent.

Type is set in **Outfit** and **Inter**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 6px.

Measured from [nuxt.com](https://nuxt.com/) on November 4, 2026 at 1440×900 and 390×844 from 328 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Near Black (#0A0A0A):** Page background, seen 16 times. Token `background`.
- **Mist (#E5E5E5):** Primary text and headings, seen 12 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 11 times. Token `on-surface-strong`, CSS `--color-white`.
- **Light Indigo (#BABED8):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Gray (#A1A1A1):** Muted text and metadata, seen 12 times. Token `on-surface-muted`.
- **Charcoal (#171717):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Graphite (#262626):** Cards and panels, seen 8 times. Token `surface-container`.
- **Vivid Teal 10% (#00DC821A):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Near Black 75% (#0A0A0ABF):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Graphite (#262626):** Borders and dividers, seen 10 times. Token `outline`.
- **Vivid Teal (#00DC82):** Primary buttons and calls to action, seen 8 times. Token `primary`, CSS `--ui-color-success-400`.
- **Charcoal (#171717):** Text and icons on primary. Token `on-primary`.
- **Light Cyan (#89DDFF):** Accent in text, fills and borders, seen 20 times. Token `secondary`.
- **Red (#F07178):** Accent in text, fills and borders, seen 10 times. Token `tertiary`.

## Typography

**Outfit** and **Inter** share the interface. Fallback stack: `Outfit, Outfit Fallback: BlinkMacSystemFont, Outfit Fallback: Segoe UI, Outfit Fallback: Helvetica Neue`.

- **headline-display:** Outfit 72px at weight 500, line height 1, tracking -0.025em (48px on mobile). Page title (h1).
- **headline-lg:** Outfit 48px at weight 500, line height 1, tracking -0.025em (30px on mobile). Section headings (h2).
- **body-md:** Inter 14px at weight 400, line height 1.43. Body text.
- **label-lg:** Inter 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** Inter 14px at weight 500, line height 1.43. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 500, line height 1.33. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (79% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 16px, lg 24px, xl 64px.
- **Gaps:** 32px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#171717 → #262626) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklch(0.371 0 none) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.786145 -0.174855 0.0792278 / 0.25) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 144 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #00DC82 fill, #171717 text, 16px/500, 6px radius, padding 8px 12px.
- **button-outline (“Nuxt in 100 seconds”):** #171717 fill, #E5E5E5 text, 16px/500, 6px radius, padding 8px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklch(0.371 0 none) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-ghost (“app.vue”):** #171717 fill, #FFFFFF text, 14px/400, 6px radius, padding 6px 10px.
- **input-field:** transparent fill, #FFFFFF text, 16px/400, 6px radius, padding 8px 44px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklch(0.371 0 none) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **link:** transparent fill, #A1A1A1 text, padding 0px.

## Do's and Don'ts

- Do use #0A0A0A for the page and lift surfaces in small steps: #171717, #262626.
- Do keep text in 4 levels: #E5E5E5, #FFFFFF, #BABED8, #A1A1A1.
- Do reserve #00DC82 for primary actions and key highlights.
- Do set headlines in Outfit with tight tracking (-0.025em).
- Do reuse the measured spacing steps (6px, 16px, 24px).
- Do use 6px corners on most elements.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Outfit and Inter.
- Don't use #00DC82 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.4s. Longer ambient animations run 0.9s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.25, 1, 0.5, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/nuxt.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
