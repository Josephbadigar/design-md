---
version: alpha
name: Sanity
description: "Dark interface measured from sanity.io: Waldenburg type, vivid orange accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#0B0B0B"
  surface: "#0B0B0B"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#E1E4E8"
  on-surface-muted: "#B9B9B9"
  on-surface-subtle: "#797979"
  surface-container-low: "#212121"
  outline: "#212121"
  outline-variant: "#353535"
  primary: "#FF4100"
  on-primary: "#0B0B0B"
  secondary: "#9ECBFF"
  tertiary: "#AFE3FF"
typography:
  headline-display:
    fontFamily: Waldenburg
    fontSize: 112px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Waldenburg
    fontSize: 72px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.04em
  headline-md:
    fontFamily: Waldenburg
    fontSize: 60px
    fontWeight: 400
    lineHeight: 0.8
  headline-sm:
    fontFamily: Waldenburg
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.07
    letterSpacing: -0.035em
  title-lg:
    fontFamily: Waldenburg
    fontSize: 38px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.03em
  body-md:
    fontFamily: Waldenburg
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Waldenburg
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.01em
  body-sm:
    fontFamily: Waldenburg
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.3
  label-md:
    fontFamily: Waldenburg
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.5
  code:
    fontFamily: IBM Plex Mono
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.3
  headline-display-mobile:
    fontFamily: Waldenburg
    fontSize: 60px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.04em
  headline-lg-mobile:
    fontFamily: Waldenburg
    fontSize: 50px
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: -0.04em
rounded:
  sm: 3px
  md: 5px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24.16px
  xl: 48px
  gutter: 12px
  section: 128px
  margin: 24px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 4px 12px
    height: 35px
  button-primary-hover:
    backgroundColor: "{colors.background}"
    textColor: "{colors.primary}"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.full}"
    padding: 8px 32px
    height: 55px
  button-secondary-hover:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: 6px
    padding: 12px
    height: 51px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 4px 12px
  input-field:
    textColor: "{colors.on-surface-muted}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
  link:
    textColor: "{colors.on-surface}"
---

# Sanity Design System

## Overview

Sanity describes itself as: “Sanity is the back-end built for AI content operations. Power web, mobile, and agentic applications at scale.” The interface is dark, built on **Near Black (#0B0B0B)** with **White (#FFFFFF)** text, and **Vivid Orange (#FF4100)** as the main accent.

Type is set in **Waldenburg**, with **IBM Plex Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [sanity.io](https://www.sanity.io/) on November 4, 2026 at 1440×900 and 390×844 from 419 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Near Black (#0B0B0B):** Page background, seen 11 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 69 times. Token `on-surface`, CSS `--osano-toggle-on-thumb-color`.
- **Cool Mist (#E1E4E8):** Secondary text, seen 29 times. Token `on-surface-variant`.
- **Silver (#B9B9B9):** Muted text and metadata, seen 8 times. Token `on-surface-muted`, CSS `--color-gray-300`.
- **Slate (#797979):** Subtle text and placeholders, seen 6 times. Token `on-surface-subtle`, CSS `--color-gray-500`.
- **Charcoal (#212121):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **Charcoal (#212121):** Borders and dividers, seen 6 times. Token `outline`.
- **Graphite (#353535):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Orange (#FF4100):** Primary buttons and calls to action, seen 9 times. Token `primary`.
- **Near Black (#0B0B0B):** Text and icons on primary. Token `on-primary`.
- **Light Blue (#9ECBFF):** Accent in text, fills and borders, seen 10 times. Token `secondary`.
- **Light Blue (#AFE3FF):** Accent (CSS variable). Token `tertiary`.

## Typography

**Waldenburg** and **IBM Plex Mono** (monospace) share the interface. Fallback stack: `Waldenburg-75357948a2b6a39b, Waldenburg-75357948a2b6a39b fallback: Arial, ui-sans-serif, system-ui`. Other loaded fonts: Waldenburg-75357948a2b6a39b, IBM Plex Mono-c20ba633a65a8c57.

- **headline-display:** Waldenburg 112px at weight 400, line height 1, tracking -0.04em (60px on mobile). Page title (h1).
- **headline-lg:** Waldenburg 72px at weight 400, line height 1, tracking -0.04em (50px on mobile). Section headings (h2).
- **headline-md:** Waldenburg 60px at weight 400, line height 0.8. Sub-section headings.
- **headline-sm:** Waldenburg 48px at weight 400, line height 1.07, tracking -0.035em. Card and feature titles.
- **title-lg:** Waldenburg 38px at weight 400, line height 1.1, tracking -0.03em. Small titles.
- **body-md:** Waldenburg 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Waldenburg 18px at weight 400, line height 1.3, tracking -0.01em. Lead paragraphs.
- **body-sm:** Waldenburg 13px at weight 400, line height 1.3. Secondary and small text.
- **label-md:** Waldenburg 13px at weight 500, line height 1.5. Buttons, navigation and labels.
- **code:** IBM Plex Mono 13px at weight 400, line height 1.3, uppercase. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (76% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24.16px, xl 48px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 376px, 480px, 768px, 1000px, 1200px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#212121) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(0, 82, 239) 0px 0px 0px 1px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 120 elements.
- **md (5px):** 32 elements.
- **sm (3px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“GET STARTED”):** #FF4100 fill, #0B0B0B text, 13px/400, 99999px radius, padding 4px 12px, border 1px solid #FF4100.
- **button-primary-hover:** background #0B0B0B, text #FF4100 on hover.
- **button-secondary (“Watch demo”):** #FFFFFF fill, #0B0B0B text, 24px/400, 99999px radius, padding 8px 32px, border 1px solid #FFFFFF.
- **button-secondary-hover:** background #0B0B0B, text #FFFFFF on hover.
- **button-outline (“KG Published”):** #212121 fill, #0B0B0B text, 16px/400, 6px radius, padding 12px.
- **button-ghost (“PRODUCTS”):** transparent fill, #FFFFFF text, 13px/400, 99999px radius, padding 4px 12px.
- **input-field (“Title”):** transparent fill, #B9B9B9 text, 15px/400, 3px radius, padding 0px 12px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #0B0B0B for the page and lift surfaces in small steps: #212121.
- Do keep text in 4 levels: #FFFFFF, #E1E4E8, #B9B9B9, #797979.
- Do reserve #FF4100 for primary actions and key highlights.
- Do set headlines in Waldenburg with tight tracking (-0.04em).
- Do reuse the measured spacing steps (8px, 12px, 24.16px).
- Do make buttons and chips fully rounded (9999px); most other elements use 5px corners.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Waldenburg and IBM Plex Mono.
- Don't use #FF4100 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.5s, 0.3s, 0.2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/sanity.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
