---
version: alpha
name: Ableton
description: "Light interface measured from ableton.com: futura-pt type, vivid indigo accents, tonal surfaces and square corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  surface-container-low: "#F3F3F3"
  surface-container: "#EEEEEE"
  outline: "#EEEEEE"
  primary: "#0000FF"
  on-primary: "#000000"
  secondary: "#00D2BE"
  tertiary: "#FF8389"
typography:
  display-hero:
    fontFamily: futura-pt
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.2
  headline-display:
    fontFamily: futura-pt
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.4
  headline-lg:
    fontFamily: futura-pt
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.5
  headline-md:
    fontFamily: futura-pt
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.5
  body-md:
    fontFamily: futura-pt
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: futura-pt
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: futura-pt
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
  label-sm:
    fontFamily: futura-pt
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: futura-pt
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.5
  headline-md-mobile:
    fontFamily: futura-pt
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
rounded:
  none: 0px
spacing:
  xs: 2.8px
  sm: 5px
  md: 10px
  lg: 18px
  xl: 60px
  section: 60px
  margin: 120px
  container: 1600px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.none}"
    padding: 0px
    height: 60px
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.none}"
    padding: 1.96px 11.9px
    height: 25px
  button-tertiary:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.none}"
    padding: 1.96px 11.9px
    height: 25px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-md}"
    rounded: "{rounded.none}"
    padding: 0px
  input-field:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-md}"
    rounded: "{rounded.none}"
    padding: 8px 15px
  link:
    textColor: "{colors.on-surface}"
---

# Ableton Design System

## Overview

Ableton describes itself as: “Ableton makes software, hardware and other creative tools for a global community of music makers.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Indigo (#0000FF)** as the main accent.

Type is set in **futura-pt**. Headlines run large; body text is 16px. The surface language is flat. Corners are square.

Measured from [ableton.com](https://www.ableton.com/) on November 4, 2026 at 1440×900 and 390×844 from 179 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 59 times. Token `on-surface`.
- **Mist (#F3F3F3):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Mist (#EEEEEE):** Cards and panels, seen 4 times. Token `surface-container`.
- **Mist (#EEEEEE):** Borders and dividers, seen 1 time. Token `outline`.
- **Vivid Indigo (#0000FF):** Primary buttons and calls to action, seen 20 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Teal (#00D2BE):** Secondary buttons, seen 2 times. Token `secondary`.
- **Light Red (#FF8389):** Secondary buttons, seen 1 time. Token `tertiary`.

## Typography

**futura-pt** carries the whole interface. Fallback stack: `futura-pt, Avenir, -apple-system, BlinkMacSystemFont`.

- **display-hero:** futura-pt 40px at weight 700, line height 1.2. Oversized hero statements.
- **headline-display:** futura-pt 30px at weight 700, line height 1.4 (20px on mobile). Page title (h1).
- **headline-lg:** futura-pt 24px at weight 700, line height 1.5. Section headings (h2).
- **headline-md:** futura-pt 20px at weight 700, line height 1.5 (14px on mobile). Sub-section headings.
- **body-md:** futura-pt 16px at weight 400, line height 1.5. Body text.
- **body-sm:** futura-pt 14px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** futura-pt 16px at weight 700, line height 1.5. Buttons, navigation and labels.
- **label-sm:** futura-pt 14px at weight 700, line height 1.5. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 19% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2.8px, sm 5px, md 10px, lg 18px, xl 60px.
- **Sections:** 60px vertical padding between major sections.
- **Container:** content is capped at 1600px.
- **Page margin:** 120px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F3F3F3 → #EEEEEE) and #EEEEEE borders.

## Shapes

Corners are square. Measured radii, most used first:

- **none (0px):** measured.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Scroll down”):** #0000FF fill, #000000 text, 16px/400, padding 0px.
- **button-secondary (“View posts in category: Tutorial”):** #00D2BE fill, #000000 text, 14px/700, padding 1.96px 11.9px.
- **button-tertiary (“View posts in category: Download”):** #FF8389 fill, #000000 text, 14px/700, padding 1.96px 11.9px.
- **button-ghost (“More”):** transparent fill, #000000 text, 20px/700, padding 0px.
- **input-field (“Email Address”):** #EEEEEE fill, #000000 text, 20px/400, padding 8px 15px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F3F3F3, #EEEEEE.
- Do reserve #0000FF for primary actions and key highlights.
- Do reuse the measured spacing steps (5px, 10px, 18px).
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond futura-pt.
- Don't use #0000FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.35s.

## Motion

Interface transitions are quick: 0.15s, 0.35s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/ableton.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
