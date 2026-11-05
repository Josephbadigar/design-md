---
version: alpha
name: Homebrew
description: "Dark interface measured from brew.sh: system-ui type, orange accents, flat surfaces and 6.4px corners."
colors:
  background: "#2E2A24"
  surface: "#2E2A24"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#999999"
  overlay: "#FFFFFF0F"
  overlay-strong: "#0000004D"
  outline: "#A26B144D"
  outline-variant: "#745626"
  primary: "#E2A843"
  on-primary: "#000000"
  inverse-surface: "#EBEDF0"
  secondary: "#9C7645"
  tertiary: "#008080"
  warning: "#FFD79A"
typography:
  headline-display:
    fontFamily: system-ui
    fontSize: 53px
    fontWeight: 900
    lineHeight: 0.95
  headline-lg:
    fontFamily: system-ui
    fontSize: 48px
    fontWeight: 800
    lineHeight: 1.1
  headline-md:
    fontFamily: system-ui
    fontSize: 20px
    fontWeight: 800
    lineHeight: 1.1
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.48
  body-lg:
    fontFamily: system-ui
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.48
  body-sm:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.48
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.48
  label-sm:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.48
  headline-display-mobile:
    fontFamily: system-ui
    fontSize: 29px
    fontWeight: 900
    lineHeight: 0.95
  headline-lg-mobile:
    fontFamily: system-ui
    fontSize: 24px
    fontWeight: 800
    lineHeight: 1.1
rounded:
  sm: 4px
  md: 6.4px
spacing:
  sm: 5.6px
  md: 16px
  lg: 20px
  xl: 35.2px
  gutter: 19.2px
components:
  button-primary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "#969FAF"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px 8px
    height: 44px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
    textColor: "#1C1E21"
  input-field:
    backgroundColor: "#EFEFEF"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 5.6px 10.4px
  card:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.warning}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 16px
  link:
    textColor: "{colors.primary}"
---

# Homebrew Design System

## Overview

Homebrew describes itself as: “The Package Manager for Everywhere.” The interface is dark, built on **Warm Graphite (#2E2A24)** with **White (#FFFFFF)** text, and **Orange (#E2A843)** as the main accent.

Type is set in **system-ui**. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 6.4px.

Measured from [brew.sh](https://brew.sh/) on November 4, 2026 at 1440×900 and 390×844 from 196 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Warm Graphite (#2E2A24):** Page background, seen 1 time. Token `background`, CSS `--docsearch-footer-background`.
- **White (#FFFFFF):** Primary text and headings, seen 26 times. Token `on-surface`, CSS `--docsearch-hit-active-color`.
- **Gray (#999999):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **White 6% (#FFFFFF0F):** Translucent fill for cards and controls, seen 7 times. Token `overlay`.
- **Near Black 30% (#0000004D):** Stronger translucent fill, seen 1 time. Token `overlay-strong`, CSS `--docsearch-hit-background`.
- **Dark Orange 30% (#A26B144D):** Borders and dividers, seen 7 times. Token `outline`.
- **Dark Orange (#745626):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Orange (#E2A843):** Brand accent (CSS variable), seen 49 times. Token `primary`, CSS `--docsearch-primary-color`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Mist (#EBEDF0):** High-contrast fills, seen 1 time. Token `inverse-surface`, CSS `--docsearch-searchbox-background`.
- **Orange (#9C7645):** Accent in text, fills and borders, seen 22 times. Token `secondary`.
- **Dark Cyan (#008080):** Accent in text, fills and borders, seen 14 times. Token `tertiary`.
- **Light Orange (#FFD79A):** Warnings and highlights, seen 25 times. Token `warning`.

## Typography

**system-ui** carries the whole interface. Fallback stack: `ui-sans-serif, -apple-system, BlinkMacSystemFont, Helvetica Neue`.

- **headline-display:** system-ui 53px at weight 900, line height 0.95 (29px on mobile). Page title (h1).
- **headline-lg:** system-ui 48px at weight 800, line height 1.1 (24px on mobile). Section headings (h2).
- **headline-md:** system-ui 20px at weight 800, line height 1.1. Sub-section headings.
- **body-md:** system-ui 16px at weight 400, line height 1.48. Body text.
- **body-lg:** system-ui 18px at weight 700, line height 1.48. Lead paragraphs.
- **body-sm:** system-ui 13px at weight 400, line height 1.48. Secondary and small text.
- **label-md:** system-ui 16px at weight 700, line height 1.48. Buttons, navigation and labels.
- **label-sm:** system-ui 13px at weight 700, line height 1.48. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 50% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 5.6px, md 16px, lg 20px, xl 35.2px.
- **Gaps:** 19.2px is the most common gap in flex and grid layouts.
- **Breakpoints:** 480px, 700px, 768px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #A26B144D borders.

## Shapes

Most elements use 6.4px corners. Measured radii, most used first:

- **md (6.4px):** 30 elements.
- **sm (4px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Search K”):** #EBEDF0 fill, #969FAF text, 16px/500, 4px radius, padding 0px 8px.
- **button-primary-hover:** background #FFFFFF, text #1C1E21 on hover.
- **input-field (“Language”):** #EFEFEF fill, #000000 text, 16px/400, padding 5.6px 10.4px, border 1px solid #767676.
- **card:** #FFFFFF0F fill, #FFD79A text, 16px/400, 6.4px radius, padding 16px, border 1px solid #A26B144D.
- **link:** transparent fill, #E2A843 text, padding 0px.

## Do's and Don'ts

- Do use #2E2A24 for the page.
- Do keep text in 2 levels: #FFFFFF, #999999.
- Do use #E2A843 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (5.6px, 16px, 20px).
- Do use 6.4px corners on most elements; larger surfaces also use 4px.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond system-ui.
- Don't use #E2A843 for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/brew.sh/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
