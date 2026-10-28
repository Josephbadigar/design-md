---
version: alpha
name: Python.org
description: "Light interface measured from python.org: Flux-Regular type with SourceSansProBold, dark blue accents, tonal surfaces and 6px corners."
colors:
  background: "#F9F9F9"
  surface: "#F9F9F9"
  on-surface: "#444444"
  on-background: "#444444"
  on-surface-variant: "#4D4D4D"
  on-surface-muted: "#666666"
  on-surface-subtle: "#999999"
  surface-container-low: "#FFFFFF"
  surface-container: "#E6E8EA"
  outline: "#CACCCE"
  outline-variant: "#F2F4F6"
  primary: "#2B5B84"
  on-primary: "#FFFFFF"
  inverse-surface: "#1F2A32"
  secondary: "#1C3B56"
  tertiary: "#FFDF76"
  success: "#0D870D"
  warning: "#FFD343"
typography:
  headline-display:
    fontFamily: Flux-Regular
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.25
  headline-lg:
    fontFamily: SourceSansProBold
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1
  body-md:
    fontFamily: SourceSansProRegular
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.63
  body-lg:
    fontFamily: SourceSansProRegular
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.63
  body-sm:
    fontFamily: SourceSansProRegular
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.62
  caption:
    fontFamily: SourceSansProRegular
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.62
  label-md:
    fontFamily: SourceSansProRegular
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.63
rounded:
  sm: 6px
  md: 8px
spacing:
  xs: 2.63px
  sm: 5.25px
  md: 10.5px
  lg: 22.5px
components:
  button-primary:
    backgroundColor: "{colors.warning}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 6.4px 12px 5.6px 12px
    height: 32px
  button-primary-hover:
    textColor: "#1A1A1A"
  button-secondary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 8px 12px 6.4px 12px
    height: 42px
  button-tertiary:
    backgroundColor: "#006DAD"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 6.4px 12px 5.6px 12px
    height: 40px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#BBBBBB"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 6.4px 8px 4.8px 8px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Python.org Design System

## Overview

Python.org describes itself as: “The official home of the Python Programming Language” The interface is light, built on **Snow (#F9F9F9)** with **Graphite (#444444)** text, and **Dark Blue (#2B5B84)** as the main accent.

Type is set in **Flux-Regular** and **SourceSansProBold**. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 6px.

Measured from [python.org](https://www.python.org/) on October 21, 2026 at 1440×900 and 390×844 from 318 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #3776AB, #2B5B84, #FFDF76, #FFD343.

- **Snow (#F9F9F9):** Page background. Token `background`.
- **Graphite (#444444):** Primary text and headings, seen 35 times. Token `on-surface`, CSS `--color-default`.
- **Slate (#4D4D4D):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Slate (#666666):** Muted text and metadata, seen 47 times. Token `on-surface-muted`, CSS `--color-grey`.
- **Gray (#999999):** Subtle text and placeholders, seen 20 times. Token `on-surface-subtle`, CSS `--color-grey-light`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`, CSS `--color-white`.
- **Mist (#E6E8EA):** Cards and panels, seen 31 times. Token `surface-container`, CSS `--color-grey-lightest`.
- **Silver (#CACCCE):** Borders and dividers, seen 46 times. Token `outline`, CSS `--color-grey-lighter`.
- **Snow (#F2F4F6):** Secondary dividers, seen 30 times. Token `outline-variant`.
- **Dark Blue (#2B5B84):** Brand color in the header, seen 15 times. Token `primary`, CSS `--color-blue-medium`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Blue (#1F2A32):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Dark Blue (#1C3B56):** Brand color on large areas, seen 62 times. Token `secondary`.
- **Light Amber (#FFDF76):** Brand color on large areas, seen 26 times. Token `tertiary`.
- **Dark Green (#0D870D):** Success and positive states, seen 26 times. Token `success`.
- **Amber (#FFD343):** Warnings and highlights, seen 15 times. Token `warning`, CSS `--color-yellow`.

## Typography

**Flux-Regular**, **SourceSansProBold** and **SourceSansProRegular** share the interface. Fallback stack: `Flux-Regular, SourceSansProRegular, Arial, sans-serif`. Other loaded fonts: Pythonicon, Flux-Bold, SourceSansProItalic.

- **headline-display:** Flux-Regular 24px at weight 400, line height 1.25. Page title (h1).
- **headline-lg:** SourceSansProBold 21px at weight 400, line height 1. Section headings (h2).
- **body-md:** SourceSansProRegular 14px at weight 400, line height 1.63. Body text.
- **body-lg:** SourceSansProRegular 15px at weight 400, line height 1.63. Lead paragraphs.
- **body-sm:** SourceSansProRegular 13px at weight 400, line height 1.62. Secondary and small text.
- **caption:** SourceSansProRegular 12px at weight 400, line height 1.62. Captions and fine print.
- **label-md:** SourceSansProRegular 16px at weight 400, line height 1.63. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 14% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2.63px, sm 5.25px, md 10.5px, lg 22.5px.
- **Breakpoints:** 640px, 768px, 860px, 1200px, 1320px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#FFFFFF → #E6E8EA):

- `rgba(55, 118, 171, 0.2) 0px 0px 5px 0px inset`
- `rgba(0, 0, 0, 0.03) 0px 0px 50px 0px inset, rgba(0, 0, 0, 0.03) 0px 0px 20px 0px inset`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0.05) 1px 1px 1px 0px, rgba(255, 255, 255, 0.5) 0px 0px 5px 0px inset`.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **sm (6px):** 44 elements.
- **md (8px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Donate”):** #FFD343 fill, #4D4D4D text, 16px/400, 6px radius, padding 6.4px 12px 5.6px 12px, border 1px solid #DCA900, shadow `rgba(0, 0, 0, 0.05) 1px 1px 1px 0px, rgba(255, 255, 255, 0.5) 0px 0px 5px 0px inset`.
- **button-primary-hover:** background #FFD343, text #1A1A1A on hover.
- **button-secondary (“Python”):** #1F2A32 fill, #FFFFFF text, 16px/400, padding 8px 12px 6.4px 12px.
- **button-tertiary (“See more”):** #006DAD fill, #4D4D4D text, 16px/400, 6px radius, padding 6.4px 12px 5.6px 12px, border 1px solid #006DAD, shadow `rgba(0, 0, 0, 0.05) 1px 1px 1px 0px, rgba(255, 255, 255, 0.5) 0px 0px 5px 0px inset`.
- **input-field (“Search”):** #FFFFFF fill, #BBBBBB text, 16px/400, padding 6.4px 8px 4.8px 8px.
- **link:** transparent fill, #666666 text, padding 0px.

## Do's and Don'ts

- Do use #F9F9F9 for the page and lift surfaces in small steps: #FFFFFF, #E6E8EA.
- Do keep text in 4 levels: #444444, #4D4D4D, #666666, #999999.
- Do use #2B5B84 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (5.25px, 10.5px, 22.5px).
- Do use 6px corners on most elements; larger surfaces also use 8px.
- Don't use #999999 for body text; it reaches 2.7:1 on #F9F9F9. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Flux-Regular, SourceSansProBold and SourceSansProRegular.
- Don't use #2B5B84 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s.

- **Easing:** `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/python.org/), the free DESIGN.md generator.
