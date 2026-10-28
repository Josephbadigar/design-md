---
version: alpha
name: GSAP
description: "Dark monochrome interface measured from gsap.com: Mori type, tonal surfaces and 100px corners."
colors:
  background: "#0E100F"
  surface: "#0E100F"
  on-surface: "#FFFCE1"
  on-background: "#FFFCE1"
  on-surface-variant: "#FEC5FB"
  on-surface-muted: "#7C7C6F"
  surface-container-low: "#000000"
  primary: "#FFFCE1"
  on-primary: "#000000"
  secondary: "#9D95FF"
  tertiary: "#FF8709"
  success: "#0AE448"
typography:
  headline-display:
    fontFamily: Mori
    fontSize: 101px
    fontWeight: 600
    lineHeight: 1
  headline-lg:
    fontFamily: Mori
    fontSize: 44.5px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Mori
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1
  headline-sm:
    fontFamily: Mori
    fontSize: 33px
    fontWeight: 600
    lineHeight: 1
  title-lg:
    fontFamily: Mori
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.15
  body-md:
    fontFamily: Mori
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.15
  body-sm:
    fontFamily: Mori
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  caption:
    fontFamily: Mori
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.01em
  label-md:
    fontFamily: Mori
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.15
  label-sm:
    fontFamily: Mori
    fontSize: 15.5px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.01em
rounded:
  sm: 1px
  md: 8px
  lg: 100px
  full: 9999px
spacing:
  sm: 7.32px
  md: 16px
  lg: 24px
  xl: 33.65px
  gutter: 16px
  section: 108.12px
  margin: 16px
components:
  button-ghost:
    textColor: "{colors.on-surface-muted}"
    rounded: 0px
    padding: 16px 0px
  input-field:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 16px 0px
  link:
    textColor: "{colors.primary}"
---

# GSAP Design System

## Overview

GSAP describes itself as: “Supported by Webflow. Animate Anything - A wildly robust JavaScript animation library built for professionals.” The interface is dark, built on **Charcoal (#0E100F)** with **Pale Yellow (#FFFCE1)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Mori**. Headlines run large; body text is 19px. The surface language is flat. Corners are mostly 100px.

Measured from [gsap.com](https://gsap.com/) on October 21, 2026 at 1440×900 and 390×844 from 358 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles, plus gradient stops #0AE448, #ABFF84, #F7BDF8, #2F3CC0.

- **Charcoal (#0E100F):** Page background, seen 3 times. Token `background`, CSS `--color-just-black`.
- **Pale Yellow (#FFFCE1):** Primary text and headings, seen 66 times. Token `on-surface`, CSS `--color-surface-white`.
- **Pale Purple (#FEC5FB):** Secondary text, seen 2 times. Token `on-surface-variant`, CSS `--color-pink`.
- **Warm Slate (#7C7C6F):** Muted text and metadata, seen 8 times. Token `on-surface-muted`, CSS `--color-surface50`.
- **Near Black (#000000):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **Pale Yellow (#FFFCE1):** Primary actions (the main text color; the palette is monochrome), seen 95 times. Token `primary`, CSS `--color-surface-white`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Light Indigo (#9D95FF):** Most used accent color, seen 5 times. Token `secondary`, CSS `--color-lilac`.
- **Vivid Orange (#FF8709):** Most used accent color, seen 3 times. Token `tertiary`, CSS `--color-orangey`.
- **Vivid Green (#0AE448):** Success and positive states, seen 4 times. Token `success`, CSS `--color-shockingly-green`.

## Typography

**Mori** carries the whole interface. Fallback stack: `Mori, sans-serif`.

- **headline-display:** Mori 101px at weight 600, line height 1. Page title (h1).
- **headline-lg:** Mori 44.5px at weight 400, line height 1.2, tracking -0.01em. Section headings (h2).
- **headline-md:** Mori 40px at weight 600, line height 1. Sub-section headings.
- **headline-sm:** Mori 33px at weight 600, line height 1. Card and feature titles.
- **title-lg:** Mori 32px at weight 400, line height 1.15. Small titles.
- **body-md:** Mori 19px at weight 400, line height 1.15. Body text.
- **body-sm:** Mori 16px at weight 400, line height 1.15. Secondary and small text.
- **caption:** Mori 14px at weight 400, line height 1.4, tracking -0.01em. Captions and fine print.
- **label-md:** Mori 16px at weight 600, line height 1.15. Buttons, navigation and labels.
- **label-sm:** Mori 15.5px at weight 600, line height 1.2, tracking -0.01em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 44% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 7.32px, md 16px, lg 24px, xl 33.65px.
- **Sections:** 108.12px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Page margin:** 16px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#000000).

## Shapes

Most elements use 100px corners. Measured radii, most used first:

- **lg (100px):** 24 elements.
- **md (8px):** 20 elements.
- **full (9999px):** 8 elements.
- **sm (1px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Tools”):** transparent fill, #7C7C6F text, 18px/600, padding 16px 0px.
- **input-field (“Email Address”):** transparent fill, #000000 text, 16px/400, padding 16px 0px.
- **link:** transparent fill, #FFFCE1 text, padding 0px.

## Do's and Don'ts

- Do use #0E100F for the page and lift surfaces in small steps: #000000.
- Do keep text in 3 levels: #FFFCE1, #FEC5FB, #7C7C6F.
- Do let contrast carry emphasis; primary actions use #FFFCE1 on #0E100F.
- Do reuse the measured spacing steps (7.32px, 16px, 24px).
- Do use 100px corners on most elements; larger surfaces also use 8px and 1px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Mori.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.1s, 0.05s, 0.15s.

- **Easing:** `cubic-bezier(0.645, 0.045, 0.355, 1)`, `ease`, `ease-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/gsap.com/), the free DESIGN.md generator.
