---
version: alpha
name: Pinecone
description: "Light interface measured from pinecone.io: gtPlanar type, vivid indigo accents, tonal surfaces and square corners."
colors:
  background: "#FBFBFC"
  surface: "#FBFBFC"
  on-surface: "#1C1917"
  on-background: "#1C1917"
  on-surface-variant: "#57534E"
  on-surface-muted: "#A8A29E"
  surface-container-low: "#FFFFFF"
  outline: "#E7E5E4"
  primary: "#002BFF"
  on-primary: "#FFFFFF"
  secondary: "#3D11A0"
typography:
  headline-display:
    fontFamily: gtPlanar
    fontSize: 44px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: gtPlanar
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.2
  headline-md:
    fontFamily: gtPlanar
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.33
  headline-sm:
    fontFamily: gtPlanar
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.4
  body-md:
    fontFamily: gtPlanar
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: gtPlanar
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.3
  caption:
    fontFamily: gtPlanar
    fontSize: 12px
    fontWeight: 400
  label-lg:
    fontFamily: gtPlanar
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.4
  label-md:
    fontFamily: gtPlanar
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0.129em
  label-sm:
    fontFamily: gtPlanar
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0.033em
  code:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.5
  headline-lg-mobile:
    fontFamily: gtPlanar
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.2
rounded:
  none: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 20px
  xl: 40px
  gutter: 22px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.none}"
    padding: 8px 16px
    height: 39px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.code}"
    rounded: "{rounded.none}"
    padding: 8px 14px
    height: 38px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.none}"
    padding: 0px 14px
    height: 44px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.caption}"
    rounded: "{rounded.none}"
    padding: 0px 32px 0px 0px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.none}"
    padding: 10px 16px
  card:
    textColor: "#000000"
    typography: "{typography.body-md}"
    rounded: "{rounded.none}"
    padding: 0px
---

# Pinecone Design System

## Overview

Pinecone describes itself as: “Pinecone is the trusted AI knowledge company. Its AI knowledge platform—Database, Nexus, and Marketplace—powers accurate, fast, cost-effective AI for 10,000+ customers and 1M developers worldwide.” The interface is light, built on **Snow (#FBFBFC)** with **Charcoal (#1C1917)** text, and **Vivid Indigo (#002BFF)** as the main accent.

Type is set in **gtPlanar**, with **JetBrains Mono** for code. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are square.

Measured from [pinecone.io](https://www.pinecone.io/) on November 4, 2026 at 1440×900 and 390×844 from 311 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **Snow (#FBFBFC):** Page background, seen 9 times. Token `background`.
- **Charcoal (#1C1917):** Primary text and headings, seen 63 times. Token `on-surface`.
- **Warm Slate (#57534E):** Secondary text, seen 19 times. Token `on-surface-variant`, CSS `--color-text-secondary`.
- **Warm Gray (#A8A29E):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`, CSS `--osano-toggle-on-thumb-color`.
- **Mist (#E7E5E4):** Borders and dividers, seen 55 times. Token `outline`, CSS `--border`.
- **Vivid Indigo (#002BFF):** Primary buttons and calls to action, seen 20 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Violet (#3D11A0):** Accent (CSS variable). Token `secondary`.

## Typography

**gtPlanar** and **JetBrains Mono** (monospace) share the interface. Fallback stack: `gtPlanar, gtPlanar Fallback`.

- **headline-display:** gtPlanar 44px at weight 700, line height 1.1, tracking -0.02em. Page title (h1).
- **headline-lg:** gtPlanar 32px at weight 700, line height 1.2 (24px on mobile). Section headings (h2).
- **headline-md:** gtPlanar 24px at weight 700, line height 1.33. Sub-section headings.
- **headline-sm:** gtPlanar 20px at weight 700, line height 1.4. Card and feature titles.
- **body-md:** gtPlanar 16px at weight 400, line height 1.5. Body text.
- **body-sm:** gtPlanar 14px at weight 400, line height 1.3. Secondary and small text.
- **caption:** gtPlanar 12px at weight 400. Captions and fine print.
- **label-lg:** gtPlanar 16px at weight 500, line height 1.4. Large buttons and tabs.
- **label-md:** gtPlanar 14px at weight 500, line height 1.43, tracking 0.129em. Buttons, navigation and labels.
- **label-sm:** gtPlanar 12px at weight 500, line height 1, tracking 0.033em. Small labels and badges.
- **code:** JetBrains Mono 13px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing does not follow a strict grid: 68% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 10px, lg 20px, xl 40px.
- **Gaps:** 22px is the most common gap in flex and grid layouts.
- **Breakpoints:** 376px, 424px, 512px, 513px, 639px, 640px, 768px, 1024px, 1060px, 1080px, 1150px, 1175px, 1200px, 1280px, 1536px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF) and #E7E5E4 borders.

## Shapes

Corners are square. Measured radii, most used first:

- **none (0px):** measured.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for free”):** #002BFF fill, #FFFFFF text, 15px/400, padding 8px 16px, border 1px solid #002BFF.
- **button-secondary (“Claude Code”):** #1C1917 fill, #FBFBFC text, 13px/400, padding 8px 14px, border 1px solid #1C1917.
- **button-outline (“RAG pipeline”):** #FFFFFF fill, #1C1917 text, 16px/500, padding 0px 14px, border 1px solid #E7E5E4.
- **button-ghost (“Dismiss”):** transparent fill, #FFFFFF text, 12px/400, padding 0px 32px 0px 0px.
- **input-field (“Email Address”):** #FBFBFC fill, #1C1917 text, 15px/400, padding 10px 16px, border 1px solid #E7E5E4.
- **card:** transparent fill, #000000 text, 16px/400, padding 0px, border 1px solid #E7E5E4.

## Do's and Don'ts

- Do use #FBFBFC for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 3 levels: #1C1917, #57534E, #A8A29E.
- Do reserve #002BFF for primary actions and key highlights.
- Do set headlines in gtPlanar with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 10px, 20px).
- Don't use #A8A29E for body text; it reaches 2.44:1 on #FBFBFC. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond gtPlanar and JetBrains Mono.
- Don't use #002BFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.3s, 0.25s.

- **Easing:** `ease-out`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/pinecone.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
