---
version: alpha
name: Go
description: "Dark interface measured from go.dev: system-ui type with Roboto, dark cyan accents, tonal surfaces and 4px corners."
colors:
  background: "#202224"
  surface: "#202224"
  on-surface: "#F0F1F2"
  on-background: "#F0F1F2"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#AAACAE"
  surface-container-low: "#2D2D2D"
  surface-container: "#253443"
  overlay: "#007D9CBF"
  primary: "#007D9C"
  on-primary: "#FFFFFF"
  inverse-surface: "#F8F8F8E6"
  secondary: "#08667E"
  tertiary: "#50B7E0"
  warning: "#FDDD00"
typography:
  headline-display:
    fontFamily: system-ui
    fontSize: 39px
    fontWeight: 500
    lineHeight: 1.4
  headline-lg:
    fontFamily: system-ui
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.17
  headline-md:
    fontFamily: system-ui
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.17
  headline-sm:
    fontFamily: system-ui
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.4
  title-lg:
    fontFamily: system-ui
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1.71
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  body-lg:
    fontFamily: system-ui
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
  caption:
    fontFamily: system-ui
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.18
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.4
  label-sm:
    fontFamily: Roboto
    fontSize: 14px
    fontWeight: 700
  code:
    fontFamily: Menlo
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
  headline-display-mobile:
    fontFamily: system-ui
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.4
  headline-lg-mobile:
    fontFamily: system-ui
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.4
  headline-md-mobile:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
rounded:
  sm: 2px
  md: 4px
  full: 9999px
spacing:
  xs: 3.01px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 60px
  gutter: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 8px
    height: 40px
  button-secondary:
    backgroundColor: "{colors.warning}"
    textColor: "#000000"
    typography: "{typography.headline-md}"
    rounded: "{rounded.md}"
    padding: 16px 0px
    height: 64px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.tertiary}"
    typography: "{typography.label-sm}"
    rounded: 3px
    padding: 0px 10px
    height: 28px
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.headline-md}"
    rounded: "{rounded.md}"
    padding: 16px 0px
  input-field:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px 10px
  link:
    textColor: "{colors.tertiary}"
---

# Go Design System

## Overview

Go describes itself as: “Go is an open source programming language that makes it simple to build secure, scalable systems.” The interface is dark, built on **Charcoal (#202224)** with **Mist (#F0F1F2)** text, and **Dark Cyan (#007D9C)** as the main accent.

Type is set in **system-ui** and **Roboto**, with **Menlo** for code. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [go.dev](https://go.dev/) on October 21, 2026 at 1440×900 and 390×844 from 265 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Charcoal (#202224):** Page background, seen 6 times. Token `background`, CSS `--color-button-inverted-disabled`.
- **Mist (#F0F1F2):** Primary text and headings, seen 42 times. Token `on-surface`, CSS `--color-input-text`.
- **White (#FFFFFF):** Headings and emphasis, seen 20 times. Token `on-surface-strong`, CSS `--white`.
- **Gray (#AAACAE):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Graphite (#2D2D2D):** Raised areas one step from the page, seen 23 times. Token `surface-container-low`, CSS `--color-background-highlighted`.
- **Deep Blue (#253443):** Cards and panels, seen 2 times. Token `surface-container`, CSS `--slate`.
- **Dark Cyan 75% (#007D9CBF):** Translucent fill for cards and controls, seen 1 time. Token `overlay`, CSS `--color-background-banner`.
- **Dark Cyan (#007D9C):** Brand color in the header, seen 3 times. Token `primary`, CSS `--color-brand-primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Snow 90% (#F8F8F8E6):** High-contrast fills, seen 19 times. Token `inverse-surface`, CSS `--color-background-banner-secondary`.
- **Dark Cyan (#08667E):** Brand color in logos and imagery, seen 69 times. Token `secondary`.
- **Cyan (#50B7E0):** Links and interactive text, seen 33 times. Token `tertiary`, CSS `--color-text-link`.
- **Vivid Yellow (#FDDD00):** Warnings and highlights, seen 2 times. Token `warning`, CSS `--yellow`.

## Typography

**system-ui**, **Roboto** and **Menlo** (monospace) share the interface. Fallback stack: `-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica`. Other loaded fonts: Material Icons.

- **headline-display:** system-ui 39px at weight 500, line height 1.4 (22px on mobile). Page title (h1).
- **headline-lg:** system-ui 36px at weight 500, line height 1.17 (20px on mobile). Section headings (h2).
- **headline-md:** system-ui 24px at weight 400, line height 1.17 (14px on mobile). Sub-section headings.
- **headline-sm:** system-ui 22px at weight 400, line height 1.4. Card and feature titles.
- **title-lg:** system-ui 21px at weight 400, line height 1.71. Small titles.
- **body-md:** system-ui 16px at weight 400, line height 1.4. Body text.
- **body-lg:** system-ui 18px at weight 400, line height 1.4. Lead paragraphs.
- **body-sm:** system-ui 14px at weight 400. Secondary and small text.
- **caption:** system-ui 11px at weight 400, line height 1.18. Captions and fine print.
- **label-md:** system-ui 16px at weight 500, line height 1.4. Buttons, navigation and labels.
- **label-sm:** Roboto 14px at weight 700. Small labels and badges.
- **code:** Menlo 14px at weight 400, line height 1.4. Code and technical values.

## Layout

Spacing does not follow a strict grid: 69% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.01px, sm 8px, md 16px, lg 24px, xl 60px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgb(110, 112, 114) 0px 1px 4px 0px`
- `rgba(0, 0, 0, 0.2) 0px 2px 5px 0px`
- `rgba(60, 64, 67, 0.15) 0px 1px 3px 0px, rgba(60, 64, 67, 0.3) 0px 1px 2px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 120 elements.
- **sm (2px):** 96 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Okay”):** #007D9C fill, #FFFFFF text, 16px/500, padding 8px.
- **button-secondary (“Get Started”):** #FDDD00 fill, #000000 text, 24px/400, 4px radius, padding 16px 0px, border 1px solid #FDDD00, shadow `rgba(0, 0, 0, 0.2) 0px 2px 5px 0px`.
- **button-outline (“Share”):** #2D2D2D fill, #50B7E0 text, 14px/700, 3px radius, padding 0px 10px, shadow `rgba(0, 0, 0, 0.2) 0px 2px 5px 0px`.
- **button-ghost (“Download”):** transparent fill, #FFFFFF text, 24px/400, 4px radius, padding 16px 0px, border 1px solid #FFFFFF.
- **input-field (“Try Go”):** #253443 fill, #F0F1F2 text, 14px/400, padding 0px 10px.
- **link:** transparent fill, #50B7E0 text, padding 0px.

## Do's and Don'ts

- Do use #202224 for the page and lift surfaces in small steps: #2D2D2D, #253443.
- Do keep text in 3 levels: #F0F1F2, #FFFFFF, #AAACAE.
- Do use #007D9C as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 2px.
- Don't introduce new font families beyond system-ui, Roboto and Menlo.
- Don't use #007D9C for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.1s. Longer ambient animations run 1s.

- **Easing:** `ease-in-out`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/go.dev/), the free DESIGN.md generator.
