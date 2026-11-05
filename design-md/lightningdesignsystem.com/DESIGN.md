---
version: alpha
name: Salesforce Lightning Design System
description: "Light interface measured from lightningdesignsystem.com: AvantGardeForSalesforce type with Inter, indigo accents, flat surfaces and 3px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#2E2E2E"
  on-background: "#2E2E2E"
  on-surface-strong: "#212121"
  on-surface-variant: "#444444"
  outline: "#0000001F"
  outline-variant: "#E5E5E5"
  primary: "#3A49DA"
  on-primary: "#FFFFFF"
  secondary: "#011744"
  tertiary: "#A8CBFF"
typography:
  headline-display:
    fontFamily: AvantGardeForSalesforce
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.14
  headline-lg:
    fontFamily: AvantGardeForSalesforce
    fontSize: 32px
    fontWeight: 400
  headline-md:
    fontFamily: AvantGardeForSalesforce
    fontSize: 24px
    fontWeight: 400
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: DM sans
    fontSize: 13px
    fontWeight: 400
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
rounded:
  md: 3px
spacing:
  xs: 2px
  sm: 8px
  md: 16px
  lg: 24px
components:
  button-ghost:
    textColor: "#5C5C5C"
    typography: "{typography.body-sm}"
    rounded: 4px
    padding: 0px 8px
  input-field:
    textColor: "#605F60"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 1px 2px
  link:
    textColor: "{colors.on-surface}"
---

# Salesforce Lightning Design System Design System

## Overview

Salesforce Lightning Design System describes itself as: “Lightning Design System 2 · Design system documentation, made with zeroheight” The interface is light, built on **White (#FFFFFF)** with **Graphite (#2E2E2E)** text, and **Indigo (#3A49DA)** as the main accent.

Type is set in **AvantGardeForSalesforce** and **Inter**. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 3px.

Measured from [lightningdesignsystem.com](https://www.lightningdesignsystem.com/2e1ef8501/p/85bd85-lightning-design-system-2) on November 4, 2026 at 1440×900 and 390×844 from 219 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`, CSS `--colors-ui-element-background-main`.
- **Graphite (#2E2E2E):** Primary text and headings, seen 16 times. Token `on-surface`, CSS `--colors-sidebar-text-icon`.
- **Charcoal (#212121):** Headings and emphasis, seen 4 times. Token `on-surface-strong`.
- **Graphite (#444444):** Secondary text, seen 8 times. Token `on-surface-variant`, CSS `--colors-blocks-content-text-styleguide-body`.
- **Near Black 12% (#0000001F):** Borders and dividers, seen 1 time. Token `outline`.
- **Mist (#E5E5E5):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--colors-blocks-table-border-main`.
- **Indigo (#3A49DA):** Brand color in logos and imagery. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Blue (#011744):** Accent in logos and imagery. Token `secondary`.
- **Light Blue (#A8CBFF):** Accent in text, fills and borders, seen 20 times. Token `tertiary`, CSS `--colors-footer-text-links`.

## Typography

**AvantGardeForSalesforce**, **Inter** and **DM sans** share the interface. Fallback stack: `AvantGardeForSalesforce`. Other loaded fonts: DM Sans.

- **headline-display:** AvantGardeForSalesforce 56px at weight 400, line height 1.14. Page title (h1).
- **headline-lg:** AvantGardeForSalesforce 32px at weight 400. Section headings (h2).
- **headline-md:** AvantGardeForSalesforce 24px at weight 400. Sub-section headings.
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-sm:** DM sans 13px at weight 400. Secondary and small text.
- **label-md:** Inter 14px at weight 500, line height 1.43. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 56% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 16px, lg 24px.
- **Breakpoints:** 480px, 699px, 700px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #0000001F borders.

## Shapes

Most elements use 3px corners. Measured radii, most used first:

- **md (3px):** 104 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Fall '26 v 3.5.1”):** transparent fill, #5C5C5C text, 13px/400, 4px radius, padding 0px 8px.
- **input-field (“Search...”):** transparent fill, #605F60 text, 14px/400, padding 1px 2px.
- **link:** transparent fill, #2E2E2E text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #2E2E2E, #212121, #444444.
- Do use #3A49DA as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 3px corners on most elements.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond AvantGardeForSalesforce, Inter and DM sans.
- Don't use #3A49DA for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.1s.

- **Easing:** `ease-in-out`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/lightningdesignsystem.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
