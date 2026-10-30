---
version: alpha
name: Airbnb
description: "Light interface measured from airbnb.com: Airbnb Cereal VF type, vivid red accents, tonal surfaces and 4px corners."
colors:
  background: "#F7F7F7"
  surface: "#F7F7F7"
  on-surface: "#222222"
  on-background: "#222222"
  on-surface-variant: "#6C6C6C"
  surface-container-low: "#F2F2F2"
  surface-container: "#FFFFFF"
  overlay: "#FFFFFF4D"
  primary: "#FF385C"
  on-primary: "#000000"
  secondary: "#DA1249"
  tertiary: "#0066FF"
typography:
  headline-display:
    fontFamily: Airbnb Cereal VF
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.43
  headline-lg:
    fontFamily: Airbnb Cereal VF
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.18
    letterSpacing: -0.02em
  body-md:
    fontFamily: Airbnb Cereal VF
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: Airbnb Cereal VF
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.29
rounded:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 100px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  xl: 48px
  section: 80px
  margin: 48px
  container: 1920px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    padding: 0px
    height: 40px
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.surface-container}"
    typography: "{typography.body-md}"
    rounded: 50px
    padding: 0px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Airbnb Design System

## Overview

Airbnb describes itself as: “Get an Airbnb for every kind of trip → 8 million vacation rentals → 2 million Guest Favorites → 220+ countries and regions worldwide” The interface is light, built on **Snow (#F7F7F7)** with **Charcoal (#222222)** text, and **Vivid Red (#FF385C)** as the main accent.

Type is set in **Airbnb Cereal VF**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [airbnb.com](https://www.airbnb.com/) on October 29, 2026 at 1440×900 and 390×844 from 269 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Snow (#F7F7F7):** Page background, seen 1 time. Token `background`, CSS `--palette-grey100`.
- **Charcoal (#222222):** Primary text and headings, seen 66 times. Token `on-surface`, CSS `--palette-bg-slider-track-active`.
- **Slate (#6C6C6C):** Secondary text, seen 27 times. Token `on-surface-variant`, CSS `--palette-bg-scrollbar-handle-active`.
- **Mist (#F2F2F2):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`, CSS `--palette-bg-quaternary`.
- **White (#FFFFFF):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--palette-loading-material`.
- **White 30% (#FFFFFF4D):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Vivid Red (#FF385C):** Brand accent (CSS variable), seen 1 time. Token `primary`, CSS `--palette-bg-primary-core`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Pink (#DA1249):** Secondary buttons. Token `secondary`.
- **Vivid Blue (#0066FF):** Accent, seen 3 times. Token `tertiary`.

## Typography

**Airbnb Cereal VF** carries the whole interface. Fallback stack: `Airbnb Cereal VF, Circular, -apple-system, BlinkMacSystemFont`.

- **headline-display:** Airbnb Cereal VF 28px at weight 700, line height 1.43. Page title (h1).
- **headline-lg:** Airbnb Cereal VF 22px at weight 500, line height 1.18, tracking -0.02em. Section headings (h2).
- **body-md:** Airbnb Cereal VF 14px at weight 400, line height 1.43. Body text.
- **label-md:** Airbnb Cereal VF 14px at weight 500, line height 1.29. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 63% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 16px, xl 48px.
- **Sections:** 80px vertical padding between major sections.
- **Container:** content is capped at 1920px.
- **Page margin:** 48px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.16) 0px 2px 2px 0px, rgba(255, 255, 255, 0.04) 1px 1.5px 3px 0px inset, rgba(255, 255, 255, 0.04) -1px 1.25px 3px 0px inset, rgba(255, 56, 92, 0.3) 0px -1px 3px 0px inset, rgba(0, 0, 0, 0.16) 0px -1px 2px 0px inset`
- `rgba(218, 218, 218, 0.6) 0px 0.5px 1px 0px, rgba(0, 0, 0, 0.12) 0px -0.502px 1.004px 0px, rgba(0, 0, 0, 0.04) 0px -1.5px 3.5px 0px, rgba(0, 0, 0, 0.05) 0px 3px 5px 0px, rgba(0, 0, 0, 0.2) 0px 0.75px 1px 0px inset, rgba(34, 34, 34, 0.6) 0px -0.5px 5px 1px inset, rgba(0, 0, 0, 0.16) 0.502px 0.5px 2px 0px inset, rgba(0, 0, 0, 0.12) 0px -3px 7px 0px inset, rgba(0, 0, 0, 0.05) 0.502px 2px 4px 0px inset, rgba(0, 0, 0, 0.04) 1.004px 4px 4px 0px inset, rgba(184, 72, 155, 0.2) 0px -3px 7px 0px inset`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **xs (4px):** 120 elements.
- **sm (8px):** 36 elements.
- **full (9999px):** 20 elements.
- **md (12px):** 8 elements.
- **lg (32px):** 8 elements.
- **xl (100px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Log in or sign up”):** #F2F2F2 fill, #222222 text, 14px/400, 50% radius, padding 0px.
- **button-secondary (“Search”):** #DA1249 fill, #FFFFFF text, 14px/400, 50px radius, padding 0px.
- **button-ghost (“When Add dates”):** transparent fill, #222222 text, 14px/400, 32px radius, padding 0px.
- **input-field (“Search destinations”):** transparent fill, #222222 text, 14px/500, padding 0px.
- **link:** transparent fill, #222222 text, padding 0px.

## Do's and Don'ts

- Do use #F7F7F7 for the page and lift surfaces in small steps: #F2F2F2, #FFFFFF.
- Do keep text in 2 levels: #222222, #6C6C6C.
- Do use #FF385C as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 16px).
- Do use 4px corners on most elements; larger surfaces also use 8px, 12px and 32px.
- Don't introduce new font families beyond Airbnb Cereal VF.
- Don't use #FF385C for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.1s, 0.25s, 0.2s.

- **Easing:** `cubic-bezier(0.2, 0, 0, 1)`, `cubic-bezier(0, 0, 1, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/airbnb.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
