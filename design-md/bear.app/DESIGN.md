---
version: alpha
name: Bear
description: "Light interface measured from bear.app: bearsansheadline type with bearsans, red accents, flat surfaces and 3.84px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#444444"
  on-background: "#444444"
  on-surface-variant: "#888888"
  outline: "#F3F5F7"
  outline-variant: "#D9D9D9"
  primary: "#DD4C4F"
  on-primary: "#000000"
  secondary: "#456AA3"
typography:
  headline-display:
    fontFamily: bearsansheadline
    fontSize: 51px
    fontWeight: 400
    lineHeight: 1.1
  headline-lg:
    fontFamily: bearsansheadline
    fontSize: 41.5px
    fontWeight: 400
    lineHeight: 1.1
  headline-md:
    fontFamily: bearsansheadline
    fontSize: 30.5px
    fontWeight: 400
    lineHeight: 1.1
  headline-sm:
    fontFamily: bearsans
    fontSize: 22.5px
    fontWeight: 400
    lineHeight: 1.4
  body-md:
    fontFamily: bearsans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.7
  body-lg:
    fontFamily: bearsans
    fontSize: 17.5px
    fontWeight: 700
    lineHeight: 1.45
  headline-display-mobile:
    fontFamily: bearsansheadline
    fontSize: 41.5px
    fontWeight: 400
    lineHeight: 1.1
rounded:
  sm: 3.84px
  md: 8.64px
spacing:
  xs: 3.84px
  sm: 6.4px
  md: 12.8px
  lg: 32px
  xl: 48px
  container: 960px
components:
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: 8.8px
    padding: 0px 17.6px
  link:
    textColor: "{colors.on-surface}"
---

# Bear Design System

## Overview

Bear describes itself as: “Bear is a beautiful, powerfully simple Markdown note taking app to capture, write, and organize your life.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#444444)** text, and **Red (#DD4C4F)** as the main accent.

Type is set in **bearsansheadline** and **bearsans**. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 3.84px.

Measured from [bear.app](https://bear.app/) on November 4, 2026 at 1440×900 and 390×844 from 320 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`, CSS `--background-color`.
- **Graphite (#444444):** Primary text and headings, seen 90 times. Token `on-surface`, CSS `--text-color`.
- **Gray (#888888):** Secondary text, seen 15 times. Token `on-surface-variant`, CSS `--text-secondary-color`.
- **Snow (#F3F5F7):** Borders and dividers, seen 12 times. Token `outline`, CSS `--background-secondary-color`.
- **Silver (#D9D9D9):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--text-tertiary-color`.
- **Red (#DD4C4F):** Brand accent (CSS variable), seen 9 times. Token `primary`, CSS `--accent-color`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Blue (#456AA3):** Accent, seen 1 time. Token `secondary`.

## Typography

**bearsansheadline** and **bearsans** share the interface. Fallback stack: `bearsansheadline`.

- **headline-display:** bearsansheadline 51px at weight 400, line height 1.1 (41.5px on mobile). Page title (h1).
- **headline-lg:** bearsansheadline 41.5px at weight 400, line height 1.1. Section headings (h2).
- **headline-md:** bearsansheadline 30.5px at weight 400, line height 1.1. Sub-section headings.
- **headline-sm:** bearsans 22.5px at weight 400, line height 1.4. Card and feature titles.
- **body-md:** bearsans 16px at weight 400, line height 1.7. Body text.
- **body-lg:** bearsans 17.5px at weight 700, line height 1.45. Lead paragraphs.

## Layout

Spacing does not follow a strict grid: 27% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.84px, sm 6.4px, md 12.8px, lg 32px, xl 48px.
- **Container:** content is capped at 960px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #F3F5F7 borders.

## Shapes

Most elements use 3.84px corners. Measured radii, most used first:

- **sm (3.84px):** 20 elements.
- **md (8.64px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **input-field (“Your email address”):** #FFFFFF fill, #444444 text, 17.6px/400, 8.8px radius, padding 0px 17.6px, border 1px solid #D9D9D9.
- **link:** transparent fill, #444444 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #444444, #888888.
- Do use #DD4C4F as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (6.4px, 12.8px, 32px).
- Do use 3.84px corners on most elements; larger surfaces also use 8.64px.
- Don't use #888888 for body text; it reaches 3.54:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond bearsansheadline and bearsans.
- Don't use #DD4C4F for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/bear.app/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
