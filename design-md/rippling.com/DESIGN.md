---
version: alpha
name: Rippling
description: "Dark interface measured from rippling.com: basel type, deep purple accents, tonal surfaces and 4px corners."
colors:
  background: "#4A0039"
  surface: "#4A0039"
  on-surface: "#C9B3C4"
  on-background: "#C9B3C4"
  on-surface-strong: "#FFFFFF"
  surface-container-low: "#000000"
  outline: "#FFFFFF4D"
  primary: "#4A0039"
  on-primary: "#FFFFFF"
  inverse-surface: "#EAE4E2"
  secondary: "#000088"
  tertiary: "#7A005D"
  warning: "#FFA81D"
  success: "#128807"
typography:
  headline-display:
    fontFamily: basel
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: -0.015em
  headline-lg:
    fontFamily: basel
    fontSize: 42px
    fontWeight: 500
    lineHeight: 1.14
    letterSpacing: -0.036em
  headline-md:
    fontFamily: basel
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
  headline-sm:
    fontFamily: basel
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: 0.01em
  body-md:
    fontFamily: basel
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.47
    letterSpacing: 0.017em
  body-lg:
    fontFamily: basel
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.44
    letterSpacing: 0.014em
  body-sm:
    fontFamily: basel
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: 0.021em
  label-md:
    fontFamily: basel
    fontSize: 16px
    fontWeight: 400
  label-sm:
    fontFamily: basel
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.47
    letterSpacing: 0.017em
  headline-display-mobile:
    fontFamily: basel
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.17
    letterSpacing: -0.028em
  headline-lg-mobile:
    fontFamily: basel
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
  headline-md-mobile:
    fontFamily: basel
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: 0.008em
rounded:
  sm: 4px
  md: 8px
  lg: 12px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 64px
  gutter: 16px
  section: 64px
components:
  button-primary:
    backgroundColor: "{colors.warning}"
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 24px
    height: 38px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 0px
  input-field:
    textColor: "{colors.surface-container-low}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px 150.61px 0px 0px
  card:
    backgroundColor: "#F2EEEB"
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 120px 24px
  link:
    textColor: "{colors.on-surface}"
---

# Rippling Design System

## Overview

Rippling describes itself as: “Most global systems rely on manual work behind the scenes, resulting in less effective experience for admins and employees. Rippling has been designed to operate differently.” The interface is dark, built on **Deep Purple (#4A0039)** with **Light Purple (#C9B3C4)** text, and **Deep Purple (#4A0039)** as the main accent.

Type is set in **basel**. Headlines run large with tight negative tracking; body text is 15px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [rippling.com](https://www.rippling.com/en-IN/products/global) on October 21, 2026 at 1440×900 and 390×844 from 430 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Deep Purple (#4A0039):** Page background. Token `background`.
- **Light Purple (#C9B3C4):** Primary text and headings. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 14 times. Token `on-surface-strong`, CSS `--tw-ring-offset-color`.
- **Near Black (#000000):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **White 30% (#FFFFFF4D):** Borders and dividers, seen 1 time. Token `outline`.
- **Deep Purple (#4A0039):** Brand color on large areas. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Warm Mist (#EAE4E2):** High-contrast fills, seen 3 times. Token `inverse-surface`.
- **Dark Indigo (#000088):** Accent, seen 50 times. Token `secondary`.
- **Dark Purple (#7A005D):** Accent, seen 3 times. Token `tertiary`.
- **Vivid Orange (#FFA81D):** Warnings and highlights, seen 6 times. Token `warning`.
- **Dark Green (#128807):** Success and positive states, seen 1 time. Token `success`.

## Typography

**basel** carries the whole interface. Fallback stack: `__basel_e55247, __basel_Fallback_e55247, ui-sans-serif, system-ui`. Other loaded fonts: __basel_e55247, __basel_Fallback_e55247.

- **headline-display:** basel 48px at weight 500, line height 1.08, tracking -0.015em (36px on mobile). Page title (h1).
- **headline-lg:** basel 42px at weight 500, line height 1.14, tracking -0.036em (30px on mobile). Section headings (h2).
- **headline-md:** basel 30px at weight 500, line height 1.2 (24px on mobile). Sub-section headings.
- **headline-sm:** basel 24px at weight 500, line height 1.25, tracking 0.01em. Card and feature titles.
- **body-md:** basel 15px at weight 400, line height 1.47, tracking 0.017em. Body text.
- **body-lg:** basel 18px at weight 400, line height 1.44, tracking 0.014em. Lead paragraphs.
- **body-sm:** basel 12px at weight 400, line height 1.33, tracking 0.021em. Secondary and small text.
- **label-md:** basel 16px at weight 400. Buttons, navigation and labels.
- **label-sm:** basel 15px at weight 500, line height 1.47, tracking 0.017em. Small labels and badges.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 1px, 428px, 480px, 481px, 560px, 620px, 767px, 768px, 959px, 1023px, 1024px, 1025px, 1100px, 1280px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 24px 60px -24px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 16 elements.
- **lg (12px):** 16 elements.
- **md (8px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“See Rippling”):** #FFA81D fill, #000000 text, 15px/500, 4px radius, padding 8px 24px.
- **button-ghost (“Products”):** transparent fill, #FFFFFFB3 text, 15px/500, padding 0px.
- **input-field:** transparent fill, #000000 text, 15px/400, padding 0px 150.61px 0px 0px.
- **card:** #F2EEEB fill, #000000 text, 16px/400, padding 120px 24px.
- **link:** transparent fill, #FFFFFFB3 text, padding 0px.

## Do's and Don'ts

- Do use #4A0039 for the page and lift surfaces in small steps: #000000.
- Do keep text in 2 levels: #C9B3C4, #FFFFFF.
- Do use #4A0039 as the brand accent: header, logo and key highlights.
- Do set headlines in basel with tight tracking (-0.015em).
- Do keep spacing on the 4px grid.
- Do use 4px corners on most elements; larger surfaces also use 12px and 8px.
- Don't introduce new font families beyond basel.
- Don't use #4A0039 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/rippling.com/), the free DESIGN.md generator.
