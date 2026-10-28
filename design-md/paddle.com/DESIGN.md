---
version: alpha
name: Paddle
description: "Light interface measured from paddle.com: serrifCondensed type with Inter, vivid amber accents, tonal surfaces and 16px corners."
colors:
  background: "#F9F8F7"
  surface: "#F9F8F7"
  on-surface: "#1C1A15"
  on-background: "#1C1A15"
  surface-container-low: "#FCFCFC"
  surface-container: "#E8E6E2"
  surface-container-high: "#E4E1D1"
  outline: "#D9D3C9"
  primary: "#FFD400"
  on-primary: "#000000"
typography:
  headline-display:
    fontFamily: serrifCondensed
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: serrifCondensed
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  headline-md:
    fontFamily: serrifCondensed
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: serrifCondensed
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.02em
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.029em
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.025em
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0.03em
  code:
    fontFamily: ui-monospace
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.029em
  headline-display-mobile:
    fontFamily: serrifCondensed
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: serrifCondensed
    fontSize: 37px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  headline-md-mobile:
    fontFamily: serrifCondensed
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
rounded:
  xs: 3px
  sm: 6.4px
  md: 10px
  lg: 16px
  xl: 24px
spacing:
  base: 4px
  xs: 3.52px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 40px
  gutter: 16px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 16px 20px
    height: 52px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 16px 20px
    height: 52px
  button-outline-hover:
    backgroundColor: "#E5E2D3"
  button-ghost:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px
    height: 52px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 40px
  link:
    textColor: "{colors.on-surface}"
---

# Paddle Design System

## Overview

Paddle describes itself as: “Increase revenue, reduce risk and reduce cost with Paddle, the payment solution powering global revenue for n8n, Letterboxd & AdGuard. One platform that handles billing, tax and compliance.” The interface is light, built on **Snow (#F9F8F7)** with **Warm Charcoal (#1C1A15)** text, and **Vivid Amber (#FFD400)** as the main accent.

Type is set in **serrifCondensed** and **Inter**, with **ui-monospace** for code. Headlines run large with tight negative tracking; body text is 20px. The surface language is flat. Corners are mostly 16px.

Measured from [paddle.com](https://www.paddle.com/) on October 21, 2026 at 1440×900 and 390×844 from 253 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Snow (#F9F8F7):** Page background, seen 2 times. Token `background`.
- **Warm Charcoal (#1C1A15):** Primary text and headings, seen 62 times. Token `on-surface`, CSS `--th-color-heading`.
- **Snow (#FCFCFC):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`.
- **Warm Mist (#E8E6E2):** Cards and panels, seen 6 times. Token `surface-container`.
- **Light Amber (#E4E1D1):** Hover and pressed fills, seen 4 times. Token `surface-container-high`.
- **Warm Silver (#D9D3C9):** Borders and dividers, seen 3 times. Token `outline`.
- **Vivid Amber (#FFD400):** Brand accent (CSS variable), seen 8 times. Token `primary`, CSS `--color-primary-yellow`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.

## Typography

**serrifCondensed**, **Inter** and **ui-monospace** (monospace) share the interface. Fallback stack: `serrifCondensed, serrifCondensed Fallback, Helvetica Neue, Helvetica`. Other loaded fonts: Inter Fallback, serrifCondensed Fallback.

- **headline-display:** serrifCondensed 64px at weight 400, line height 1, tracking -0.01em (56px on mobile). Page title (h1).
- **headline-lg:** serrifCondensed 48px at weight 400, line height 1.2, tracking -0.01em (37px on mobile). Section headings (h2).
- **headline-md:** serrifCondensed 40px at weight 400, line height 1.2, tracking -0.01em (21px on mobile). Sub-section headings.
- **headline-sm:** serrifCondensed 24px at weight 400, line height 1.2, tracking -0.01em. Card and feature titles.
- **body-md:** Inter 20px at weight 400, line height 1.5, tracking -0.02em. Body text.
- **body-sm:** Inter 14px at weight 400, line height 1.5, tracking -0.029em. Secondary and small text.
- **label-md:** Inter 16px at weight 500, line height 1.5, tracking -0.025em. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1, tracking 0.03em. Small labels and badges.
- **code:** ui-monospace 14px at weight 400, line height 1.5, tracking -0.029em. Code and technical values.

## Layout

Spacing follows a 4px grid: 92% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 3.52px, sm 8px, md 16px, lg 20px, xl 40px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 428px, 640px, 641px, 843px, 1023px, 1024px, 1439px, 1440px, 1920px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FCFCFC → #E8E6E2 → #E4E1D1) and #D9D3C9 borders.

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **lg (16px):** 56 elements.
- **md (10px):** 44 elements.
- **sm (6.4px):** 14 elements.
- **xs (3px):** 12 elements.
- **xl (24px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Book a demo”):** #1C1A15 fill, #FCFCFC text, 16px/500, 10px radius, padding 16px 20px.
- **button-outline (“Discover Billing”):** #FCFCFC fill, #1C1A15 text, 16px/500, 10px radius, padding 16px 20px.
- **button-outline-hover:** background #E5E2D3, text #1C1A15 on hover.
- **button-ghost (“Get started”):** #E4E1D1 fill, #1C1A15 text, 16px/500, 10px radius, padding 0px.
- **card:** #FCFCFC fill, #1C1A15 text, 20px/400, 24px radius, padding 40px.
- **link:** transparent fill, #1C1A15 text, padding 0px.

## Do's and Don'ts

- Do use #F9F8F7 for the page and lift surfaces in small steps: #FCFCFC, #E8E6E2, #E4E1D1.
- Do use #FFD400 as the brand accent: header, logo and key highlights.
- Do set headlines in serrifCondensed with tight tracking (-0.01em).
- Do keep spacing on the 4px grid.
- Do use 16px corners on most elements; larger surfaces also use 10px, 6.4px and 3px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond serrifCondensed, Inter and ui-monospace.
- Don't use #FFD400 for large backgrounds or body text.
- Don't make interface transitions slower than 0.32s.

## Motion

Interface transitions are quick: 0.2s, 0.24s, 0.32s, 0.3s. Longer ambient animations run 0.8s.

- **Easing:** `cubic-bezier(0.246, 0.75, 0.187, 1)`, `ease-out`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/paddle.com/), the free DESIGN.md generator.
