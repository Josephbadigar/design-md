---
version: alpha
name: Modern Treasury
description: "Light interface measured from moderntreasury.com: mt-neue-display type with mt-neue-text, dark teal accents, tonal surfaces and 2px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#151515"
  on-background: "#151515"
  on-surface-variant: "#444444"
  on-surface-muted: "#2A5060"
  on-surface-subtle: "#215B4B"
  surface-container-low: "#FFFFFFE6"
  surface-container: "#F8F7F5"
  overlay: "#15151521"
  overlay-strong: "#29735C80"
  outline: "#15151533"
  outline-variant: "#FFFFFF33"
  primary: "#29735C"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: mt-neue-display
    fontSize: 71px
    fontWeight: 450
    lineHeight: 1.1
  headline-lg:
    fontFamily: mt-neue-display
    fontSize: 47px
    fontWeight: 450
    lineHeight: 1.25
  headline-md:
    fontFamily: mt-neue-text
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.25
  headline-sm:
    fontFamily: mt-neue-text
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1.3
  body-md:
    fontFamily: mt-sans
    fontSize: 14px
    fontWeight: 330
    lineHeight: 1.5
  body-lg:
    fontFamily: mt-sans
    fontSize: 16px
    fontWeight: 360
    lineHeight: 1.5
  label-md:
    fontFamily: mt-sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: mt-sans
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.5
  code:
    fontFamily: mt-mono
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.04em
  headline-display-mobile:
    fontFamily: mt-neue-display
    fontSize: 47px
    fontWeight: 450
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: mt-neue-display
    fontSize: 32px
    fontWeight: 450
    lineHeight: 1.25
  headline-md-mobile:
    fontFamily: mt-neue-text
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.25
rounded:
  sm: 2px
  md: 4px
  lg: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 16px
  section: 60px
  margin: 48px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 6px 12px
    height: 33px
  button-ghost:
    textColor: "#000000"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 4px 8px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 8px 12px
  card:
    backgroundColor: "{colors.background}"
    textColor: "#000000"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Modern Treasury Design System

## Overview

Modern Treasury describes itself as: “A payment service provider (PSP) for fiat and stablecoin. Launch in days with one API, sub-accounts, and built-in compliance across ACH, RTP, FedNow, and wire.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#151515)** text, and **Dark Teal (#29735C)** as the main accent.

Type is set in **mt-neue-display** and **mt-neue-text**, with **mt-mono** for code. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 2px.

Measured from [moderntreasury.com](https://www.moderntreasury.com/) on November 4, 2026 at 1440×900 and 390×844 from 294 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 13 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Charcoal (#151515):** Primary text and headings, seen 36 times. Token `on-surface`, CSS `--color-button-secondary-text`.
- **Graphite (#444444):** Secondary text, seen 16 times. Token `on-surface-variant`.
- **Dark Cyan (#2A5060):** Muted text and metadata, seen 15 times. Token `on-surface-muted`.
- **Dark Teal (#215B4B):** Subtle text and placeholders, seen 14 times. Token `on-surface-subtle`.
- **White 90% (#FFFFFFE6):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#F8F7F5):** Cards and panels, seen 4 times. Token `surface-container`.
- **Charcoal 13% (#15151521):** Translucent fill for cards and controls, seen 1 time. Token `overlay`, CSS `--color-alpha-black-100`.
- **Dark Teal 50% (#29735C80):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Charcoal 20% (#15151533):** Borders and dividers, seen 3 times. Token `outline`.
- **White 20% (#FFFFFF33):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Dark Teal (#29735C):** Brand color in the logo, seen 23 times. Token `primary`, CSS `--color-mt-logo`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**mt-neue-display**, **mt-neue-text**, **mt-sans** and **mt-mono** (monospace) share the interface. Fallback stack: `mt-neue-display, ui-sans-serif, system-ui, sans-serif`.

- **headline-display:** mt-neue-display 71px at weight 450, line height 1.1 (47px on mobile). Page title (h1).
- **headline-lg:** mt-neue-display 47px at weight 450, line height 1.25 (32px on mobile). Section headings (h2).
- **headline-md:** mt-neue-text 32px at weight 400, line height 1.25 (26px on mobile). Sub-section headings.
- **headline-sm:** mt-neue-text 21px at weight 400, line height 1.3. Card and feature titles.
- **body-md:** mt-sans 14px at weight 330, line height 1.5. Body text.
- **body-lg:** mt-sans 16px at weight 360, line height 1.5. Lead paragraphs.
- **label-md:** mt-sans 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** mt-sans 14px at weight 600, line height 1.5. Small labels and badges.
- **code:** mt-mono 10px at weight 400, line height 1.5, tracking 0.04em. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (85% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Page margin:** 48px on each side of full-width sections.
- **Breakpoints:** 375px, 600px, 900px, 1024px, 1200px, 1300px, 1440px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#FFFFFFE6 → #F8F7F5):

- `rgb(21, 21, 21) 0px 0px 0px 1px inset`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, lab(0 0 0 / 0.04) 0px 20px 25px -5px, lab(0 0 0 / 0.04) 0px 8px 10px -6px`.

## Shapes

Most elements use 2px corners. Measured radii, most used first:

- **sm (2px):** 68 elements.
- **md (4px):** 24 elements.
- **lg (8px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Talk to us”):** #151515 fill, #FFFFFF text, 14px/600, 2px radius, padding 6px 12px, shadow `rgb(21, 21, 21) 0px 0px 0px 1px inset`.
- **button-ghost (“Products”):** transparent fill, #000000 text, 14px/500, 4px radius, padding 4px 8px.
- **input-field:** #FFFFFF fill, #151515 text, 16px/500, padding 8px 12px.
- **card:** #FFFFFF fill, #000000 text, 16px/400, padding 0px.
- **link:** transparent fill, #151515 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FFFFFFE6, #F8F7F5.
- Do keep text in 4 levels: #151515, #444444, #2A5060, #215B4B.
- Do use #29735C as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 2px corners on most elements; larger surfaces also use 4px and 8px.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond mt-neue-display, mt-neue-text, mt-sans and mt-mono.
- Don't use #29735C for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.3s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/moderntreasury.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
