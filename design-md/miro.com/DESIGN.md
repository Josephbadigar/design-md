---
version: alpha
name: Miro
description: "Light interface measured from miro.com: Roobert PRO Medium type with Noto Sans, amber accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#1C1C1E"
  on-surface-muted: "#222428"
  on-surface-subtle: "#555A6A"
  surface-container-low: "#F0F0F0"
  surface-container: "#FDE0F0"
  outline: "#C7CAD5"
  outline-variant: "#E9EAEF"
  primary: "#FDE050"
  on-primary: "#1C1C1E"
  secondary: "#0000EE"
  tertiary: "#00B473"
  error: "#DB4F4F"
  warning: "#FFDD33"
  success: "#0AAE3A"
typography:
  headline-display:
    fontFamily: Roobert PRO Medium
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Roobert PRO Medium
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: -0.03em
  body-md:
    fontFamily: Noto Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.45
  body-sm:
    fontFamily: sans-serif
    fontSize: 12px
    fontWeight: 400
  label-md:
    fontFamily: Noto Sans
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: -0.01em
  label-sm:
    fontFamily: Noto Sans
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.45
rounded:
  sm: 8px
  md: 20px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 28px
  xl: 48px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
    height: 40px
  button-secondary:
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 1px 6px
    height: 48px
  button-tertiary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.background}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 16px
  link:
    textColor: "{colors.secondary}"
---

# Miro Design System

## Overview

Miro describes itself as: “Speed up product development from ideation to launch. Align teams, break tool silos and ship what customers need in one AI-powered visual platform.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Amber (#FDE050)** as the main accent.

Type is set in **Roobert PRO Medium** and **Noto Sans**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [miro.com](https://miro.com/) on October 21, 2026 at 1440×900 and 666×1442 from 359 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #5974FF, #395AFF.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 17 times. Token `on-surface`.
- **Charcoal (#1C1C1E):** Secondary text, seen 35 times. Token `on-surface-variant`.
- **Cool Graphite (#222428):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Dark Blue (#555A6A):** Subtle text and placeholders, seen 14 times. Token `on-surface-subtle`, CSS `--tw-color-input-active`.
- **Mist (#F0F0F0):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Pale Pink (#FDE0F0):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--tw-color-pink`.
- **Cool Silver (#C7CAD5):** Borders and dividers, seen 1 time. Token `outline`.
- **Cool Mist (#E9EAEF):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--tw-color-gray-150`.
- **Amber (#FDE050):** Primary buttons and calls to action, seen 2 times. Token `primary`.
- **Charcoal (#1C1C1E):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#0000EE):** Links and interactive text, seen 33 times. Token `secondary`.
- **Dark Teal (#00B473):** Brand accent (CSS variable), seen 12 times. Token `tertiary`.
- **Red (#DB4F4F):** Errors and destructive states, seen 4 times. Token `error`.
- **Vivid Amber (#FFDD33):** Warnings and highlights, seen 2 times. Token `warning`.
- **Dark Green (#0AAE3A):** Success and positive states, seen 1 time. Token `success`.

## Typography

**Roobert PRO Medium**, **Noto Sans** and **sans-serif** share the interface. Fallback stack: `Roobert PRO Medium, Roobert PRO Medium Placeholder, sans-serif`. Other loaded fonts: Open Sans, Roobert PRO SemiBold, Roobert PRO SemiBold Italic, Inter.

- **headline-display:** Roobert PRO Medium 48px at weight 400, line height 1.15, tracking -0.03em. Page title (h1).
- **headline-lg:** Roobert PRO Medium 24px at weight 400, line height 1.15, tracking -0.03em. Section headings (h2).
- **body-md:** Noto Sans 18px at weight 400, line height 1.45. Body text.
- **body-sm:** sans-serif 12px at weight 400. Secondary and small text.
- **label-md:** Noto Sans 16px at weight 600, line height 1.5, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** Noto Sans 14px at weight 600, line height 1.45. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 68% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 10px, lg 28px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 576px, 767px, 768px, 809.98px, 810px, 992px, 1023px, 1024px, 1199px, 1199.98px, 1200px, 1280px, 1365px, 1365.98px, 1366px, 1400px, 1920px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F0F0F0 → #FDE0F0) and hairline rings:

- `rgb(122, 144, 254) 0px 1px 1px 0px inset`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 84 elements.
- **md (20px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“See here why we rebuilt Miro →”):** #FDE050 fill, #1C1C1E text, 16px/900, 8px radius, padding 8px 12px.
- **button-secondary (“Get started free”):** transparent fill, #FFFFFF text, 16px/600, 8px radius, padding 1px 6px.
- **button-tertiary (“Get started free”):** #1C1C1E fill, #FFFFFF text, 14px/600, 8px radius, padding 8px 12px.
- **button-ghost (“Product”):** transparent fill, #1C1C1E text, 14px/500, 8px radius, padding 8px 12px.
- **input-field (“Enter your work email”):** #FFFFFF fill, #1C1C1E text, 16px/400, 8px radius, padding 16px, border 1px solid #E9EAEF.
- **link:** transparent fill, #0000EE text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F0F0F0, #FDE0F0.
- Do keep text in 4 levels: #000000, #1C1C1E, #222428, #555A6A.
- Do reserve #FDE050 for primary actions and key highlights.
- Do set headlines in Roobert PRO Medium with tight tracking (-0.03em).
- Do reuse the measured spacing steps (8px, 10px, 28px).
- Do use 8px corners on most elements; larger surfaces also use 20px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Roobert PRO Medium, Noto Sans and sans-serif.
- Don't use #FDE050 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.15s, 0.6s, 0.2s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.16, 1, 0.3, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/miro.com/), the free DESIGN.md generator.
