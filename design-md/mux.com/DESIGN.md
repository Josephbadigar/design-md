---
version: alpha
name: Mux
description: "Light interface measured from mux.com: Rotonto type with Aeonik, vivid orange accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#E2E4DD"
  surface: "#E2E4DD"
  on-surface: "#000000"
  on-background: "#000000"
  surface-container-low: "#D0D2C8"
  surface-container: "#FFFFFF"
  outline: "#D0D2C8"
  primary: "#FF6100"
  on-primary: "#000000"
  inverse-surface: "#242628"
  secondary: "#FA50B5"
  warning: "#FFB200"
typography:
  headline-display:
    fontFamily: Rotonto
    fontSize: 66px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: 0.02em
  headline-lg:
    fontFamily: Rotonto
    fontSize: 50px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: 0.02em
  headline-md:
    fontFamily: Aeonik
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.15
  headline-sm:
    fontFamily: Aeonik
    fontSize: 21px
    fontWeight: 700
    lineHeight: 1.15
  body-md:
    fontFamily: Aeonik
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: 0.02em
  body-sm:
    fontFamily: Aeonik
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.02em
  label-md:
    fontFamily: Aeonik
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  code:
    fontFamily: JetBrainsMono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.2
  headline-display-mobile:
    fontFamily: Rotonto
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: 0.02em
rounded:
  sm: 2px
  md: 28px
  lg: 112px
  full: 9999px
spacing:
  xs: 3.5px
  sm: 7px
  md: 14px
  lg: 28px
  xl: 56px
  gutter: 28px
  section: 64px
  margin: 84px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px
    height: 56px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.surface-container}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px
    height: 85px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 14px 28px
    height: 42px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.surface-container}"
---

# Mux Design System

## Overview

Mux describes itself as: “Mux helps teams ship high-performance and cost-effective video in minutes, not months. Build better video into anything from websites to platforms to AI workflows.” The interface is light, built on **Mist (#E2E4DD)** with **Near Black (#000000)** text, and **Vivid Orange (#FF6100)** as the main accent.

Type is set in **Rotonto** and **Aeonik**, with **JetBrainsMono** for code. Headlines run large; body text is 18px. The surface language is flat. Controls are pill-shaped.

Measured from [mux.com](https://www.mux.com/) on November 4, 2026 at 1440×900 and 390×844 from 436 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Mist (#E2E4DD):** Page background, seen 11 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 32 times. Token `on-surface`.
- **Silver (#D0D2C8):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **White (#FFFFFF):** Cards and panels, seen 3 times. Token `surface-container`, CSS `--tw-ring-offset-color`.
- **Silver (#D0D2C8):** Borders and dividers, seen 3 times. Token `outline`.
- **Vivid Orange (#FF6100):** Primary buttons and calls to action, seen 13 times. Token `primary`, CSS `--color-orange`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Graphite (#242628):** High-contrast fills, seen 8 times. Token `inverse-surface`.
- **Pink (#FA50B5):** Accent in text, fills and borders, seen 4 times. Token `secondary`.
- **Vivid Amber (#FFB200):** Warnings and highlights, seen 46 times. Token `warning`.

## Typography

**Rotonto**, **Aeonik** and **JetBrainsMono** (monospace) share the interface. Fallback stack: `Rotonto, Rotonto Fallback, Helvetica, sans-serif`.

- **headline-display:** Rotonto 66px at weight 400, line height 1.15, tracking 0.02em, uppercase (32px on mobile). Page title (h1).
- **headline-lg:** Rotonto 50px at weight 400, line height 1.15, tracking 0.02em. Section headings (h2).
- **headline-md:** Aeonik 24px at weight 700, line height 1.15. Sub-section headings.
- **headline-sm:** Aeonik 21px at weight 700, line height 1.15. Card and feature titles.
- **body-md:** Aeonik 18px at weight 700, line height 1.5, tracking 0.02em. Body text.
- **body-sm:** Aeonik 14px at weight 400, line height 1.5, tracking 0.02em. Secondary and small text.
- **label-md:** Aeonik 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **code:** JetBrainsMono 14px at weight 400, line height 1.2. Code and technical values.

## Layout

Spacing does not follow a strict grid: 59% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.5px, sm 7px, md 14px, lg 28px, xl 56px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 28px is the most common gap in flex and grid layouts.
- **Page margin:** 84px on each side of full-width sections.
- **Breakpoints:** 352px, 440px, 504px, 576px, 768px, 783px, 784px, 1024px, 1176px, 1320px, 1456px, 1920px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#D0D2C8 → #FFFFFF) and #D0D2C8 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (28px):** 48 elements.
- **full (9999px):** 32 elements.
- **sm (2px):** 28 elements.
- **lg (112px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“READ OUR DOCS READ OUR DOCS”):** #FF6100 fill, #000000 text, 16px/400, 112px radius, padding 0px.
- **button-secondary (“LOG IN LOG IN”):** #000000 fill, #FFFFFF text, 14px/400, padding 0px.
- **button-outline (“TRY ANOTHER VIDEO CARET”):** #E2E4DD fill, #000000 text, 14px/400, padding 14px 28px, border 1px solid #D0D2C8.
- **button-ghost (“Toggle Mux Brand Popover”):** transparent fill, #000000 text, 16px/400, padding 0px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #E2E4DD for the page and lift surfaces in small steps: #D0D2C8, #FFFFFF.
- Do reserve #FF6100 for primary actions and key highlights.
- Do reuse the measured spacing steps (7px, 14px, 28px).
- Do make buttons and chips fully rounded (9999px); most other elements use 28px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Rotonto, Aeonik and JetBrainsMono.
- Don't use #FF6100 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.12s, 0.24s, 0.3s, 0.2s. Longer ambient animations run 2s.

- **Easing:** `cubic-bezier(0.7, 0, 0.3, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mux.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
