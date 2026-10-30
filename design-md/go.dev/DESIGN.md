---
version: alpha
name: Go
description: "Dark interface measured from go.dev: system-ui type with Roboto, vivid yellow accents, flat surfaces and 4px corners."
colors:
  background: "#007D9C"
  surface: "#007D9C"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#202224"
  outline: "#00ADD8"
  primary: "#FDDD00"
  on-primary: "#000000"
  inverse-surface: "#F8F8F8"
  secondary: "#FFED89"
  tertiary: "#00769C"
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
    typography: "{typography.headline-md}"
    rounded: "{rounded.md}"
    padding: 16px 0px
    height: 64px
  button-secondary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.tertiary}"
    typography: "{typography.label-sm}"
    rounded: 3px
    padding: 0px 10px
    height: 28px
  button-tertiary:
    backgroundColor: "#FFFFDD"
    textColor: "{colors.background}"
    typography: "{typography.label-sm}"
    rounded: 3px
    padding: 0px 10px
    height: 28px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-md}"
    rounded: "{rounded.md}"
    padding: 16px 0px
  input-field:
    backgroundColor: "#FFFFDD"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px 10px
  link:
    textColor: "{colors.background}"
---

# Go Design System

## Overview

Go describes itself as: “Go is an open source programming language that makes it simple to build secure, scalable systems.” The interface is dark, built on **Dark Cyan (#007D9C)** with **White (#FFFFFF)** text, and **Vivid Yellow (#FDDD00)** as the main accent.

Type is set in **system-ui** and **Roboto**, with **Menlo** for code. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [go.dev](https://go.dev/) on October 29, 2026 at 1440×900 and 390×844 from 264 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **Dark Cyan (#007D9C):** Page background, seen 4 times. Token `background`, CSS `--color-brand-primary`.
- **White (#FFFFFF):** Primary text and headings, seen 20 times. Token `on-surface`, CSS `--color-button-inverted-disabled`.
- **Charcoal (#202224):** Secondary text, seen 46 times. Token `on-surface-variant`, CSS `--color-input-text`.
- **Vivid Cyan (#00ADD8):** Borders and dividers, seen 1 time. Token `outline`.
- **Vivid Yellow (#FDDD00):** Primary buttons and calls to action, seen 2 times. Token `primary`, CSS `--yellow`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Snow (#F8F8F8):** High-contrast fills, seen 23 times. Token `inverse-surface`, CSS `--color-background-card-footer`.
- **Light Amber (#FFED89):** Accent on large areas, seen 1 time. Token `secondary`, CSS `--survey-yellow`.
- **Dark Cyan (#00769C):** Accent, seen 18 times. Token `tertiary`, CSS `--color-bright-text-link`.

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

Spacing does not follow a strict grid: 70% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.01px, sm 8px, md 16px, lg 24px, xl 60px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgb(198, 200, 202) 0px 1px 4px 0px`
- `rgba(0, 0, 0, 0.2) 0px 2px 5px 0px`
- `rgba(60, 64, 67, 0.15) 0px 1px 3px 0px, rgba(60, 64, 67, 0.3) 0px 1px 2px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 116 elements.
- **sm (2px):** 96 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #FDDD00 fill, #000000 text, 24px/400, 4px radius, padding 16px 0px, border 1px solid #FDDD00, shadow `rgba(0, 0, 0, 0.2) 0px 2px 5px 0px`.
- **button-secondary (“Share”):** #F8F8F8 fill, #00769C text, 14px/700, 3px radius, padding 0px 10px, shadow `rgba(0, 0, 0, 0.2) 0px 2px 5px 0px`.
- **button-tertiary (“Run”):** #FFFFDD fill, #007D9C text, 14px/700, 3px radius, padding 0px 10px, border 1px solid #00ADD8, shadow `rgba(0, 0, 0, 0.2) 0px 2px 5px 0px`.
- **button-ghost (“Download”):** transparent fill, #FFFFFF text, 24px/400, 4px radius, padding 16px 0px, border 1px solid #FFFFFF.
- **input-field (“Try Go”):** #FFFFDD fill, #202224 text, 14px/400, padding 0px 10px.
- **link:** transparent fill, #007D9C text, padding 0px.

## Do's and Don'ts

- Do use #007D9C for the page.
- Do keep text in 2 levels: #FFFFFF, #202224.
- Do reserve #FDDD00 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 2px.
- Don't use #202224 for body text; it reaches 3.35:1 on #007D9C. Keep it for large text or metadata.
- Don't introduce new font families beyond system-ui, Roboto and Menlo.
- Don't use #FDDD00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.1s. Longer ambient animations run 1s.

- **Easing:** `ease-in-out`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/go.dev/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
