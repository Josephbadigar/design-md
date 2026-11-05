---
version: alpha
name: Josh W. Comeau
description: "Light interface measured from joshwcomeau.com: Wotfard type, light blue accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0A0C10"
  on-background: "#0A0C10"
  on-surface-strong: "#000000"
  on-surface-variant: "#294E60"
  on-surface-muted: "#5A6072"
  primary: "#A0D4EE"
  on-primary: "#000000"
  inverse-surface: "#262D40"
  secondary: "#B1DFF6"
  tertiary: "#4242FA"
typography:
  headline-display:
    fontFamily: Wotfard
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.5
  headline-lg:
    fontFamily: Wotfard
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.042em
  headline-md:
    fontFamily: Wotfard
    fontSize: 22px
    fontWeight: 600
    lineHeight: 1.5
  body-md:
    fontFamily: Wotfard
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Wotfard
    fontSize: 19px
    fontWeight: 500
    lineHeight: 1.5
  body-sm:
    fontFamily: Wotfard
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Wotfard
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Wotfard
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
rounded:
  sm: 2px
  md: 4px
  lg: 8px
  full: 9999px
spacing:
  xs: 4px
  sm: 5px
  md: 16px
  lg: 24px
  xl: 36px
  gutter: 12px
components:
  button-primary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 5px 12px
    height: 31px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px 16px
  input-field:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 4px 8px
  link:
    textColor: "{colors.on-surface}"
---

# Josh W. Comeau Design System

## Overview

Josh W. Comeau describes itself as: “Friendly articles and tutorials for front-end web developers. ❤️” The interface is light, built on **White (#FFFFFF)** with **Cool Charcoal (#0A0C10)** text, and **Light Blue (#A0D4EE)** as the main accent.

Type is set in **Wotfard**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [joshwcomeau.com](https://www.joshwcomeau.com/) on November 4, 2026 at 1440×900 and 390×844 from 327 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles, plus gradient stops #A0D4EE, #7DC4E8.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`, CSS `--color-adaptive-white`.
- **Cool Charcoal (#0A0C10):** Primary text and headings, seen 101 times. Token `on-surface`, CSS `--color-text`.
- **Near Black (#000000):** Headings and emphasis, seen 2 times. Token `on-surface-strong`, CSS `--selection-text-color`.
- **Dark Cyan (#294E60):** Secondary text, seen 20 times. Token `on-surface-variant`.
- **Blue (#5A6072):** Muted text and metadata, seen 6 times. Token `on-surface-muted`, CSS `--color-gray-700`.
- **Light Blue (#A0D4EE):** Brand color on large areas, seen 2 times. Token `primary`, CSS `--color-sky-from`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Deep Blue (#262D40):** High-contrast fills, seen 1 time. Token `inverse-surface`, CSS `--color-gray-900`.
- **Light Blue (#B1DFF6):** Accent on large areas, seen 2 times. Token `secondary`.
- **Vivid Indigo (#4242FA):** Accent (CSS variable), seen 4 times. Token `tertiary`, CSS `--color-action`.

## Typography

**Wotfard** carries the whole interface. Fallback stack: `Wotfard, Wotfard-fallback, sans-serif`. Other loaded fonts: Cartograph CF.

- **headline-display:** Wotfard 32px at weight 700, line height 1.5. Page title (h1).
- **headline-lg:** Wotfard 24px at weight 400, line height 1.5, tracking -0.042em. Section headings (h2).
- **headline-md:** Wotfard 22px at weight 600, line height 1.5. Sub-section headings.
- **body-md:** Wotfard 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Wotfard 19px at weight 500, line height 1.5. Lead paragraphs.
- **body-sm:** Wotfard 12px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Wotfard 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Wotfard 14px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (76% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 5px, md 16px, lg 24px, xl 36px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.02) 0px -5.9px 2.7px 0px, rgba(0, 0, 0, 0.024) 0px -1.2px 6.9px 0px, rgba(0, 0, 0, 0.03) 0px 8px 14.2px 0px, rgba(0, 0, 0, 0.04) 0px 21.9px 29.2px 0px, rgba(0, 0, 0, 0.07) 0px 49px 80px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (2px):** 52 elements.
- **md (4px):** 48 elements.
- **full (9999px):** 44 elements.
- **lg (8px):** 32 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“CSS”):** #B1DFF6 fill, #0A0C10 text, 14px/400, 8px radius, padding 5px 12px.
- **button-ghost (“Categories”):** transparent fill, #0A0C10 text, 16px/400, padding 0px 16px.
- **input-field (“samuel@aol.com”):** transparent fill, #000000 text, 16px/400, padding 4px 8px.
- **link:** transparent fill, #0A0C10 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 4 levels: #0A0C10, #000000, #294E60, #5A6072.
- Do use #A0D4EE as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (5px, 16px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 2px corners.
- Don't introduce new font families beyond Wotfard.
- Don't use #A0D4EE for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.5s, 0.3s, 0.35s, 0.2s.

- **Easing:** `cubic-bezier(0.07, 0.7, 0.35, 1.35)`, `ease`, `cubic-bezier(0.27, 0.22, 0.44, 1.03)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/joshwcomeau.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
