---
version: alpha
name: Nike.com
description: "Light monochrome interface measured from nike.com: Nike Futura ND type with Helvetica Now Display Medium, tonal surfaces and 30px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#111111"
  on-background: "#111111"
  on-surface-variant: "#707072"
  surface-container-low: "#F5F5F5"
  primary: "#111111"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: Nike Futura ND
    fontSize: 76px
    fontWeight: 500
    lineHeight: 0.9
  headline-lg:
    fontFamily: Helvetica Now Display Medium
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.2
  headline-md:
    fontFamily: Helvetica Now Display Medium
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
  body-md:
    fontFamily: Helvetica Now Text
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Helvetica Now Text Medium
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: Helvetica Now Text Medium
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Helvetica Now Text Medium
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Nike Futura ND
    fontSize: 40px
    fontWeight: 500
    lineHeight: 0.9
rounded:
  sm: 24px
  md: 30px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 24px
  xl: 48px
  section: 48px
  margin: 48px
  container: 1920px
components:
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 7px 0px 9px 2px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Nike.com Design System

## Overview

Nike.com describes itself as: “Inspiring the world's athletes, Nike delivers innovative products, experiences and services.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#111111)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Nike Futura ND** and **Helvetica Now Display Medium**. Headlines run large; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 30px.

Measured from [nike.com](https://www.nike.com/) on October 29, 2026 at 1440×900 and 390×844 from 366 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 6 roles.

- **White (#FFFFFF):** Page background, seen 17 times. Token `background`, CSS `--podium-cds-button-color-bg-primary-on-dark`.
- **Charcoal (#111111):** Primary text and headings, seen 56 times. Token `on-surface`, CSS `--podium-cds-icon-button-color-bg-primary`.
- **Slate (#707072):** Secondary text, seen 49 times. Token `on-surface-variant`, CSS `--pds-color-element-disabled-always-dark`.
- **Snow (#F5F5F5):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`, CSS `--podium-cds-color-bg-secondary`.
- **Charcoal (#111111):** Primary actions (the main text color; the palette is monochrome), seen 73 times. Token `primary`, CSS `--podium-cds-icon-button-color-bg-primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**Nike Futura ND**, **Helvetica Now Display Medium**, **Helvetica Now Text** and **Helvetica Now Text Medium** share the interface. Fallback stack: `Nike Futura ND, Helvetica Now Text Medium, Helvetica, Arial`.

- **headline-display:** Nike Futura ND 76px at weight 500, line height 0.9, uppercase (40px on mobile). Page title (h1).
- **headline-lg:** Helvetica Now Display Medium 24px at weight 500, line height 1.2. Section headings (h2).
- **headline-md:** Helvetica Now Display Medium 20px at weight 500, line height 1.2. Sub-section headings.
- **body-md:** Helvetica Now Text 16px at weight 400, line height 1.5. Body text.
- **label-lg:** Helvetica Now Text Medium 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** Helvetica Now Text Medium 14px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Helvetica Now Text Medium 12px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 51% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 16px, lg 24px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Container:** content is capped at 1920px.
- **Page margin:** 48px on each side of full-width sections.
- **Breakpoints:** 0px, 599px, 600px, 890px, 891px, 959px, 960px, 961px, 1023px, 1440px, 1920px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F5F5F5) and hairline rings:

- `rgb(17, 17, 17) 0px -1px 0px 0px inset`

## Shapes

Most elements use 30px corners. Measured radii, most used first:

- **md (30px):** 56 elements.
- **sm (24px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“HOW REFRESHING The Milwaukee Bre”):** transparent fill, #111111 text, 16px/400, padding 0px.
- **input-field (“Search”):** #F5F5F5 fill, #111111 text, 16px/500, 24px radius, padding 7px 0px 9px 2px.
- **link:** transparent fill, #707072 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5F5F5.
- Do keep text in 2 levels: #111111, #707072.
- Do let contrast carry emphasis; primary actions use #111111 on #FFFFFF.
- Do reuse the measured spacing steps (6px, 16px, 24px).
- Do use 30px corners on most elements; larger surfaces also use 24px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Nike Futura ND, Helvetica Now Display Medium, Helvetica Now Text and Helvetica Now Text Medium.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s. Longer ambient animations run 0.7s, 0.65s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/nike.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
