---
version: alpha
name: Blender
description: "Dark interface measured from blender.org: Inter type, vivid blue accents, flat surfaces and 12px corners."
colors:
  background: "#292D32"
  surface: "#292D32"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#ABB2BA"
  on-surface-muted: "#737E8C"
  overlay: "#FFFFFF1A"
  primary: "#0099FF"
  on-primary: "#4C4D52"
  inverse-surface: "#F2F2F3"
  secondary: "#46EBC2"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 72px
    fontWeight: 800
    lineHeight: 1.3
  headline-lg:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.14
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.71
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 50.5px
    fontWeight: 800
    lineHeight: 1.3
rounded:
  sm: 6px
  md: 12px
spacing:
  base: 8px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    padding: 0px 8px
    height: 64px
  button-secondary:
    backgroundColor: "#FFFFFFE6"
    textColor: "#000000"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 4px 48px
    height: 40px
  button-tertiary:
    backgroundColor: "#EAEDF0"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 4px 16px
    height: 32px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Blender Design System

## Overview

Blender describes itself as: “The Freedom to Create” The interface is dark, built on **Cool Graphite (#292D32)** with **White (#FFFFFF)** text, and **Vivid Blue (#0099FF)** as the main accent.

Type is set in **Inter**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 12px.

Measured from [blender.org](https://www.blender.org/) on November 4, 2026 at 1440×900 and 390×844 from 209 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles, plus gradient stops #6183FF, #47AAF5, #020381, #2874FC.

- **Cool Graphite (#292D32):** Page background, seen 2 times. Token `background`, CSS `--color-bg-alt`.
- **White (#FFFFFF):** Primary text and headings, seen 11 times. Token `on-surface`, CSS `--navbar-bg`.
- **Cool Gray (#ABB2BA):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Cool Slate (#737E8C):** Muted text and metadata, seen 25 times. Token `on-surface-muted`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Vivid Blue (#0099FF):** Primary buttons and calls to action, seen 4 times. Token `primary`.
- **Cool Slate (#4C4D52):** Text and icons on primary. Token `on-primary`.
- **Mist (#F2F2F3):** High-contrast fills, seen 8 times. Token `inverse-surface`, CSS `--color-bg`.
- **Vivid Teal (#46EBC2):** Accent, seen 1 time. Token `secondary`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, -apple-system, BlinkMacSystemFont, Segoe UI`. Other loaded fonts: fontutti.

- **headline-display:** Inter 72px at weight 800, line height 1.3 (50.5px on mobile). Page title (h1).
- **headline-lg:** Inter 28px at weight 600, line height 1.14. Section headings (h2).
- **body-md:** Inter 14px at weight 400, line height 1.71. Body text.
- **body-lg:** Inter 18px at weight 400, line height 1.56. Lead paragraphs.
- **label-md:** Inter 14px at weight 600, line height 1.71. Buttons, navigation and labels.

## Layout

Spacing follows a 8px grid: 93% of measured gaps and paddings are multiples of 8px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 240px, 241px, 480px, 481px, 576px, 767px, 768px, 899.98px, 900px, 979.98px, 980px, 992px, 1219.98px, 1220px, 1320px, 1379.98px, 1380px, 1679.98px, 1680px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(149, 157, 165, 0.2) 0px 8px 24px 0px`
- `rgba(0, 82, 255, 0.1) 2px 4px 4px 0px, rgba(0, 82, 255, 0.1) 1px 16px 24px 0px, rgba(0, 82, 255, 0.3) 2px 8px 32px 0px`
- `rgba(0, 82, 255, 0.1) 2px 4px 4px 0px, rgba(0, 82, 255, 0.1) 1px 8px 24px 0px, rgba(0, 82, 255, 0.55) 2px 8px 48px 0px`

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **md (12px):** 124 elements.
- **sm (6px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Roadmap”):** #0099FF fill, #4C4D52 text, 14px/400, 50% radius, padding 0px 8px.
- **button-secondary (“What's Coming”):** #FFFFFFE6 fill, #000000 text, 18px/500, 6px radius, padding 4px 48px.
- **button-tertiary (“Donate”):** #EAEDF0 fill, #FFFFFF text, 14px/500, 6px radius, padding 4px 16px, shadow `rgba(0, 82, 255, 0.1) 2px 4px 4px 0px, rgba(0, 82, 255, 0.1) 1px 16px 24px 0px, rgba(0, 82, 255, 0.3) 2px 8px 32px 0px`.
- **link:** transparent fill, #737E8C text, padding 0px.

## Do's and Don'ts

- Do use #292D32 for the page.
- Do keep text in 3 levels: #FFFFFF, #ABB2BA, #737E8C.
- Do reserve #0099FF for primary actions and key highlights.
- Do keep spacing on the 8px grid.
- Do use 12px corners on most elements; larger surfaces also use 6px.
- Don't use #737E8C for body text; it reaches 3.36:1 on #292D32. Keep it for large text or metadata.
- Don't introduce new font families beyond Inter.
- Don't use #0099FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.08s, 0.5s. Longer ambient animations run 1s.

- **Easing:** `ease-in-out`, `ease`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/blender.org/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
