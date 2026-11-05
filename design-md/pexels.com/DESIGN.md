---
version: alpha
name: Pexels
description: "Light monochrome interface measured from pexels.com: Canva Sans type, tonal surfaces and 12px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#191919"
  on-background: "#191919"
  on-surface-strong: "#000000"
  on-surface-variant: "#393939"
  on-surface-muted: "#A8A8A8"
  surface-container-low: "#CDCDCD"
  surface-container: "#B2C0C3"
  outline: "#EDEDED"
  primary: "#000000"
  on-primary: "#FFFFFF"
  secondary: "#0000EE"
typography:
  headline-display:
    fontFamily: Canva Sans
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.042em
  headline-lg:
    fontFamily: Canva Sans
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: -0.063em
  body-md:
    fontFamily: Canva Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
  body-lg:
    fontFamily: Canva Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.031em
  label-md:
    fontFamily: Canva Sans
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.029em
  headline-display-mobile:
    fontFamily: Canva Sans
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.04em
rounded:
  sm: 12px
  md: 30px
  lg: 100px
  xl: 180px
spacing:
  xs: 2px
  sm: 8px
  md: 15px
  lg: 20px
  xl: 40px
  gutter: 8px
  section: 452px
  margin: 30px
  container: 1600px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 20px
    height: 48px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 12px 11px 12px 16px
    height: 48px
  button-outline-hover:
    backgroundColor: "{colors.outline}"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 1px 20px
    height: 48px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 0px
  input-field:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 1px 2px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: 24px
    padding: 16px 20px
  link:
    textColor: "{colors.secondary}"
---

# Pexels Design System

## Overview

Pexels describes itself as: “Free stock photos & videos you can use everywhere. Browse millions of high-quality royalty free stock images & copyright free pictures. No attribution required.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#191919)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Canva Sans**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 12px.

Measured from [pexels.com](https://www.pexels.com/) on November 4, 2026 at 1440×900 and 390×844 from 367 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 5 times. Token `background`.
- **Charcoal (#191919):** Primary text and headings, seen 39 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 4 times. Token `on-surface-strong`.
- **Graphite (#393939):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Gray (#A8A8A8):** Muted text and metadata, seen 39 times. Token `on-surface-muted`.
- **Silver (#CDCDCD):** Raised areas one step from the page, seen 8 times. Token `surface-container-low`.
- **Cool Silver (#B2C0C3):** Cards and panels, seen 1 time. Token `surface-container`.
- **Mist (#EDEDED):** Borders and dividers, seen 56 times. Token `outline`.
- **Near Black (#000000):** Primary buttons and calls to action, seen 6 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#0000EE):** Links and interactive text. Token `secondary`.

## Typography

**Canva Sans** carries the whole interface. Fallback stack: `Canva Sans, Helvetica Neue, Roboto, -apple-system`.

- **headline-display:** Canva Sans 48px at weight 700, line height 1.1, tracking -0.042em (40px on mobile). Page title (h1).
- **headline-lg:** Canva Sans 24px at weight 700, line height 1.3, tracking -0.063em. Section headings (h2).
- **body-md:** Canva Sans 14px at weight 400, line height 1.4. Body text.
- **body-lg:** Canva Sans 16px at weight 400, line height 1.5, tracking -0.031em, capitalize. Lead paragraphs.
- **label-md:** Canva Sans 17px at weight 400, line height 1, tracking -0.029em. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 66% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 15px, lg 20px, xl 40px.
- **Sections:** 452px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1600px.
- **Page margin:** 30px on each side of full-width sections.
- **Breakpoints:** 379px, 439px, 450px, 650px, 651px, 900px, 901px, 960px, 1249px, 1250px, 1440px, 1441px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#CDCDCD → #B2C0C3) and #EDEDED borders.

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **sm (12px):** 188 elements.
- **xl (180px):** 144 elements.
- **lg (100px):** 64 elements.
- **md (30px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Home”):** #000000 fill, #FFFFFF text, 17px/400, 30px radius, padding 0px 20px.
- **button-primary-hover:** background #191919, text #FFFFFF on hover.
- **button-outline (“Photos”):** #FFFFFF fill, #000000 text, 17px/400, 12px radius, padding 12px 11px 12px 16px.
- **button-outline-hover:** background #EDEDED, text #000000 on hover.
- **button-secondary (“Join”):** #191919 fill, #FFFFFF text, 17px/400, 12px radius, padding 1px 20px, border 1px solid #191919.
- **button-ghost (“Join”):** transparent fill, #FFFFFF text, 16px/400, padding 0px.
- **input-field (“Search for free photos”):** transparent fill, #000000 text, 17px/400, padding 1px 2px.
- **card:** #FFFFFF fill, #000000 text, 14px/400, 24px radius, padding 16px 20px, border 1px solid #EDEDED.
- **link:** transparent fill, #0000EE text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #CDCDCD, #B2C0C3.
- Do keep text in 4 levels: #191919, #000000, #393939, #A8A8A8.
- Do let contrast carry emphasis; primary actions use #000000 on #FFFFFF.
- Do set headlines in Canva Sans with tight tracking (-0.042em).
- Do reuse the measured spacing steps (8px, 15px, 20px).
- Do use 12px corners on most elements; larger surfaces also use 180px, 100px and 30px.
- Don't use #A8A8A8 for body text; it reaches 2.38:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Canva Sans.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.1s, 0.2s, 0.25s, 0.005s.

- **Easing:** `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/pexels.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
