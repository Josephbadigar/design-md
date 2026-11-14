---
version: alpha
name: Mistral
description: "Light interface measured from mistral.ai: ALTMistral type with Inter, red accents, tonal surfaces and 6px corners."
colors:
  background: "#FBFBF8"
  surface: "#FBFBF8"
  on-surface: "#18181B"
  on-background: "#18181B"
  on-surface-variant: "#27272A"
  on-surface-muted: "#3F3F47"
  on-surface-subtle: "#71717B"
  surface-container-low: "#F4F4F5"
  surface-container: "#F5F4EF"
  overlay: "#07070B0D"
  outline: "#E4E3DE"
  primary: "#C4001D"
  on-primary: "#FFFFFF"
  inverse-surface: "#09090B"
  secondary: "#FA500F"
  tertiary: "#FF8204"
typography:
  headline-display:
    fontFamily: ALTMistral
    fontSize: 56px
    fontWeight: 500
    lineHeight: 1.07
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: ALTMistral
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.18
    letterSpacing: -0.01em
  headline-md:
    fontFamily: ALTMistral
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
  headline-sm:
    fontFamily: ALTMistral
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
  title-lg:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.02em
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: ALTMistral
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0.02em
  headline-lg-mobile:
    fontFamily: ALTMistral
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.17
    letterSpacing: -0.01em
rounded:
  sm: 4px
  md: 6px
spacing:
  base: 8px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 16px
  section: 160px
components:
  button-primary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px 16px
    height: 48px
  button-ghost:
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 16px
  card:
    backgroundColor: "{colors.surface-container}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 8px 16px
  link:
    textColor: "{colors.on-surface}"
---

# Mistral Design System

## Overview

Mistral describes itself as: “Frontier open-weight models you own and control. Customize with Forge, deploy with Studio, run on-prem, your VPC, or our cloud.” The interface is light, built on **Snow (#FBFBF8)** with **Charcoal (#18181B)** text, and **Red (#C4001D)** as the main accent.

Type is set in **ALTMistral** and **Inter**. Headlines run large with tight negative tracking; body text is compact. The surface language is flat. Corners are mostly 6px.

Measured from [mistral.ai](https://mistral.ai/) on November 13, 2026 at 1440×900 and 390×844 from 332 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Snow (#FBFBF8):** Page background, seen 8 times. Token `background`.
- **Charcoal (#18181B):** Primary text and headings, seen 45 times. Token `on-surface`.
- **Graphite (#27272A):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Cool Graphite (#3F3F47):** Muted text and metadata, seen 3 times. Token `on-surface-muted`.
- **Cool Slate (#71717B):** Subtle text and placeholders, seen 5 times. Token `on-surface-subtle`.
- **Snow (#F4F4F5):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **Warm Mist (#F5F4EF):** Cards and panels, seen 3 times. Token `surface-container`.
- **Near Black 5% (#07070B0D):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Warm Mist (#E4E3DE):** Borders and dividers, seen 38 times. Token `outline`.
- **Red (#C4001D):** Brand accent (CSS variable), seen 2 times. Token `primary`, CSS `--color-chart-brand-4`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Near Black (#09090B):** High-contrast fills, seen 2 times. Token `inverse-surface`.
- **Vivid Orange (#FA500F):** Accent in the logo, seen 1 time. Token `secondary`, CSS `--color-orange-600`.
- **Vivid Orange (#FF8204):** Accent in the logo, seen 2 times. Token `tertiary`, CSS `--color-tangerine-500`.

## Typography

**ALTMistral** and **Inter** share the interface. Fallback stack: `ALTMistral, sans-serif`.

- **headline-display:** ALTMistral 56px at weight 500, line height 1.07, tracking -0.01em. Page title (h1).
- **headline-lg:** ALTMistral 44px at weight 500, line height 1.18, tracking -0.01em (24px on mobile). Section headings (h2).
- **headline-md:** ALTMistral 32px at weight 500, line height 1.25. Sub-section headings.
- **headline-sm:** ALTMistral 24px at weight 500, line height 1.33. Card and feature titles.
- **title-lg:** Inter 20px at weight 400, line height 1.4, tracking -0.02em. Small titles.
- **label-md:** Inter 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** ALTMistral 14px at weight 500, line height 1.43, tracking 0.02em. Small labels and badges.

## Layout

Spacing follows a 8px grid: 93% of measured gaps and paddings are multiples of 8px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Sections:** 160px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F4F4F5 → #F5F4EF) and #E4E3DE borders.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 40 elements.
- **sm (4px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start building”):** #09090B fill, #FFFFFF text, 16px/500, padding 0px 16px.
- **button-ghost (“Sovereign AI”):** transparent fill, 16px/400, padding 16px.
- **card:** #F5F4EF fill, 16px/400, padding 8px 16px, border 1px solid #E4E3DE.
- **link:** transparent fill, #18181B text, padding 0px.

## Do's and Don'ts

- Do use #FBFBF8 for the page and lift surfaces in small steps: #F4F4F5, #F5F4EF.
- Do keep text in 4 levels: #18181B, #27272A, #3F3F47, #71717B.
- Do use #C4001D as the brand accent: header, logo and key highlights.
- Do set headlines in ALTMistral with tight tracking (-0.01em).
- Do keep spacing on the 8px grid.
- Do use 6px corners on most elements; larger surfaces also use 4px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond ALTMistral and Inter.
- Don't use #C4001D for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.5s. Longer ambient animations run 2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mistral.ai/), the free DESIGN.md generator (engine 2026.10.29+f0c146f7cdfd).
