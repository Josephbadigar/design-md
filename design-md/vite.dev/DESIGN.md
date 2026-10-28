---
version: alpha
name: Vite
description: "Dark interface measured from vite.dev: APK Protocol type with Inter, light blue accents, tonal surfaces and 8px corners."
colors:
  background: "#16171D"
  surface: "#16171D"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#BABABC"
  on-surface-muted: "#98989F"
  on-surface-subtle: "#867E8E"
  surface-container-low: "#14121A"
  outline: "#3B3440"
  outline-variant: "#2E2E32"
  primary: "#9AC8FF"
  on-primary: "#000000"
  secondary: "#B39AFF"
typography:
  headline-display:
    fontFamily: APK Protocol
    fontSize: 60px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: APK Protocol
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
  headline-md:
    fontFamily: APK Protocol
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.025em
  headline-sm:
    fontFamily: APK Protocol
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.17
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: APK Protocol
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
  code:
    fontFamily: KH Teka Mono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: 0.025em
  headline-display-mobile:
    fontFamily: APK Protocol
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.05em
  headline-lg-mobile:
    fontFamily: APK Protocol
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.025em
  headline-md-mobile:
    fontFamily: APK Protocol
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.025em
rounded:
  sm: 4px
  md: 8px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 40px
  gutter: 24px
  section: 112px
  margin: 40px
  container: 1440px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 38px
  button-secondary:
    backgroundColor: "#CCCCCC"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 11px
    padding: 8px 16px
    height: 38px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 8px 12px
  link:
    textColor: "{colors.on-surface}"
---

# Vite Design System

## Overview

Vite describes itself as: “Next Generation Frontend Tooling” The interface is dark, built on **Cool Charcoal (#16171D)** with **White (#FFFFFF)** text, and **Light Blue (#9AC8FF)** as the main accent.

Type is set in **APK Protocol** and **Inter**, with **KH Teka Mono** for code. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 8px.

Measured from [vite.dev](https://vite.dev/) on October 21, 2026 at 1440×900 and 390×844 from 228 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Cool Charcoal (#16171D):** Page background, seen 5 times. Token `background`, CSS `--vp-local-nav-bg-color`.
- **White (#FFFFFF):** Primary text and headings, seen 56 times. Token `on-surface`, CSS `--docsearch-sidepanel-hit-color`.
- **Silver (#BABABC):** Secondary text, seen 17 times. Token `on-surface-variant`.
- **Cool Gray (#98989F):** Muted text and metadata, seen 10 times. Token `on-surface-muted`, CSS `--vp-code-line-number-color`.
- **Cool Gray (#867E8E):** Subtle text and placeholders, seen 21 times. Token `on-surface-subtle`.
- **Cool Charcoal (#14121A):** Raised areas one step from the page, seen 10 times. Token `surface-container-low`, CSS `--docsearch-background-color`.
- **Cool Graphite (#3B3440):** Borders and dividers, seen 62 times. Token `outline`, CSS `--color-nickel`.
- **Graphite (#2E2E32):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Light Blue (#9AC8FF):** Brand accent (CSS variable). Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Light Violet (#B39AFF):** Most used accent color, seen 5 times. Token `secondary`, CSS `--vp-c-note-1`.

## Typography

**APK Protocol**, **Inter** and **KH Teka Mono** (monospace) share the interface. Fallback stack: `APK Protocol, sans-serif`.

- **headline-display:** APK Protocol 60px at weight 500, line height 1.12, tracking -0.05em (36px on mobile). Page title (h1).
- **headline-lg:** APK Protocol 48px at weight 500, line height 1, tracking -0.025em (30px on mobile). Section headings (h2).
- **headline-md:** APK Protocol 40px at weight 500, line height 1.33, tracking -0.025em (24px on mobile). Sub-section headings.
- **headline-sm:** APK Protocol 24px at weight 500, line height 1.17. Card and feature titles.
- **body-md:** Inter 16px at weight 400, line height 1.4. Body text.
- **body-lg:** Inter 18px at weight 400, line height 1.56. Lead paragraphs.
- **body-sm:** Inter 14px at weight 400, line height 1.43. Secondary and small text.
- **label-md:** APK Protocol 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500. Small labels and badges.
- **code:** KH Teka Mono 12px at weight 400, line height 1.33, tracking 0.025em, uppercase. Code and technical values.

## Layout

Spacing follows a 4px grid: 99% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 32px, xl 40px.
- **Sections:** 112px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 40px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#14121A) and #3B3440 borders.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 56 elements.
- **sm (4px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Search Ctrl K”):** #14121A fill, #98989F text, 14px/400, 8px radius, padding 8px 12px.
- **button-secondary (“Get Started”):** #CCCCCC fill, #FFFFFF text, 16px/500, 11px radius, padding 8px 16px.
- **button-ghost (“Resources”):** transparent fill, #FFFFFF text, 16px/400, padding 8px 12px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #16171D for the page and lift surfaces in small steps: #14121A.
- Do keep text in 4 levels: #FFFFFF, #BABABC, #98989F, #867E8E.
- Do use #9AC8FF as the brand accent: header, logo and key highlights.
- Do set headlines in APK Protocol with tight tracking (-0.05em).
- Do keep spacing on the 4px grid.
- Do use 8px corners on most elements; larger surfaces also use 4px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond APK Protocol, Inter and KH Teka Mono.
- Don't use #9AC8FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.001s.

## Motion

Interface transitions are quick: 0.001s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/vite.dev/), the free DESIGN.md generator.
