---
version: alpha
name: Evernote
description: "Light interface measured from evernote.com: Figtree type with Inter, lime accents, tonal surfaces and 5px corners."
colors:
  background: "#F4EEE5"
  surface: "#F4EEE5"
  on-surface: "#141414"
  on-background: "#141414"
  on-surface-strong: "#000000"
  on-surface-variant: "#262626"
  on-surface-muted: "#4E4D4C"
  surface-container-low: "#F9F6F2"
  surface-container: "#FFFFFF"
  outline: "#A1A1A1"
  outline-variant: "#E7E7E7"
  primary: "#94E130"
  on-primary: "#141414"
  secondary: "#4D64FF"
typography:
  headline-display:
    fontFamily: Figtree
    fontSize: 72px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: Figtree
    fontSize: 50px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.05em
  headline-md:
    fontFamily: Figtree
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-sm:
    fontFamily: Figtree
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.1
  title-lg:
    fontFamily: Figtree
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.3
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
  body-lg:
    fontFamily: Figtree
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0.01em
  label-md:
    fontFamily: Figtree
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Figtree
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.05em
  headline-lg-mobile:
    fontFamily: Figtree
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.05em
  headline-md-mobile:
    fontFamily: Figtree
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.03em
rounded:
  sm: 5px
  md: 10px
  lg: 16px
spacing:
  base: 4px
  xs: 2px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 40px
  section: 120px
  margin: 20px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 16px 40px
    height: 59px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.surface-container}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 10px 28px
    height: 46px
  button-secondary-hover:
    backgroundColor: "#00A82D"
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 10px 28px
    height: 46px
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px 6px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 80px 40px 0px 40px
  link:
    textColor: "{colors.on-surface}"
---

# Evernote Design System

## Overview

Evernote describes itself as: “Our note taking app helps you capture and prioritize ideas, projects and to-do lists, so nothing falls through the cracks. Start your free trial today!” The interface is light, built on **Warm Mist (#F4EEE5)** with **Charcoal (#141414)** text, and **Lime (#94E130)** as the main accent.

Type is set in **Figtree** and **Inter**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 5px.

Measured from [evernote.com](https://evernote.com/) on November 4, 2026 at 1440×900 and 390×844 from 417 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Warm Mist (#F4EEE5):** Page background, seen 6 times. Token `background`, CSS `--color-bg-secondary`.
- **Charcoal (#141414):** Primary text and headings, seen 92 times. Token `on-surface`, CSS `--color-text-primary`.
- **Near Black (#000000):** Headings and emphasis, seen 7 times. Token `on-surface-strong`.
- **Graphite (#262626):** Secondary text, seen 3 times. Token `on-surface-variant`, CSS `--color-text-secondary`.
- **Slate (#4E4D4C):** Muted text and metadata, seen 24 times. Token `on-surface-muted`, CSS `--color-text-tertiary`.
- **Warm Snow (#F9F6F2):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`, CSS `--color-bg-primary`.
- **White (#FFFFFF):** Cards and panels, seen 27 times. Token `surface-container`, CSS `--tw-ring-offset-color`.
- **Gray (#A1A1A1):** Borders and dividers, seen 8 times. Token `outline`, CSS `--color-stroke-buttons`.
- **Mist (#E7E7E7):** Secondary dividers, seen 6 times. Token `outline-variant`, CSS `--color-stroke-cards`.
- **Lime (#94E130):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **Charcoal (#141414):** Text and icons on primary. Token `on-primary`.
- **Indigo (#4D64FF):** Accent, seen 2 times. Token `secondary`.

## Typography

**Figtree** and **Inter** share the interface. Fallback stack: `Figtree, Figtree Fallback`.

- **headline-display:** Figtree 72px at weight 600, line height 1, tracking -0.05em (36px on mobile). Page title (h1).
- **headline-lg:** Figtree 50px at weight 600, line height 1.1, tracking -0.05em (32px on mobile). Section headings (h2).
- **headline-md:** Figtree 40px at weight 600, line height 1.1, tracking -0.03em (28px on mobile). Sub-section headings.
- **headline-sm:** Figtree 24px at weight 600, line height 1.1. Card and feature titles.
- **title-lg:** Figtree 20px at weight 600, line height 1.3. Small titles.
- **body-md:** Inter 16px at weight 400, line height 1.3. Body text.
- **body-lg:** Figtree 18px at weight 400, line height 1.6, tracking 0.01em. Lead paragraphs.
- **label-md:** Figtree 16px at weight 400, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 93% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 2px, sm 8px, md 16px, lg 32px, xl 40px.
- **Sections:** 120px vertical padding between major sections.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 400px, 425px, 426px, 480px, 500px, 550px, 600px, 768px, 896px, 1024px, 1280px, 1440px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F9F6F2 → #FFFFFF) and #A1A1A1 borders.

## Shapes

Most elements use 5px corners. Measured radii, most used first:

- **sm (5px):** 204 elements.
- **md (10px):** 124 elements.
- **lg (16px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Discover more”):** #94E130 fill, #141414 text, 16px/400, 5px radius, padding 16px 40px.
- **button-secondary (“Start for free”):** #141414 fill, #FFFFFF text, 16px/400, 5px radius, padding 10px 28px.
- **button-secondary-hover:** background #00A82D, text #FFFFFF on hover.
- **button-outline (“Download”):** transparent fill, #141414 text, 16px/400, 5px radius, padding 10px 28px, border 1px solid #A1A1A1.
- **button-ghost (“Explore”):** transparent fill, #000000 text, 16px/400, padding 0px 6px.
- **card:** #F4EEE5 fill, #000000 text, 16px/400, 16px radius, padding 80px 40px 0px 40px, border 1px solid #E7E7E7.
- **link:** transparent fill, #141414 text, padding 0px.

## Do's and Don'ts

- Do use #F4EEE5 for the page and lift surfaces in small steps: #F9F6F2, #FFFFFF.
- Do keep text in 4 levels: #141414, #000000, #262626, #4E4D4C.
- Do reserve #94E130 for primary actions and key highlights.
- Do set headlines in Figtree with tight tracking (-0.05em).
- Do keep spacing on the 4px grid.
- Do use 5px corners on most elements; larger surfaces also use 10px and 16px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Figtree and Inter.
- Don't use #94E130 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/evernote.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
