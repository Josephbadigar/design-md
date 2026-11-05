---
version: alpha
name: Pangram Pangram
description: "Light interface measured from pangrampangram.com: Neue Montreal type, vivid red accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FAFAFA"
  surface: "#FAFAFA"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#666666"
  surface-container-low: "#FFFFFF"
  surface-container: "#EDEDED"
  outline: "#FFFFFF"
  primary: "#FF2F00"
  on-primary: "#000000"
  secondary: "#FFB700"
typography:
  headline-display:
    fontFamily: Neue Montreal
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1
  headline-lg:
    fontFamily: Neue Montreal
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.3
  body-md:
    fontFamily: Neue Montreal
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.3
  body-sm:
    fontFamily: Neue Montreal
    fontSize: 12.5px
    fontWeight: 400
  label-md:
    fontFamily: Neue Montreal
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.3
  headline-display-mobile:
    fontFamily: Neue Montreal
    fontSize: 25px
    fontWeight: 400
    lineHeight: 1
rounded:
  md: 20px
  full: 9999px
spacing:
  xs: 4px
  sm: 7.65px
  md: 11.65px
  lg: 22.95px
  xl: 45.91px
  gutter: 25.72px
components:
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 7.65px 22.95px
    height: 31px
  button-ghost:
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 7.65px 22.95px
    height: 33px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 24px 45.91px 24px 24px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 25.72px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Pangram Pangram Design System

## Overview

Pangram Pangram describes itself as: “Pangram Pangram is a world-renowned type foundry crafting premium, contemporary fonts for bold brands and creatives. Explore our full catalog, every font is free to try, made to perform across print, digital, and everyth” The interface is light, built on **Snow (#FAFAFA)** with **Near Black (#000000)** text, and **Vivid Red (#FF2F00)** as the main accent.

Type is set in **Neue Montreal**. Headlines run large; body text is 18px. The surface language is flat. Controls are pill-shaped.

Measured from [pangrampangram.com](https://pangrampangram.com/) on November 4, 2026 at 1440×900 and 390×844 from 373 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **Snow (#FAFAFA):** Page background, seen 1 time. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 60 times. Token `on-surface`, CSS `--swiper-pagination-bullet-inactive-color`.
- **Slate (#666666):** Secondary text, seen 50 times. Token `on-surface-variant`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 17 times. Token `surface-container-low`, CSS `--swiper-navigation-color`.
- **Mist (#EDEDED):** Cards and panels, seen 17 times. Token `surface-container`.
- **White (#FFFFFF):** Borders and dividers, seen 3 times. Token `outline`, CSS `--swiper-navigation-color`.
- **Vivid Red (#FF2F00):** Most used accent color, seen 13 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Amber (#FFB700):** Accent, seen 1 time. Token `secondary`.

## Typography

**Neue Montreal** carries the whole interface. Fallback stack: `Neue Montreal, sans-serif`. Other loaded fonts: altera-carve-semibold, neue-gstaad-normal-normal-semibold, palma-fizzy-heavy, neue-montreal-semibold.

- **headline-display:** Neue Montreal 36px at weight 400, line height 1 (25px on mobile). Page title (h1).
- **headline-lg:** Neue Montreal 22px at weight 400, line height 1.3. Section headings (h2).
- **body-md:** Neue Montreal 18px at weight 600, line height 1.3. Body text.
- **body-sm:** Neue Montreal 12.5px at weight 400. Secondary and small text.
- **label-md:** Neue Montreal 14px at weight 400, line height 1.3. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 12% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 7.65px, md 11.65px, lg 22.95px, xl 45.91px.
- **Gaps:** 25.72px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF → #EDEDED) and #FFFFFF borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (20px):** 204 elements.
- **full (9999px):** 88 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Explore font”):** #EDEDED fill, #000000 text, 14px/400, 20px radius, padding 7.65px 22.95px.
- **button-ghost (“Try for Free”):** transparent fill, #FFFFFF text, 14px/400, 20px radius, padding 7.65px 22.95px, border 1px solid #FFFFFF.
- **input-field (“Email address”):** #FFFFFF fill, #000000 text, 14px/400, 20px radius, padding 24px 45.91px 24px 24px.
- **card:** #EDEDED fill, #000000 text, 14px/400, 20px radius, padding 25.72px.
- **link:** transparent fill, #666666 text, padding 0px.

## Do's and Don'ts

- Do use #FAFAFA for the page and lift surfaces in small steps: #FFFFFF, #EDEDED.
- Do keep text in 2 levels: #000000, #666666.
- Do reserve #FF2F00 for primary actions and key highlights.
- Do reuse the measured spacing steps (7.65px, 11.65px, 22.95px).
- Do make buttons and chips fully rounded (9999px); most other elements use 20px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Neue Montreal.
- Don't use #FF2F00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.5s, 0.1s. Longer ambient animations run 0.75s.

- **Easing:** `cubic-bezier(0.22, 1, 0.36, 1)`, `ease`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/pangrampangram.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
