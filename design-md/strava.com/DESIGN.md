---
version: alpha
name: Strava
description: "Light interface measured from strava.com: Boathouse type, vivid orange accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#21211F"
  on-surface-muted: "#43423F"
  surface-container-low: "#FAFAFA"
  surface-container: "#F9F8F5"
  outline: "#E0E0DE"
  primary: "#FC5200"
  on-primary: "#000000"
  inverse-surface: "#0D0C0C"
  secondary: "#0060D0"
  success: "#34A853"
  warning: "#FBBC05"
  error: "#EA4335"
typography:
  headline-display:
    fontFamily: Boathouse
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1
  body-md:
    fontFamily: Boathouse
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.29
  body-lg:
    fontFamily: Boathouse
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.33
  body-sm:
    fontFamily: Boathouse
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Boathouse
    fontSize: 16px
    fontWeight: 600
  label-sm:
    fontFamily: Boathouse
    fontSize: 15px
    fontWeight: 600
rounded:
  md: 4px
spacing:
  sm: 8px
  md: 12px
  lg: 20px
  xl: 50px
  gutter: 8px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 10px 50px
    height: 43px
  button-outline-hover:
    backgroundColor: "{colors.outline}"
  button-secondary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-sm}"
    rounded: 3.75px
    padding: 15px
    height: 54px
  button-tertiary:
    backgroundColor: "#050505"
    textColor: "{colors.background}"
    typography: "{typography.label-sm}"
    rounded: 3.75px
    padding: 15px
    height: 54px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Strava Design System

## Overview

Strava describes itself as: “Strava connects millions of runners, cyclists, hikers, walkers and other active people through the sports they love – all on our mobile app and website.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Orange (#FC5200)** as the main accent.

Type is set in **Boathouse**. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 4px.

Measured from [strava.com](https://www.strava.com/) on October 21, 2026 at 1440×900 and 390×844 from 111 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 7 times. Token `on-surface`, CSS `--color-extendedneutraln00`.
- **Charcoal (#21211F):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Graphite (#43423F):** Muted text and metadata, seen 21 times. Token `on-surface-muted`.
- **Snow (#FAFAFA):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Snow (#F9F8F5):** Cards and panels, seen 1 time. Token `surface-container`.
- **Silver (#E0E0DE):** Borders and dividers, seen 1 time. Token `outline`.
- **Vivid Orange (#FC5200):** Most used accent color, seen 9 times. Token `primary`, CSS `--color-coreo3`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#0D0C0C):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Blue (#0060D0):** Most used accent color, seen 3 times. Token `secondary`, CSS `--color-extendedblueb3`.
- **Green (#34A853):** Success and positive states, seen 1 time. Token `success`.
- **Vivid Amber (#FBBC05):** Warnings and highlights, seen 1 time. Token `warning`.
- **Vivid Red (#EA4335):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**Boathouse** carries the whole interface. Fallback stack: `Boathouse, Segoe UI, Helvetica Neue, -apple-system`.

- **headline-display:** Boathouse 32px at weight 600, line height 1. Page title (h1).
- **body-md:** Boathouse 14px at weight 400, line height 1.29. Body text.
- **body-lg:** Boathouse 15px at weight 400, line height 1.33. Lead paragraphs.
- **body-sm:** Boathouse 12px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Boathouse 16px at weight 600. Buttons, navigation and labels.
- **label-sm:** Boathouse 15px at weight 600. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 57% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 8px, md 12px, lg 20px, xl 50px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FAFAFA → #F9F8F5) and #E0E0DE borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 40 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Sign Up With Google”):** #FAFAFA fill, #21211F text, 16px/600, 4px radius, padding 10px 50px, border 1px solid #64635E.
- **button-outline-hover:** background #E0E0DE, text #21211F on hover.
- **button-secondary (“Accept All”):** #0D0C0C fill, #FFFFFF text, 15px/600, 3.75px radius, padding 15px, border 2px solid #FFFFFF.
- **button-tertiary (“Customize”):** #050505 fill, #FFFFFF text, 15px/600, 3.75px radius, padding 15px, border 2px solid #FFFFFF.
- **link:** transparent fill, #43423F text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAFAFA, #F9F8F5.
- Do keep text in 3 levels: #000000, #21211F, #43423F.
- Do reserve #FC5200 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 4px corners on most elements.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Boathouse.
- Don't use #FC5200 for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s, 0.1s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/strava.com/), the free DESIGN.md generator.
