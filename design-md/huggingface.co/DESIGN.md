---
version: alpha
name: Hugging Face
description: "Dark monochrome interface measured from huggingface.co: Source Sans Pro type, tonal surfaces and 8px corners."
colors:
  background: "#0B0F19"
  surface: "#0B0F19"
  on-surface: "#E5E7EB"
  on-background: "#E5E7EB"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#D1D5DC"
  on-surface-muted: "#99A1AF"
  surface-container-low: "#101828"
  overlay: "#10182899"
  overlay-strong: "#FFFFFF1A"
  outline: "#141C2E"
  outline-variant: "#1E2939"
  primary: "#E5E7EB"
  on-primary: "#000000"
  secondary: "#2B7FFF"
  warning: "#FE9A00"
typography:
  headline-display:
    fontFamily: Source Sans Pro
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1
  headline-lg:
    fontFamily: Source Sans Pro
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.2
  headline-md:
    fontFamily: Source Sans Pro
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
  headline-sm:
    fontFamily: Source Sans Pro
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.25
  body-md:
    fontFamily: Source Sans Pro
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Source Sans Pro
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-sm:
    fontFamily: Source Sans Pro
    fontSize: 13.5px
    fontWeight: 400
    lineHeight: 1.37
  label-md:
    fontFamily: Source Sans Pro
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.25
  label-sm:
    fontFamily: Source Sans Pro
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  code:
    fontFamily: IBM Plex Mono
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
  headline-display-mobile:
    fontFamily: Source Sans Pro
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.11
rounded:
  sm: 6px
  md: 8px
  lg: 25.6px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
components:
  button-primary:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    padding: 0px 21.6px
    height: 42px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    padding: 4px 12px
    height: 30px
  button-outline-hover:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.on-primary}"
  card:
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.primary}"
---

# Hugging Face Design System

## Overview

Hugging Face describes itself as: “We’re on a journey to advance and democratize artificial intelligence through open source and open science.” The interface is dark, built on **Cool Charcoal (#0B0F19)** with **Cool Mist (#E5E7EB)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Source Sans Pro**, with **IBM Plex Mono** for code. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [huggingface.co](https://huggingface.co/) on October 21, 2026 at 1440×900 and 390×844 from 457 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #101828, #E17100, #E60076, #155DFC.

- **Cool Charcoal (#0B0F19):** Page background, seen 3 times. Token `background`.
- **Cool Mist (#E5E7EB):** Primary text and headings, seen 54 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 21 times. Token `on-surface-strong`, CSS `--color-white`.
- **Cool Silver (#D1D5DC):** Secondary text, seen 26 times. Token `on-surface-variant`.
- **Blue (#99A1AF):** Muted text and metadata, seen 37 times. Token `on-surface-muted`.
- **Deep Blue (#101828):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`.
- **Deep Blue 60% (#10182899):** Translucent fill for cards and controls, seen 12 times. Token `overlay`.
- **White 10% (#FFFFFF1A):** Stronger translucent fill, seen 6 times. Token `overlay-strong`.
- **Deep Blue (#141C2E):** Borders and dividers, seen 38 times. Token `outline`.
- **Deep Blue (#1E2939):** Secondary dividers, seen 13 times. Token `outline-variant`.
- **Cool Mist (#E5E7EB):** Primary actions (the main text color; the palette is monochrome), seen 54 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#2B7FFF):** Accent, seen 3 times. Token `secondary`.
- **Vivid Orange (#FE9A00):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**Source Sans Pro** and **IBM Plex Mono** (monospace) share the interface. Fallback stack: `Source Sans Pro, -apple-system, BlinkMacSystemFont, Segoe UI`.

- **headline-display:** Source Sans Pro 48px at weight 700, line height 1 (36px on mobile). Page title (h1).
- **headline-lg:** Source Sans Pro 30px at weight 700, line height 1.2. Section headings (h2).
- **headline-md:** Source Sans Pro 24px at weight 600, line height 1.33. Sub-section headings.
- **headline-sm:** Source Sans Pro 20px at weight 700, line height 1.25. Card and feature titles.
- **body-md:** Source Sans Pro 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Source Sans Pro 18px at weight 400, line height 1.56. Lead paragraphs.
- **body-sm:** Source Sans Pro 13.5px at weight 400, line height 1.37. Secondary and small text.
- **label-md:** Source Sans Pro 16px at weight 600, line height 1.25. Buttons, navigation and labels.
- **label-sm:** Source Sans Pro 14px at weight 600, line height 1.43. Small labels and badges.
- **code:** IBM Plex Mono 15px at weight 400, line height 1.6. Code and technical values.

## Layout

Spacing does not follow a strict grid: 61% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 12px, lg 24px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 20px 25px -5px, rgba(0, 0, 0, 0.1) 0px 8px 10px -6px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 2px 4px 0px inset`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 132 elements.
- **lg (25.6px):** 48 elements.
- **sm (6px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Explore AI Apps”):** transparent fill, #FFFFFF text, 16px/400, 3.35544e+07px radius, padding 0px 21.6px, border 1px solid #4A5565, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 20px 25px -5px, rgba(0, 0, 0, 0.1) 0px 8px 10px -6px`.
- **button-outline (“Sign Up”):** #101828 fill, #FFFFFF text, 16px/400, 3.35544e+07px radius, padding 4px 12px, border 1px solid #141C2E.
- **button-outline-hover:** background #FFFFFF, text #000000 on hover.
- **card:** transparent fill, 16px/400, 8px radius, padding 0px, border 1px solid #141C2E, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`.
- **link:** transparent fill, #E5E7EB text, padding 0px.

## Do's and Don'ts

- Do use #0B0F19 for the page and lift surfaces in small steps: #101828.
- Do keep text in 4 levels: #E5E7EB, #FFFFFF, #D1D5DC, #99A1AF.
- Do let contrast carry emphasis; primary actions use #E5E7EB on #0B0F19.
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 25.6px and 6px.
- Don't introduce new font families beyond Source Sans Pro and IBM Plex Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/huggingface.co/), the free DESIGN.md generator.
