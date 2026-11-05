---
version: alpha
name: Muzli
description: "Light interface measured from muz.li: Instrument Serif type with Poppins, vivid indigo accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#303030"
  on-surface-muted: "#404565"
  overlay: "#2E54FF1A"
  primary: "#2E54FF"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: Instrument Serif
    fontSize: 85px
    fontWeight: 400
    lineHeight: 1.38
  headline-lg:
    fontFamily: Poppins
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.38
  headline-md:
    fontFamily: Instrument Serif
    fontSize: 30.5px
    fontWeight: 400
    lineHeight: 1.3
  headline-sm:
    fontFamily: Poppins
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.5
  body-md:
    fontFamily: Poppins
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Poppins
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Instrument Serif
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.38
  headline-lg-mobile:
    fontFamily: Poppins
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.33
rounded:
  md: 70px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 28px
  xl: 40px
  gutter: 40px
  section: 100px
  margin: 28px
  container: 1280px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 8px 20px
    height: 36px
  button-primary-hover:
    backgroundColor: "#2C4DE2"
  link:
    textColor: "{colors.on-surface-muted}"
---

# Muzli Design System

## Overview

Muzli describes itself as: “Designers' Secret Source: all the design inspiration from the world in one place. Served fresh.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Indigo (#2E54FF)** as the main accent.

Type is set in **Instrument Serif** and **Poppins**. Headlines run large; body text is 14px. The surface language is flat. Controls are pill-shaped.

Measured from [muz.li](https://muz.li/) on November 4, 2026 at 1440×900 and 390×844 from 173 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles, plus gradient stops #DA47F9, #946BFE.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`, CSS `--cc-bg`.
- **Near Black (#000000):** Primary text and headings, seen 22 times. Token `on-surface`.
- **Graphite (#303030):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Dark Indigo (#404565):** Muted text and metadata, seen 34 times. Token `on-surface-muted`.
- **Vivid Indigo 10% (#2E54FF1A):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Vivid Indigo (#2E54FF):** Primary buttons and calls to action, seen 26 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**Instrument Serif** and **Poppins** share the interface. Fallback stack: `Instrument Serif, Georgia`. Other loaded fonts: icomoon.

- **headline-display:** Instrument Serif 85px at weight 400, line height 1.38 (48px on mobile). Page title (h1).
- **headline-lg:** Poppins 48px at weight 400, line height 1.38 (24px on mobile). Section headings (h2).
- **headline-md:** Instrument Serif 30.5px at weight 400, line height 1.3. Sub-section headings.
- **headline-sm:** Poppins 20px at weight 500, line height 1.5. Card and feature titles.
- **body-md:** Poppins 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Poppins 16px at weight 400, line height 1.5. Lead paragraphs.

## Layout

Spacing follows a 4px grid: 91% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 28px, xl 40px.
- **Sections:** 100px vertical padding between major sections.
- **Gaps:** 40px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1280px.
- **Page margin:** 28px on each side of full-width sections.
- **Breakpoints:** 420px, 480px, 640px, 760px, 767px, 768px, 769px, 900px, 1023px, 1024px, 1280px, 1536px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 20 elements.
- **md (70px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Muzli”):** #2E54FF fill, #FFFFFF text, 14px/400, 9999px radius, padding 8px 20px.
- **button-primary-hover:** background #2C4DE2, text #FFFFFF on hover.
- **link:** transparent fill, #404565 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #000000, #303030, #404565.
- Do reserve #2E54FF for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 70px corners.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Instrument Serif and Poppins.
- Don't use #2E54FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.25s, 0.15s, 0.3s, 0.2s. Longer ambient animations run 2s.

- **Easing:** `ease`, `ease-in`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/muz.li/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
