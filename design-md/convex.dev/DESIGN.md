---
version: alpha
name: Convex
description: "Dark monochrome interface measured from convex.dev: neue-haas-grotesk-display type with gtAmerica, tonal surfaces and 4px corners."
colors:
  background: "#281D1D"
  surface: "#281D1D"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#FAF4E9"
  on-surface-muted: "#F6EEDB"
  on-surface-subtle: "#C2C2C2"
  surface-container-low: "#292929"
  surface-container: "#141414"
  surface-container-high: "#1A0F0F"
  surface-container-highest: "#38383A"
  overlay: "#FFFFFF0D"
  overlay-strong: "#FAF4E940"
  outline: "#524946"
  outline-variant: "#FFFFFF26"
  primary: "#38383A"
  on-primary: "#FFFFFF"
  secondary: "#FFD7BF"
  tertiary: "#F3B01C"
  warning: "#F4DCB4"
typography:
  headline-display:
    fontFamily: neue-haas-grotesk-display
    fontSize: 60px
    fontWeight: 900
    lineHeight: 0.85
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: gtAmerica
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.025em
  headline-md:
    fontFamily: gtAmerica
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.5
  body-md:
    fontFamily: gtAmerica
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.25
  body-lg:
    fontFamily: gtAmerica
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: gtAmerica
    fontSize: 14px
    fontWeight: 300
    lineHeight: 1.5
  caption:
    fontFamily: gtAmerica
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: 0.018em
  label-lg:
    fontFamily: gtAmerica
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: gtAmerica
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: gtAmerica
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: neue-haas-grotesk-display
    fontSize: 46px
    fontWeight: 900
    lineHeight: 0.85
    letterSpacing: -0.04em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 48px
  gutter: 8px
  section: 60px
  container: 576px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 12px
    height: 64px
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "#A9A972"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 12px
    height: 45px
  button-ghost:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 4px 8px 4px 4px
    height: 30px
  link:
    textColor: "{colors.surface-container}"
---

# Convex Design System

## Overview

Convex describes itself as: “All gas, no breakages. Convex is the reactive backend platform that keeps up with you and your agents.” The interface is dark, built on **Warm Charcoal (#281D1D)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **neue-haas-grotesk-display** and **gtAmerica**. Headlines run large with tight negative tracking; body text is 15px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [convex.dev](https://www.convex.dev/) on November 4, 2026 at 1440×900 and 390×844 from 312 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 18 roles, plus gradient stops #73312B.

- **Warm Charcoal (#281D1D):** Page background, seen 2 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 64 times. Token `on-surface`, CSS `--tw-ring-offset-color`.
- **Warm Mist (#FAF4E9):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Pale Amber (#F6EEDB):** Muted text and metadata, seen 14 times. Token `on-surface-muted`, CSS `--color-antiqueWhite`.
- **Silver (#C2C2C2):** Subtle text and placeholders, seen 9 times. Token `on-surface-subtle`.
- **Graphite (#292929):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Charcoal (#141414):** Cards and panels, seen 4 times. Token `surface-container`, CSS `--color-neutral-n12`.
- **Warm Charcoal (#1A0F0F):** Hover and pressed fills, seen 10 times. Token `surface-container-high`.
- **Graphite (#38383A):** Highest raised elements, seen 5 times. Token `surface-container-highest`.
- **White 5% (#FFFFFF0D):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Warm Mist 25% (#FAF4E940):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Warm Graphite (#524946):** Borders and dividers, seen 6 times. Token `outline`.
- **White 15% (#FFFFFF26):** Secondary dividers, seen 4 times. Token `outline-variant`.
- **Graphite (#38383A):** Primary buttons and calls to action, seen 5 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Pale Orange (#FFD7BF):** Accent in text, fills and borders, seen 5 times. Token `secondary`.
- **Vivid Amber (#F3B01C):** Accent in logos and imagery, seen 1 time. Token `tertiary`, CSS `--color-yellow-y3`.
- **Light Orange (#F4DCB4):** Warnings and highlights, seen 6 times. Token `warning`.

## Typography

**neue-haas-grotesk-display** and **gtAmerica** share the interface. Fallback stack: `neue-haas-grotesk-display, gtAmerica, sans-serif`. Other loaded fonts: vcr, publico, plex.

- **headline-display:** neue-haas-grotesk-display 60px at weight 900, line height 0.85, tracking -0.04em, uppercase (46px on mobile). Page title (h1).
- **headline-lg:** gtAmerica 40px at weight 700, line height 1, tracking -0.025em. Section headings (h2).
- **headline-md:** gtAmerica 20px at weight 500, line height 1.5. Sub-section headings.
- **body-md:** gtAmerica 15px at weight 400, line height 1.25. Body text.
- **body-lg:** gtAmerica 18px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** gtAmerica 14px at weight 300, line height 1.5. Secondary and small text.
- **caption:** gtAmerica 12px at weight 400, line height 1.38, tracking 0.018em. Captions and fine print.
- **label-lg:** gtAmerica 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** gtAmerica 15px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** gtAmerica 14px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing follows a 4px grid: 90% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 48px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 576px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 2px 11px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 56 elements.
- **lg (8px):** 32 elements.
- **md (6px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Stripe”):** #38383A fill, #FFFFFF text, 16px/400, 8px radius, padding 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 2px 11px 0px`.
- **button-outline (“$ npm install @convex-dev/workpo”):** #141414 fill, #A9A972 text, 16px/400, 8px radius, padding 12px.
- **button-ghost (“npm create convex@latest”):** #1A0F0F fill, #FFFFFF text, 16px/400, 4px radius, padding 4px 8px 4px 4px, border 1px solid #FFFFFF26.
- **link:** transparent fill, #141414 text, padding 0px.

## Do's and Don'ts

- Do use #281D1D for the page and lift surfaces in small steps: #292929, #141414, #1A0F0F, #38383A.
- Do keep text in 4 levels: #FFFFFF, #FAF4E9, #F6EEDB, #C2C2C2.
- Do let contrast carry emphasis; primary actions use #38383A on #281D1D.
- Do set headlines in neue-haas-grotesk-display with tight tracking (-0.04em).
- Do keep spacing on the 4px grid.
- Do use 4px corners on most elements; larger surfaces also use 8px and 6px.
- Don't introduce new font families beyond neue-haas-grotesk-display and gtAmerica.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/convex.dev/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
