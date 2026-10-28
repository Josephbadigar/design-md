---
version: alpha
name: Svelte
description: "Dark interface measured from svelte.dev: DM Serif Display type with Fira Sans, vivid red accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#1C1E22"
  surface: "#1C1E22"
  on-surface: "#CACBCE"
  on-background: "#CACBCE"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#E5E5E6"
  surface-container-low: "#23272F"
  surface-container: "#2E333E"
  outline: "#303541"
  outline-variant: "#23272F"
  primary: "#F96743"
  on-primary: "#000000"
  inverse-surface: "#A1A4AA"
  secondary: "#B32D00"
typography:
  headline-display:
    fontFamily: DM Serif Display
    fontSize: 54px
    fontWeight: 500
    lineHeight: 1.2
  body-md:
    fontFamily: Fira Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Georgia
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Georgia
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Fira Sans
    fontSize: 10px
    fontWeight: 400
  headline-display-mobile:
    fontFamily: DM Serif Display
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
rounded:
  md: 4px
  full: 9999px
spacing:
  xs: 3.25px
  sm: 8px
  md: 10px
  lg: 18px
  xl: 48px
  gutter: 10px
  section: 100px
components:
  input-field:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-strong}"
    rounded: 56px
    padding: 7px 7px 5.6px 28px
  link:
    textColor: "{colors.primary}"
---

# Svelte Design System

## Overview

Svelte describes itself as: “Web development for the rest of us” The interface is dark, built on **Cool Charcoal (#1C1E22)** with **Silver (#CACBCE)** text, and **Vivid Red (#F96743)** as the main accent.

Type is set in **DM Serif Display** and **Fira Sans**. Headlines run large; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [svelte.dev](https://svelte.dev/) on October 21, 2026 at 1440×900 and 390×844 from 137 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Cool Charcoal (#1C1E22):** Page background, seen 2 times. Token `background`, CSS `--sk-bg-1`.
- **Silver (#CACBCE):** Primary text and headings, seen 12 times. Token `on-surface`, CSS `--sk-fg-2`.
- **White (#FFFFFF):** Headings and emphasis, seen 5 times. Token `on-surface-strong`.
- **Mist (#E5E5E6):** Secondary text, seen 4 times. Token `on-surface-variant`, CSS `--sk-fg-1`.
- **Cool Graphite (#23272F):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--sk-bg-3`.
- **Cool Graphite (#2E333E):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--sk-bg-4`.
- **Cool Graphite (#303541):** Borders and dividers, seen 2 times. Token `outline`, CSS `--sk-border`.
- **Cool Graphite (#23272F):** Secondary dividers, seen 2 times. Token `outline-variant`, CSS `--sk-bg-3`.
- **Vivid Red (#F96743):** Brand accent (CSS variable), seen 85 times. Token `primary`, CSS `--sk-fg-accent`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Cool Gray (#A1A4AA):** High-contrast fills, seen 5 times. Token `inverse-surface`, CSS `--sk-fg-3`.
- **Dark Orange (#B32D00):** Brand color on large areas, seen 32 times. Token `secondary`.

## Typography

**DM Serif Display**, **Fira Sans** and **Georgia** share the interface. Fallback stack: `DM Serif Display, Georgia, serif`.

- **headline-display:** DM Serif Display 54px at weight 500, line height 1.2 (30px on mobile). Page title (h1).
- **body-md:** Fira Sans 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Georgia 18px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** Georgia 10px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Fira Sans 10px at weight 400. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 46% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.25px, sm 8px, md 10px, lg 18px, xl 48px.
- **Sections:** 100px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#23272F → #2E333E) and #303541 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 320 elements.
- **md (4px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **input-field (“Search”):** #2E333E fill, #FFFFFF text, 14px/400, 56px radius, padding 7px 7px 5.6px 28px.
- **link:** transparent fill, #F96743 text, padding 0px.

## Do's and Don'ts

- Do use #1C1E22 for the page and lift surfaces in small steps: #23272F, #2E333E.
- Do keep text in 3 levels: #CACBCE, #FFFFFF, #E5E5E6.
- Do use #F96743 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 10px, 18px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond DM Serif Display, Fira Sans and Georgia.
- Don't use #F96743 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/svelte.dev/), the free DESIGN.md generator.
