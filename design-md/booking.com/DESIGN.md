---
version: alpha
name: Booking.com
description: "Light interface measured from booking.com: Avenir Next type with system-ui, dark blue accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1A1A1A"
  on-background: "#1A1A1A"
  on-surface-variant: "#595959"
  surface-container-low: "#F5F5F5"
  surface-container: "#E7E7E7"
  outline: "#E7E7E7"
  primary: "#003B95"
  on-primary: "#FFFFFF"
  secondary: "#006CE4"
  tertiary: "#FFB700"
typography:
  headline-display:
    fontFamily: Avenir Next
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.33
  body-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-sm:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
rounded:
  sm: 4px
  md: 8px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.sm}"
    padding: 4px 24px
    height: 51px
  button-primary-hover:
    backgroundColor: "#0057B8"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.secondary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 4px 12px
    height: 36px
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 11px 16px
    height: 44px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 8px
  link:
    textColor: "{colors.on-surface}"
---

# Booking.com Design System

## Overview

Booking.com describes itself as: “Explore the world with Booking.com. Big savings on homes, hotels, flights, car rentals, taxis, and attractions – build your perfect trip on any budget.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1A1A1A)** text, and **Dark Blue (#003B95)** as the main accent.

Type is set in **Avenir Next** and **system-ui**. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 4px.

Measured from [booking.com](https://www.booking.com/) on October 21, 2026 at 1440×900 and 390×844 from 416 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 10 times. Token `background`.
- **Charcoal (#1A1A1A):** Primary text and headings, seen 107 times. Token `on-surface`.
- **Slate (#595959):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Snow (#F5F5F5):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Mist (#E7E7E7):** Cards and panels, seen 36 times. Token `surface-container`.
- **Mist (#E7E7E7):** Borders and dividers, seen 1 time. Token `outline`.
- **Dark Blue (#003B95):** Brand color on large areas, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#006CE4):** Secondary buttons, seen 52 times. Token `secondary`.
- **Vivid Amber (#FFB700):** Brand color on large areas, seen 17 times. Token `tertiary`.

## Typography

**Avenir Next** and **system-ui** share the interface. Fallback stack: `Avenir Next, BlinkMacSystemFont, -apple-system, Segoe UI`.

- **headline-display:** Avenir Next 24px at weight 700, line height 1.33. Page title (h1).
- **body-md:** system-ui 14px at weight 400, line height 1.43. Body text.
- **body-sm:** system-ui 12px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** system-ui 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** system-ui 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (76% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F5F5F5 → #E7E7E7) and #E7E7E7 borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 204 elements.
- **full (9999px):** 52 elements.
- **md (8px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Search”):** #006CE4 fill, #FFFFFF text, 20px/500, 4px radius, padding 4px 24px.
- **button-primary-hover:** background #0057B8, text #FFFFFF on hover.
- **button-outline (“Register”):** #FFFFFF fill, #006CE4 text, 14px/500, 4px radius, padding 4px 12px.
- **button-ghost (“Stays”):** #FFFFFF fill, #FFFFFF text, 14px/500, 9999px radius, padding 11px 16px, border 1px solid #FFFFFF.
- **input-field (“Family-friendly apartments in Pa”):** transparent fill, #1A1A1A text, 14px/500, 4px radius, padding 0px 8px.
- **link:** transparent fill, #1A1A1A text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5F5F5, #E7E7E7.
- Do keep text in 2 levels: #1A1A1A, #595959.
- Do use #003B95 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 8px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Avenir Next and system-ui.
- Don't use #003B95 for large backgrounds or body text.
- Don't make interface transitions slower than 0.00001s.

## Motion

Interface transitions are quick: 1e-05s.

- **Easing:** `ease`, `cubic-bezier(0.2, 0, 0.4, 0.8)`, `ease-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/booking.com/), the free DESIGN.md generator.
