---
version: alpha
name: Lemonsqueezy
description: "Dark interface measured from lemonsqueezy.com: Circularpro book type with Inter, vivid violet accents, flat surfaces and 8px corners."
colors:
  background: "#5423E7"
  surface: "#5423E7"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#121217"
  primary: "#5423E7"
  on-primary: "#FFFFFF"
  inverse-surface: "#F7F7F8"
  secondary: "#7047EB"
  warning: "#FFC233"
typography:
  headline-display:
    fontFamily: Circularpro book
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Circularpro book
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.14
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Circularpro book
    fontSize: 38.5px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Circularpro book
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.22
    letterSpacing: -0.02em
  title-lg:
    fontFamily: Circularpro book
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.22
    letterSpacing: -0.02em
  body-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
  caption:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: -0.01em
  headline-display-mobile:
    fontFamily: Circularpro book
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.04em
  title-lg-mobile:
    fontFamily: Circularpro book
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.22
    letterSpacing: -0.02em
rounded:
  sm: 8px
  md: 40px
spacing:
  sm: 8px
  md: 9px
  lg: 30px
  xl: 40px
  gutter: 12px
components:
  button-primary:
    backgroundColor: "#FFFFFFE6"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px
    height: 57px
  button-primary-hover:
    backgroundColor: "#FFD266"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.caption}"
    rounded: "{rounded.md}"
    padding: 8px 20px
    height: 40px
  button-ghost:
    textColor: "#FFFFFF99"
    typography: "{typography.caption}"
    rounded: 0px
    padding: 32px 8px 32px 16px
  card:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
---

# Lemonsqueezy Design System

## Overview

Lemonsqueezy describes itself as: “Sell digital products and SaaS software the easy peasy way with Lemon Squeezy. As your merchant of record, we handle the tax compliance burden so you can focus on more revenue and less headache.” The interface is dark, built on **Vivid Violet (#5423E7)** with **White (#FFFFFF)** text, and **Vivid Violet (#5423E7)** as the main accent.

Type is set in **Circularpro book** and **Inter**. Headlines run large with tight negative tracking; body text is 18px. The surface language is flat. Corners are mostly 8px.

Measured from [lemonsqueezy.com](https://www.lemonsqueezy.com/) on October 21, 2026 at 1440×900 and 559×1210 from 86 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Vivid Violet (#5423E7):** Page background, seen 3 times. Token `background`, CSS `--blue`.
- **White (#FFFFFF):** Primary text and headings, seen 1 time. Token `on-surface`.
- **Charcoal (#121217):** Secondary text, seen 6 times. Token `on-surface-variant`, CSS `--black-2`.
- **Vivid Violet (#5423E7):** Brand color on large areas, seen 3 times. Token `primary`, CSS `--blue`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Snow (#F7F7F8):** High-contrast fills, seen 4 times. Token `inverse-surface`, CSS `--grey-50-51`.
- **Vivid Violet (#7047EB):** Accent, seen 1 time. Token `secondary`, CSS `--purple-500`.
- **Vivid Amber (#FFC233):** Warnings and highlights, seen 1 time. Token `warning`, CSS `--ls-color-yellow`.

## Typography

**Circularpro book** and **Inter** share the interface. Fallback stack: `Circularpro book, sans-serif`.

- **headline-display:** Circularpro book 80px at weight 400, line height 1, tracking -0.04em (40px on mobile). Page title (h1).
- **headline-lg:** Circularpro book 56px at weight 400, line height 1.14, tracking -0.03em. Section headings (h2).
- **headline-md:** Circularpro book 38.5px at weight 400, line height 1.2, tracking -0.02em. Sub-section headings.
- **headline-sm:** Circularpro book 36px at weight 400, line height 1.22, tracking -0.02em. Card and feature titles.
- **title-lg:** Circularpro book 26px at weight 400, line height 1.22, tracking -0.02em (24px on mobile). Small titles.
- **body-md:** Inter 18px at weight 400, line height 1.6. Body text.
- **body-sm:** Inter 16px at weight 400, line height 1.6. Secondary and small text.
- **caption:** Inter 15px at weight 400, line height 1.6. Captions and fine print.
- **label-md:** Inter 16px at weight 500, line height 1.4, tracking -0.01em. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (78% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** sm 8px, md 9px, lg 30px, xl 40px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 390px, 479px, 480px, 767px, 768px, 990px, 991px, 1280px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 28 elements.
- **md (40px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #FFFFFFE6 fill, #121217 text, 18px/500, 40px radius, padding 0px.
- **button-primary-hover:** background #FFD266, text #121217 on hover.
- **button-secondary (“Get started”):** #FFFFFF fill, #121217 text, 15px/500, 40px radius, padding 8px 20px.
- **button-ghost (“Platform”):** transparent fill, #FFFFFF99 text, 15px/400, padding 32px 8px 32px 16px.
- **card:** #F7F7F8 fill, #121217 text, 18px/400, padding 0px.

## Do's and Don'ts

- Do use #5423E7 for the page.
- Do keep text in 2 levels: #FFFFFF, #121217.
- Do use #5423E7 as the brand accent: header, logo and key highlights.
- Do set headlines in Circularpro book with tight tracking (-0.04em).
- Do reuse the measured spacing steps (8px, 9px, 30px).
- Do use 8px corners on most elements; larger surfaces also use 40px.
- Don't use #121217 for body text; it reaches 2.5:1 on #5423E7. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Circularpro book and Inter.
- Don't use #5423E7 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.18s, 0.1s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/lemonsqueezy.com/), the free DESIGN.md generator.
