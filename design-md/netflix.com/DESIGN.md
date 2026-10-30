---
version: alpha
name: Netflix
description: "Dark interface measured from netflix.com: Netflix Sans type, vivid red accents, tonal surfaces and 2px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#B3B3B3"
  on-surface-muted: "#414141"
  surface-container-low: "#232323"
  surface-container: "#2D2D2D"
  overlay: "#80808066"
  overlay-strong: "#FFFFFF1A"
  primary: "#E50914"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: Netflix Sans
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.25
  headline-lg:
    fontFamily: Netflix Sans
    fontSize: 24px
    fontWeight: 400
  headline-md:
    fontFamily: Netflix Sans
    fontSize: 20px
    fontWeight: 500
  body-md:
    fontFamily: Netflix Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Netflix Sans
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Netflix Sans
    fontSize: 16px
    fontWeight: 400
  headline-display-mobile:
    fontFamily: Netflix Sans
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.25
  headline-lg-mobile:
    fontFamily: Netflix Sans
    fontSize: 18px
    fontWeight: 400
rounded:
  sm: 2px
  md: 4px
  lg: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 34px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 4px 16px
    height: 32px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 6px 36px 6px 34px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Netflix Design System

## Overview

Netflix describes itself as: “Watch Netflix movies & TV shows online or stream right to your smart TV, game console, PC, Mac, mobile, tablet and more.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Vivid Red (#E50914)** as the main accent.

Type is set in **Netflix Sans**. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 2px.

Measured from [netflix.com](https://www.netflix.com/) on October 29, 2026 at 1440×900 and 390×844 from 266 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Near Black (#000000):** Page background, seen 2 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 39 times. Token `on-surface`.
- **Gray (#B3B3B3):** Secondary text, seen 30 times. Token `on-surface-variant`.
- **Graphite (#414141):** Muted text and metadata, seen 20 times. Token `on-surface-muted`.
- **Charcoal (#232323):** Raised areas one step from the page, seen 10 times. Token `surface-container-low`.
- **Graphite (#2D2D2D):** Cards and panels, seen 6 times. Token `surface-container`.
- **Gray 40% (#80808066):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White 10% (#FFFFFF1A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Vivid Red (#E50914):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**Netflix Sans** carries the whole interface. Fallback stack: `Netflix Sans, Helvetica Neue, Segoe UI, Roboto`.

- **headline-display:** Netflix Sans 56px at weight 700, line height 1.25 (32px on mobile). Page title (h1).
- **headline-lg:** Netflix Sans 24px at weight 400 (18px on mobile). Section headings (h2).
- **headline-md:** Netflix Sans 20px at weight 500. Sub-section headings.
- **body-md:** Netflix Sans 14px at weight 400, line height 1.5. Body text.
- **body-sm:** Netflix Sans 13px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Netflix Sans 16px at weight 400. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (82% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 34px.
- **Breakpoints:** 599.98px, 600px, 959.98px, 960px, 1279.98px, 1280px, 1600px, 1919.98px, 1920px, 2560px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#232323 → #2D2D2D).

## Shapes

Most elements use 2px corners. Measured radii, most used first:

- **sm (2px):** 88 elements.
- **lg (8px):** 84 elements.
- **md (4px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign In”):** #E50914 fill, #FFFFFF text, 14px/500, 4px radius, padding 4px 16px.
- **input-field:** transparent fill, #FFFFFF text, 16px/400, padding 6px 36px 6px 34px.
- **link:** transparent fill, #FFFFFFB3 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #232323, #2D2D2D.
- Do keep text in 3 levels: #FFFFFF, #B3B3B3, #414141.
- Do reserve #E50914 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 2px corners on most elements; larger surfaces also use 8px and 4px.
- Don't use #414141 for body text; it reaches 2.06:1 on #000000. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Netflix Sans.
- Don't use #E50914 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.25s, 0.2s, 0.4s.

- **Easing:** `cubic-bezier(0.4, 0, 0.68, 0.06)`, `ease-in-out`, `cubic-bezier(0.32, 0.94, 0.6, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/netflix.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
