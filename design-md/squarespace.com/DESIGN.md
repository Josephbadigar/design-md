---
version: alpha
name: Squarespace
description: "Dark monochrome interface measured from squarespace.com: Clarkson type with Clarkson Serif, tonal surfaces and 8px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#898989"
  surface-container-low: "#2F2F2F"
  overlay: "#FFFFFF4D"
  overlay-strong: "#FFFFFF33"
  primary: "#FFFFFF"
  on-primary: "#000000"
typography:
  headline-display:
    fontFamily: Clarkson
    fontSize: 64px
    fontWeight: 300
    lineHeight: 1.04
    letterSpacing: -0.06em
  headline-lg:
    fontFamily: Clarkson
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: -0.04em
  headline-md:
    fontFamily: Clarkson Serif
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Clarkson
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.01em
  body-md:
    fontFamily: Clarkson
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.001em
  body-sm:
    fontFamily: Clarkson
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
  label-lg:
    fontFamily: sans-serif
    fontSize: 16px
    fontWeight: 400
  label-md:
    fontFamily: Clarkson
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: -0.001em
  label-sm:
    fontFamily: Clarkson
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Clarkson
    fontSize: 42.5px
    fontWeight: 300
    lineHeight: 1.04
    letterSpacing: -0.06em
  headline-lg-mobile:
    fontFamily: Clarkson
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: -0.04em
  headline-md-mobile:
    fontFamily: Clarkson
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.01em
rounded:
  sm: 4px
  md: 8px
  lg: 30px
  xl: 100px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 40px
  gutter: 12px
  section: 120px
  margin: 40px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 23px 28px
    height: 60px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  input-field:
    backgroundColor: "{colors.overlay-strong}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.primary}"
---

# Squarespace Design System

## Overview

Squarespace describes itself as: “Create a website and grow your business with a free Squarespace trial. Start with customizable website templates, AI website builder tools, or a domain name.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Clarkson** and **Clarkson Serif**. Headlines run large with tight negative tracking; body text is 15px. The surface language is flat. Corners are mostly 8px.

Measured from [squarespace.com](https://www.squarespace.com/) on October 29, 2026 at 1440×900 and 390×844 from 386 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Near Black (#000000):** Page background, seen 12 times. Token `background`, CSS `--primitive-black`.
- **White (#FFFFFF):** Primary text and headings, seen 105 times. Token `on-surface`, CSS `--primitive-white`.
- **Gray (#898989):** Secondary text, seen 2 times. Token `on-surface-variant`, CSS `--color-gray-500`.
- **Graphite (#2F2F2F):** Raised areas one step from the page, seen 9 times. Token `surface-container-low`.
- **White 30% (#FFFFFF4D):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **White 20% (#FFFFFF33):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 163 times. Token `primary`, CSS `--primitive-white`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.

## Typography

**Clarkson**, **Clarkson Serif** and **sans-serif** share the interface. Fallback stack: `Clarkson, Helvetica, sans-serif`.

- **headline-display:** Clarkson 64px at weight 300, line height 1.04, tracking -0.06em (42.5px on mobile). Page title (h1).
- **headline-lg:** Clarkson 40px at weight 400, line height 1.08, tracking -0.04em (26px on mobile). Section headings (h2).
- **headline-md:** Clarkson Serif 26px at weight 400, line height 1.08, tracking -0.02em (18px on mobile). Sub-section headings.
- **headline-sm:** Clarkson 20px at weight 500, line height 1.2, tracking -0.01em. Card and feature titles.
- **body-md:** Clarkson 15px at weight 400, line height 1.4, tracking -0.001em. Body text.
- **body-sm:** Clarkson 12px at weight 400, line height 1.4. Secondary and small text.
- **label-lg:** sans-serif 16px at weight 400. Large buttons and tabs.
- **label-md:** Clarkson 15px at weight 500, line height 1.4, tracking -0.001em. Buttons, navigation and labels.
- **label-sm:** Clarkson 14px at weight 500, line height 1. Small labels and badges.

## Layout

Spacing follows a 4px grid: 98% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 32px, xl 40px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Page margin:** 40px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#2F2F2F).

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 156 elements.
- **xl (100px):** 32 elements.
- **sm (4px):** 16 elements.
- **lg (30px):** 8 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“GET STARTED →”):** #FFFFFF fill, #000000 text, 14px/500, 4px radius, padding 23px 28px.
- **button-ghost (“PRODUCTS”):** transparent fill, #000000 text, 16px/400, padding 0px.
- **input-field (“Start your search here”):** #FFFFFF33 fill, #FFFFFF text, 16px/400, 8px radius, padding 0px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #2F2F2F.
- Do keep text in 2 levels: #FFFFFF, #898989.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #000000.
- Do set headlines in Clarkson with tight tracking (-0.06em).
- Do keep spacing on the 4px grid.
- Do use 8px corners on most elements; larger surfaces also use 100px, 4px and 30px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Clarkson, Clarkson Serif and sans-serif.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.5s, 0.35s. Longer ambient animations run 1.2s.

- **Easing:** `cubic-bezier(0.645, 0.045, 0.355, 1)`, `linear`, `cubic-bezier(0.23, 1, 0.32, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/squarespace.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
