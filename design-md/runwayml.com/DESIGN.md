---
version: alpha
name: Runway
description: "Light interface measured from runwayml.com: abcNormal type, vivid indigo accents, tonal surfaces and 6px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#404040"
  on-background: "#404040"
  on-surface-strong: "#0C0C0C"
  on-surface-variant: "#1A1A1A"
  on-surface-muted: "#6B7280"
  surface-container-low: "#F7F7F7"
  surface-container: "#EEF1F5"
  overlay: "#F7F7F70D"
  outline: "#E5E7EB"
  primary: "#2B22FA"
  on-primary: "#FFFFFF"
  inverse-surface: "#262626"
typography:
  headline-display:
    fontFamily: abcNormal
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.015em
  headline-lg:
    fontFamily: abcNormal
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1
  headline-md:
    fontFamily: abcNormal
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1
  body-md:
    fontFamily: abcNormal
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.25
  body-sm:
    fontFamily: abcNormal
    fontSize: 11px
    fontWeight: 450
    lineHeight: 1.3
  label-md:
    fontFamily: abcNormal
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.01em
  label-sm:
    fontFamily: abcNormal
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: abcNormal
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.015em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 28px
  xl: 64px
  gutter: 8px
  section: 100px
  container: 1600px
components:
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 6px 10px
    height: 32px
  button-outline-hover:
    backgroundColor: "#E7EAF0"
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 8px 12px
    height: 40px
  button-ghost-hover:
    backgroundColor: "{colors.background}"
  button-secondary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 6px 10px
    height: 32px
  link:
    textColor: "{colors.on-primary}"
---

# Runway Design System

## Overview

Runway describes itself as: “Runway is building foundational Real-World Intelligence that can understand, simulate and act in the world. We offer products and services built on-top of this intelligence to empower individuals and organizations to do ” The interface is light, built on **White (#FFFFFF)** with **Graphite (#404040)** text, and **Vivid Indigo (#2B22FA)** as the main accent.

Type is set in **abcNormal**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 6px.

Measured from [runwayml.com](https://runway.com/) on October 21, 2026 at 1440×900 and 390×844 from 342 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Graphite (#404040):** Primary text and headings, seen 18 times. Token `on-surface`.
- **Charcoal (#0C0C0C):** Headings and emphasis, seen 12 times. Token `on-surface-strong`.
- **Charcoal (#1A1A1A):** Secondary text, seen 11 times. Token `on-surface-variant`.
- **Cool Slate (#6B7280):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Snow (#F7F7F7):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Cool Mist (#EEF1F5):** Cards and panels, seen 7 times. Token `surface-container`.
- **Snow 5% (#F7F7F70D):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Cool Mist (#E5E7EB):** Borders and dividers, seen 2 times. Token `outline`.
- **Vivid Indigo (#2B22FA):** Brand color in the header. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Graphite (#262626):** High-contrast fills, seen 4 times. Token `inverse-surface`.

## Typography

**abcNormal** carries the whole interface. Fallback stack: `abcNormal, abcNormal Fallback`. Other loaded fonts: abcNormal Fallback.

- **headline-display:** abcNormal 56px at weight 400, line height 1.1, tracking -0.015em (36px on mobile). Page title (h1).
- **headline-lg:** abcNormal 24px at weight 400, line height 1. Section headings (h2).
- **headline-md:** abcNormal 20px at weight 400, line height 1. Sub-section headings.
- **body-md:** abcNormal 14px at weight 400, line height 1.25. Body text.
- **body-sm:** abcNormal 11px at weight 450, line height 1.3. Secondary and small text.
- **label-md:** abcNormal 16px at weight 400, line height 1.3, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** abcNormal 14px at weight 600, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (72% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 10px, lg 28px, xl 64px.
- **Sections:** 100px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1600px.
- **Breakpoints:** 640px, 768px, 1024px, 1200px, 1280px, 1440px, 1536px, 1600px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F7F7F7 → #EEF1F5) and #E5E7EB borders.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 48 elements.
- **sm (4px):** 20 elements.
- **lg (8px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Enterprise Sales”):** #EEF1F5 fill, #1A1A1A text, 14px/600, 6px radius, padding 6px 10px.
- **button-outline-hover:** background #E7EAF0, text #1A1A1A on hover.
- **button-ghost (“Try Runway for free”):** #F7F7F7 fill, #0C0C0C text, 16px/600, 8px radius, padding 8px 12px.
- **button-ghost-hover:** background #FFFFFF, text #0C0C0C on hover.
- **button-secondary (“Try Runway”):** #262626 fill, #FFFFFF text, 14px/600, 6px radius, padding 6px 10px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F7F7F7, #EEF1F5.
- Do keep text in 4 levels: #404040, #0C0C0C, #1A1A1A, #6B7280.
- Do use #2B22FA as the brand accent: header, logo and key highlights.
- Do set headlines in abcNormal with tight tracking (-0.015em).
- Do reuse the measured spacing steps (8px, 10px, 28px).
- Do use 6px corners on most elements; larger surfaces also use 4px and 8px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond abcNormal.
- Don't use #2B22FA for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/runwayml.com/), the free DESIGN.md generator.
