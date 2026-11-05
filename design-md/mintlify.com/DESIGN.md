---
version: alpha
name: Mintlify
description: "Light interface measured from mintlify.com: arizonaFlare type with inter, dark teal accents, tonal surfaces and 6px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#08090A"
  on-background: "#08090A"
  on-surface-strong: "#000000"
  on-surface-variant: "#121715"
  on-surface-muted: "#969E9B"
  surface-container-low: "#FEFDFB"
  surface-container: "#FAF8F5"
  surface-container-high: "#F1F0EE"
  overlay: "#1FA77A14"
  outline: "#F1F0EE"
  outline-variant: "#08090A12"
  primary: "#0C8C5E"
  on-primary: "#000000"
  secondary: "#18E299"
typography:
  headline-display:
    fontFamily: arizonaFlare
    fontSize: 50px
    fontWeight: 400
    lineHeight: 1.04
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: inter
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1.09
    letterSpacing: -0.02em
  headline-md:
    fontFamily: inter
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: inter
    fontSize: 35px
    fontWeight: 500
    lineHeight: 1.14
    letterSpacing: -0.01em
  body-md:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.14
  headline-display-mobile:
    fontFamily: arizonaFlare
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-md-mobile:
    fontFamily: inter
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.14
    letterSpacing: -0.026em
rounded:
  sm: 2px
  md: 4px
  lg: 6px
  xl: 12px
spacing:
  xs: 4px
  sm: 6px
  md: 12px
  lg: 32px
  xl: 40px
  gutter: 16px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 8px 14px
    height: 34px
  button-ghost:
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 4px 10px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Mintlify Design System

## Overview

Mintlify describes itself as: “Self-updating documentation for startups, enterprises, and agents.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#08090A)** text, and **Dark Teal (#0C8C5E)** as the main accent.

Type is set in **arizonaFlare** and **inter**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 6px.

Measured from [mintlify.com](https://www.mintlify.com/) on November 4, 2026 at 1440×900 and 390×844 from 406 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **White (#FFFFFF):** Page background, seen 7 times. Token `background`, CSS `--color-white`.
- **Near Black (#08090A):** Primary text and headings, seen 44 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 4 times. Token `on-surface-strong`, CSS `--tw-mask-bottom-from-color`.
- **Charcoal (#121715):** Secondary text, seen 8 times. Token `on-surface-variant`, CSS `--consent-widget-link-text-color`.
- **Gray (#969E9B):** Muted text and metadata, seen 5 times. Token `on-surface-muted`.
- **Snow (#FEFDFB):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`, CSS `--consent-banner-background-color`.
- **Snow (#FAF8F5):** Cards and panels, seen 14 times. Token `surface-container`.
- **Mist (#F1F0EE):** Hover and pressed fills, seen 5 times. Token `surface-container-high`.
- **Teal 8% (#1FA77A14):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Mist (#F1F0EE):** Borders and dividers, seen 23 times. Token `outline`.
- **Near Black 7% (#08090A12):** Secondary dividers, seen 9 times. Token `outline-variant`.
- **Dark Teal (#0C8C5E):** Brand color in the logo, seen 66 times. Token `primary`, CSS `--consent-widget-branding-link-color`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Teal (#18E299):** Accent in the logo, seen 1 time. Token `secondary`, CSS `--color-speedy-mint`.

## Typography

**arizonaFlare** and **inter** share the interface. Fallback stack: `arizonaFlare, arizonaFlare Fallback, serif`. Other loaded fonts: paperMono.

- **headline-display:** arizonaFlare 50px at weight 400, line height 1.04, tracking -0.04em (40px on mobile). Page title (h1).
- **headline-lg:** inter 44px at weight 400, line height 1.09, tracking -0.02em. Section headings (h2).
- **headline-md:** inter 36px at weight 500, line height 1.11, tracking -0.02em (28px on mobile). Sub-section headings.
- **headline-sm:** inter 35px at weight 500, line height 1.14, tracking -0.01em. Card and feature titles.
- **body-md:** inter 14px at weight 400, line height 1.43. Body text.
- **label-md:** inter 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** inter 14px at weight 500, line height 1.14. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (77% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 12px, lg 32px, xl 40px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 480px, 640px, 899px, 935px, 950px, 965px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FEFDFB → #FAF8F5 → #F1F0EE) and #F1F0EE borders.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **lg (6px):** 96 elements.
- **md (4px):** 92 elements.
- **xl (12px):** 36 elements.
- **sm (2px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Contact sales”):** #08090A fill, #FFFFFF text, 14px/500, 4px radius, padding 8px 14px.
- **button-ghost (“Products”):** transparent fill, 14px/500, padding 4px 10px.
- **card:** #FAF8F5 fill, #000000 text, 16px/400, 6px radius, padding 0px.
- **link:** transparent fill, #08090A text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FEFDFB, #FAF8F5, #F1F0EE.
- Do keep text in 4 levels: #08090A, #000000, #121715, #969E9B.
- Do use #0C8C5E as the brand accent: header, logo and key highlights.
- Do set headlines in arizonaFlare with tight tracking (-0.04em).
- Do reuse the measured spacing steps (6px, 12px, 32px).
- Do use 6px corners on most elements; larger surfaces also use 4px, 12px and 2px.
- Don't use #969E9B for body text; it reaches 2.74:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond arizonaFlare and inter.
- Don't use #0C8C5E for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.1s, 0.15s, 0.3s. Longer ambient animations run 0.7s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mintlify.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
