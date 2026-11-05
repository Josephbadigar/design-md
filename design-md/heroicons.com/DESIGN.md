---
version: alpha
name: Heroicons
description: "Light interface measured from heroicons.com: Inter var type, light violet accents, tonal surfaces and 12px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0F172A"
  on-background: "#0F172A"
  on-surface-variant: "#64748B"
  surface-container-low: "#F8FAFC"
  surface-container: "#F1F5F9"
  outline: "#3341551A"
  outline-variant: "#94A3B833"
  primary: "#A78BFA"
  on-primary: "#000000"
  secondary: "#8B5CF6"
typography:
  headline-display:
    fontFamily: Inter var
    fontSize: 36px
    fontWeight: 800
    lineHeight: 1.11
    letterSpacing: -0.025em
  body-md:
    fontFamily: Inter var
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.85
  label-md:
    fontFamily: Inter var
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Inter var
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.85
  headline-display-mobile:
    fontFamily: Inter var
    fontSize: 28px
    fontWeight: 800
    lineHeight: 1.29
    letterSpacing: -0.025em
rounded:
  sm: 8px
  md: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 12px
  section: 80px
components:
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px
    height: 36px
  button-ghost:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-variant}"
    rounded: "{rounded.full}"
    padding: 6px 12px 6px 10px
    height: 30px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 24px 16px 24px 36px
  link:
    textColor: "{colors.on-surface}"
---

# Heroicons Design System

## Overview

Heroicons describes itself as: “Beautiful hand-crafted SVG icons, by the makers of Tailwind CSS.” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#0F172A)** text, and **Light Violet (#A78BFA)** as the main accent.

Type is set in **Inter var**. Headlines run large with tight negative tracking; body text is 13px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 12px.

Measured from [heroicons.com](https://heroicons.com/) on November 4, 2026 at 1440×900 and 390×844 from 313 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`, CSS `--tw-ring-offset-color`.
- **Deep Blue (#0F172A):** Primary text and headings, seen 8 times. Token `on-surface`.
- **Blue (#64748B):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Snow (#F8FAFC):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Cool Snow (#F1F5F9):** Cards and panels, seen 1 time. Token `surface-container`.
- **Dark Blue 10% (#3341551A):** Borders and dividers, seen 1 time. Token `outline`.
- **Blue 20% (#94A3B833):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Light Violet (#A78BFA):** Brand color in the header, seen 1 time. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Violet (#8B5CF6):** Accent in the logo, seen 2 times. Token `secondary`.

## Typography

**Inter var** carries the whole interface. Fallback stack: `Inter var, ui-sans-serif, system-ui, sans-serif`.

- **headline-display:** Inter var 36px at weight 800, line height 1.11, tracking -0.025em (28px on mobile). Page title (h1).
- **body-md:** Inter var 13px at weight 400, line height 1.85. Body text.
- **label-md:** Inter var 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Inter var 13px at weight 600, line height 1.85. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 69% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 12px, lg 24px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 480px, 640px, 768px, 1024px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F8FAFC → #F1F5F9) and hairline rings:

- `rgb(255, 255, 255) 0px 0px 0px 0px inset, rgba(15, 23, 42, 0.08) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **md (12px):** 368 elements.
- **sm (8px):** 16 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Outline”):** #F1F5F9 fill, #0F172A text, 16px/400, 9999px radius, padding 0px.
- **button-ghost (“v2.1.5”):** #F1F5F9 fill, #64748B text, 12px/600, 9999px radius, padding 6px 12px 6px 10px, border 1px solid #3341551A.
- **input-field (“Search all icons...”):** transparent fill, #0F172A text, 13px/400, 8px radius, padding 24px 16px 24px 36px.
- **link:** transparent fill, #0F172A text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8FAFC, #F1F5F9.
- Do keep text in 2 levels: #0F172A, #64748B.
- Do use #A78BFA as the brand accent: header, logo and key highlights.
- Do set headlines in Inter var with tight tracking (-0.025em).
- Do reuse the measured spacing steps (6px, 12px, 24px).
- Do use 12px corners on most elements; larger surfaces also use 8px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Inter var.
- Don't use #A78BFA for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.5s, 0.15s, 0.2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/heroicons.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
