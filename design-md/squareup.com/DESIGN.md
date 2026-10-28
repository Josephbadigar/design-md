---
version: alpha
name: Square
description: "Light interface measured from squareup.com: Square Sans Display VF type with Exact Block, vivid blue accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#707070"
  on-surface-muted: "#999999"
  on-surface-subtle: "#BBBBBB"
  surface-container-low: "#F7F6F5"
  overlay: "#00000040"
  outline: "#CCCCCC"
  outline-variant: "#80808059"
  primary: "#004BFF"
  on-primary: "#FFFFFF"
  secondary: "#041EEC"
  tertiary: "#006AFF"
typography:
  headline-display:
    fontFamily: Square Sans Display VF
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1.16
    letterSpacing: -0.008em
  headline-lg:
    fontFamily: Exact Block
    fontSize: 56px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Exact Block
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Cash Sans
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.01em
  body-md:
    fontFamily: Square Sans Text VF
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Square Sans Text VF
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: Square Sans Text VF
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1
  label-lg:
    fontFamily: Cash Sans
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: Square Sans Text VF
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Square Sans Text VF
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Square Sans Display VF
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0.013em
  headline-md-mobile:
    fontFamily: Exact Block
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.02em
rounded:
  xs: 4px
  sm: 10px
  md: 20px
  lg: 50px
  xl: 100px
  full: 9999px
spacing:
  xs: 3px
  sm: 8px
  md: 10px
  lg: 20px
  xl: 40px
  gutter: 10px
  section: 120px
components:
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.xs}"
    padding: 18px 10px
  input-field:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-primary}"
---

# Square Design System

## Overview

Square describes itself as: “Sell anywhere. Diversify revenue streams. Streamline operations. Manage your staff. Get paid faster. Sign up for Square today.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Blue (#004BFF)** as the main accent.

Type is set in **Square Sans Display VF** and **Exact Block**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [squareup.com](https://squareup.com/us/en) on October 21, 2026 at 1440×900 and 390×844 from 414 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 8 times. Token `background`, CSS `--color-form-field-hover-color-mode-dark`.
- **Near Black (#000000):** Primary text and headings, seen 41 times. Token `on-surface`, CSS `--action-variant-modal-text-color-color-mode-light`.
- **Slate (#707070):** Secondary text, seen 13 times. Token `on-surface-variant`, CSS `--color-neutral-300`.
- **Gray (#999999):** Muted text and metadata, seen 3 times. Token `on-surface-muted`.
- **Silver (#BBBBBB):** Subtle text and placeholders, seen 2 times. Token `on-surface-subtle`, CSS `--color-neutral-600`.
- **Snow (#F7F6F5):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`, CSS `--color-background-accent`.
- **Near Black 25% (#00000040):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Silver (#CCCCCC):** Borders and dividers, seen 3 times. Token `outline`, CSS `--color-gray-15`.
- **Gray 35% (#80808059):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Blue (#004BFF):** Brand color on large areas, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#041EEC):** Brand color in logos and imagery, seen 38 times. Token `secondary`.
- **Vivid Blue (#006AFF):** Most used accent color, seen 15 times. Token `tertiary`, CSS `--action-variant-button-alt-border-color`.

## Typography

**Square Sans Display VF**, **Exact Block**, **Cash Sans** and **Square Sans Text VF** share the interface. Fallback stack: `Square Sans Display VF, Square Sans Display, Helvetica, Arial`. Other loaded fonts: Square Sans Text, Cash Sans Mono.

- **headline-display:** Square Sans Display VF 64px at weight 400, line height 1.16, tracking -0.008em (40px on mobile). Page title (h1).
- **headline-lg:** Exact Block 56px at weight 500, line height 1, tracking -0.03em. Section headings (h2).
- **headline-md:** Exact Block 40px at weight 400, line height 1.13, tracking -0.02em (32px on mobile). Sub-section headings.
- **headline-sm:** Cash Sans 24px at weight 500, line height 1.2, tracking -0.01em. Card and feature titles.
- **body-md:** Square Sans Text VF 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Square Sans Text VF 14px at weight 400, line height 1.5. Secondary and small text.
- **caption:** Square Sans Text VF 10px at weight 400, line height 1. Captions and fine print.
- **label-lg:** Cash Sans 18px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** Square Sans Text VF 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Square Sans Text VF 14px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 36% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 8px, md 10px, lg 20px, xl 40px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Breakpoints:** 373px, 374px, 479px, 480px, 718px, 739px, 740px, 1023px, 1024px, 1279px, 1280px, 1679px, 1680px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F7F6F5) and hairline rings:

- `rgb(112, 112, 112) 0px 0px 0px 1px inset`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **xs (4px):** 48 elements.
- **lg (50px):** 48 elements.
- **xl (100px):** 20 elements.
- **sm (10px):** 4 elements.
- **md (20px):** 4 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Business types”):** transparent fill, #000000 text, 18px/500, 4px radius, padding 18px 10px.
- **input-field (“Email address”):** #000000 fill, #FFFFFF text, 14px/400, 10px radius, padding 12px 16px, shadow `rgb(112, 112, 112) 0px 0px 0px 1px inset`.
- **card:** #F7F6F5 fill, #000000 text, 16px/400, padding 0px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F7F6F5.
- Do keep text in 4 levels: #000000, #707070, #999999, #BBBBBB.
- Do use #004BFF as the brand accent: header, logo and key highlights.
- Do set headlines in Square Sans Display VF with tight tracking (-0.008em).
- Do reuse the measured spacing steps (8px, 10px, 20px).
- Do use 4px corners on most elements; larger surfaces also use 50px, 100px and 10px.
- Don't use #999999 for body text; it reaches 2.9:1 on #FFFFFF. Keep it for large text or metadata.
- Don't use #BBBBBB for body text; it reaches 1.9:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Square Sans Display VF, Exact Block, Cash Sans and Square Sans Text VF.
- Don't use #004BFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.6s, 0.25s.

- **Easing:** `cubic-bezier(0, 0, 0.2, 1)`, `ease`, `cubic-bezier(0.4, 0, 1, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/squareup.com/), the free DESIGN.md generator.
