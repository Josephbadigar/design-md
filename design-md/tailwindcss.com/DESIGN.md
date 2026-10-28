---
version: alpha
name: Tailwind CSS
description: "Dark interface measured from tailwindcss.com: inter type, vivid cyan accents, flat surfaces and 4px corners."
colors:
  background: "#030712"
  surface: "#030712"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#CAD5E2"
  on-surface-muted: "#99A1AF"
  on-surface-subtle: "#90A1B9"
  overlay: "#FFFFFF1A"
  overlay-strong: "#FFFFFF33"
  outline: "#74D4FF4D"
  primary: "#00BCFF"
  on-primary: "#000000"
  inverse-surface: "#364153"
  secondary: "#FB64B6"
  tertiary: "#74D4FF"
typography:
  headline-display:
    fontFamily: inter
    fontSize: 96px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: inter
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.05em
  body-md:
    fontFamily: inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: inter
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.56
  body-sm:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 2
  label-md:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 2
  label-sm:
    fontFamily: inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.67
  code:
    fontFamily: plexMono
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.85
  headline-display-mobile:
    fontFamily: inter
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.05em
rounded:
  sm: 4px
  md: 8px
  lg: 16px
  xl: 32px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 36px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 8px 16px
    height: 40px
  button-primary-hover:
    backgroundColor: "#4A5565"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 2px 6px 2px 10px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Tailwind CSS Design System

## Overview

Tailwind CSS describes itself as: “Tailwind CSS is a utility-first CSS framework for rapidly building modern websites without ever leaving your HTML.” The interface is dark, built on **Near Black (#030712)** with **White (#FFFFFF)** text, and **Vivid Cyan (#00BCFF)** as the main accent.

Type is set in **inter**, with **plexMono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [tailwindcss.com](https://tailwindcss.com/) on October 21, 2026 at 1440×900 and 390×844 from 359 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Near Black (#030712):** Page background, seen 3 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 35 times. Token `on-surface`.
- **Light Blue (#CAD5E2):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Blue (#99A1AF):** Muted text and metadata, seen 3 times. Token `on-surface-muted`.
- **Blue (#90A1B9):** Subtle text and placeholders, seen 32 times. Token `on-surface-subtle`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 23 times. Token `overlay`.
- **White 20% (#FFFFFF33):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Light Cyan 30% (#74D4FF4D):** Borders and dividers, seen 1 time. Token `outline`.
- **Vivid Cyan (#00BCFF):** Brand color in the logo, seen 5 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#364153):** High-contrast fills, seen 2 times. Token `inverse-surface`.
- **Pink (#FB64B6):** Most used accent color, seen 15 times. Token `secondary`.
- **Light Cyan (#74D4FF):** Most used accent color, seen 11 times. Token `tertiary`.

## Typography

**inter** and **plexMono** (monospace) share the interface. Fallback stack: `inter, inter Fallback, system-ui`. Other loaded fonts: inter Fallback.

- **headline-display:** inter 96px at weight 400, line height 1, tracking -0.05em (36px on mobile). Page title (h1).
- **headline-lg:** inter 40px at weight 500, line height 1, tracking -0.05em. Section headings (h2).
- **body-md:** inter 16px at weight 400, line height 1.5. Body text.
- **body-lg:** inter 18px at weight 500, line height 1.56. Lead paragraphs.
- **body-sm:** inter 14px at weight 400, line height 2. Secondary and small text.
- **label-md:** inter 14px at weight 600, line height 2. Buttons, navigation and labels.
- **label-sm:** inter 12px at weight 400, line height 1.67. Small labels and badges.
- **code:** plexMono 13px at weight 400, line height 1.85. Code and technical values.

## Layout

Spacing follows a 4px grid: 96% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 36px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 600px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.999994 0.0000455678 0.0000200868 / 0.05) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.999994 0.0000455678 0.0000200868 / 0.02) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.999994 0.0000455678 0.0000200868 / 0.15) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 20 elements.
- **xl (32px):** 10 elements.
- **lg (16px):** 6 elements.
- **md (8px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #364153 fill, #FFFFFF text, 14px/600, 32px radius, padding 8px 16px.
- **button-primary-hover:** background #4A5565, text #FFFFFF on hover.
- **button-ghost (“v4.3”):** transparent fill, #FFFFFF text, 12px/500, 16px radius, padding 2px 6px 2px 10px.
- **input-field:** transparent fill, #FFFFFF text, 16px/400, padding 0px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #030712 for the page.
- Do keep text in 4 levels: #FFFFFF, #CAD5E2, #99A1AF, #90A1B9.
- Do use #00BCFF as the brand accent: header, logo and key highlights.
- Do set headlines in inter with tight tracking (-0.05em).
- Do keep spacing on the 4px grid.
- Do use 4px corners on most elements; larger surfaces also use 32px, 16px and 8px.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond inter and plexMono.
- Don't use #00BCFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/tailwindcss.com/), the free DESIGN.md generator.
