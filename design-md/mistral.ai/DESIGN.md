---
version: alpha
name: Mistral
description: "Dark interface measured from mistral.ai: ALTMistral type with Inter, vivid amber accents, tonal surfaces and 6px corners."
colors:
  background: "#101013"
  surface: "#101013"
  on-surface: "#FAFAF4"
  on-background: "#FAFAF4"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#A1A1AA"
  on-surface-muted: "#6D6D78"
  surface-container-low: "#1A1A1E"
  overlay: "#F9F9FB0D"
  outline: "#27272B"
  primary: "#FFAF01"
  on-primary: "#000000"
  inverse-surface: "#F1F1F3"
  secondary: "#FF8204"
  tertiary: "#FA500F"
  error: "#E51300"
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
  body-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.54
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
  margin: 40px
components:
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 16px
  link:
    textColor: "{colors.on-surface}"
---

# Mistral Design System

## Overview

Mistral describes itself as: “Frontier open-weight models you own and control. Customize with Forge, deploy with Studio, run on-prem, your VPC, or our cloud.” The interface is dark, built on **Charcoal (#101013)** with **Warm Snow (#FAFAF4)** text, and **Vivid Amber (#FFAF01)** as the main accent.

Type is set in **ALTMistral** and **Inter**. Headlines run large with tight negative tracking; body text is 13px. The surface language is flat. Corners are mostly 6px.

Measured from [mistral.ai](https://mistral.ai/) on October 21, 2026 at 1440×900 and 390×844 from 327 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Charcoal (#101013):** Page background, seen 12 times. Token `background`, CSS `--color-steel-950`.
- **Warm Snow (#FAFAF4):** Primary text and headings, seen 32 times. Token `on-surface`, CSS `--color-surface-invert`.
- **White (#FFFFFF):** Headings and emphasis, seen 12 times. Token `on-surface-strong`, CSS `--color-white`.
- **Cool Gray (#A1A1AA):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Cool Slate (#6D6D78):** Muted text and metadata, seen 3 times. Token `on-surface-muted`, CSS `--color-steel-500`.
- **Charcoal (#1A1A1E):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--color-surface-neutral-secondary`.
- **Snow 5% (#F9F9FB0D):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Graphite (#27272B):** Borders and dividers, seen 38 times. Token `outline`.
- **Vivid Amber (#FFAF01):** Brand color in the logo, seen 2 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Mist (#F1F1F3):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Vivid Orange (#FF8204):** Brand color in the logo, seen 24 times. Token `secondary`, CSS `--color-tangerine-500`.
- **Vivid Orange (#FA500F):** Brand color in the logo, seen 16 times. Token `tertiary`, CSS `--color-orange-600`.
- **Vivid Red (#E51300):** Errors and destructive states, seen 3 times. Token `error`.

## Typography

**ALTMistral** and **Inter** share the interface. Fallback stack: `ALTMistral, sans-serif`. Other loaded fonts: Axeptio Inter, Axeptio Source Sans 3.

- **headline-display:** ALTMistral 56px at weight 500, line height 1.07, tracking -0.01em. Page title (h1).
- **headline-lg:** ALTMistral 44px at weight 500, line height 1.18, tracking -0.01em (24px on mobile). Section headings (h2).
- **headline-md:** ALTMistral 32px at weight 500, line height 1.25. Sub-section headings.
- **headline-sm:** ALTMistral 24px at weight 500, line height 1.33. Card and feature titles.
- **title-lg:** Inter 20px at weight 400, line height 1.4, tracking -0.02em. Small titles.
- **body-md:** Inter 13px at weight 400, line height 1.54. Body text.
- **label-md:** Inter 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** ALTMistral 14px at weight 500, line height 1.43, tracking 0.02em. Small labels and badges.

## Layout

Spacing follows a 8px grid: 91% of measured gaps and paddings are multiples of 8px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Sections:** 160px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Page margin:** 40px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#1A1A1E) and #27272B borders.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 40 elements.
- **sm (4px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Sovereign AI”):** transparent fill, #FFFFFF text, 16px/400, padding 16px.
- **link:** transparent fill, #FAFAF4 text, padding 0px.

## Do's and Don'ts

- Do use #101013 for the page and lift surfaces in small steps: #1A1A1E.
- Do keep text in 4 levels: #FAFAF4, #FFFFFF, #A1A1AA, #6D6D78.
- Do use #FFAF01 as the brand accent: header, logo and key highlights.
- Do set headlines in ALTMistral with tight tracking (-0.01em).
- Do keep spacing on the 8px grid.
- Do use 6px corners on most elements; larger surfaces also use 4px.
- Don't use #6D6D78 for body text; it reaches 3.7:1 on #101013. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond ALTMistral and Inter.
- Don't use #FFAF01 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.5s. Longer ambient animations run 2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mistral.ai/), the free DESIGN.md generator.
