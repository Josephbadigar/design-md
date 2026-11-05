---
version: alpha
name: Godot
description: "Dark interface measured from godotengine.org: Montserrat type with system-ui, light red accents, flat surfaces and 7px corners."
colors:
  background: "#333F67"
  surface: "#333F67"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#F5F5F7"
  on-surface-muted: "#DEE0E7"
  on-surface-subtle: "#B0C4DE"
  overlay: "#6F6F6F45"
  overlay-strong: "#818181A8"
  primary: "#F57389"
  on-primary: "#000000"
  secondary: "#1F3C5E"
  tertiary: "#3E8ECC"
typography:
  headline-display:
    fontFamily: Montserrat
    fontSize: 60px
    fontWeight: 800
  headline-lg:
    fontFamily: Montserrat
    fontSize: 36px
    fontWeight: 800
  headline-md:
    fontFamily: Montserrat
    fontSize: 28px
    fontWeight: 400
  headline-sm:
    fontFamily: Montserrat
    fontSize: 25px
    fontWeight: 800
  title-lg:
    fontFamily: Montserrat
    fontSize: 22px
    fontWeight: 800
  body-md:
    fontFamily: system-ui
    fontSize: 18px
    fontWeight: 400
  body-sm:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: system-ui
    fontSize: 15px
    fontWeight: 300
  headline-display-mobile:
    fontFamily: Montserrat
    fontSize: 40px
    fontWeight: 800
  title-lg-mobile:
    fontFamily: Montserrat
    fontSize: 19px
    fontWeight: 800
rounded:
  sm: 7px
  md: 10px
  lg: 12px
spacing:
  sm: 5px
  md: 16px
  lg: 17px
  xl: 64px
  gutter: 20px
  section: 64px
  container: 1200px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px
    height: 54px
  button-secondary:
    backgroundColor: "{colors.overlay-strong}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 16px 32px
    height: 54px
  button-tertiary:
    backgroundColor: "{colors.on-surface}"
    textColor: "#546B99"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 16px 32px
    height: 54px
  card:
    backgroundColor: "{colors.on-surface}"
    textColor: "#3689C9"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 17px
  link:
    textColor: "#2C2C2C"
---

# Godot Design System

## Overview

Godot describes itself as: “Godot provides a huge set of common tools, so you can just focus on making your game without reinventing the wheel.” The interface is dark, built on **Dark Blue (#333F67)** with **White (#FFFFFF)** text, and **Light Red (#F57389)** as the main accent.

Type is set in **Montserrat** and **system-ui**. Headlines run large; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 7px.

Measured from [godotengine.org](https://godotengine.org/) on November 4, 2026 at 1440×900 and 390×844 from 241 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Dark Blue (#333F67):** Page background, seen 2 times. Token `background`, CSS `--navbar-link-color`.
- **White (#FFFFFF):** Primary text and headings, seen 20 times. Token `on-surface`, CSS `--primary-color-text-hl`.
- **Snow (#F5F5F7):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Cool Mist (#DEE0E7):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Light Blue (#B0C4DE):** Subtle text and placeholders, seen 8 times. Token `on-surface-subtle`, CSS `--dark-color-text`.
- **Slate 27% (#6F6F6F45):** Translucent fill for cards and controls, seen 5 times. Token `overlay`.
- **Gray 66% (#818181A8):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Light Red (#F57389):** Brand accent (CSS variable). Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#1F3C5E):** Accent (CSS variable). Token `secondary`.
- **Blue (#3E8ECC):** Accent in text, fills and borders. Token `tertiary`.

## Typography

**Montserrat** and **system-ui** share the interface. Fallback stack: `Montserrat, sans-serif`. Other loaded fonts: montserrat.

- **headline-display:** Montserrat 60px at weight 800 (40px on mobile). Page title (h1).
- **headline-lg:** Montserrat 36px at weight 800. Section headings (h2).
- **headline-md:** Montserrat 28px at weight 400. Sub-section headings.
- **headline-sm:** Montserrat 25px at weight 800. Card and feature titles.
- **title-lg:** Montserrat 22px at weight 800 (19px on mobile). Small titles.
- **body-md:** system-ui 18px at weight 400. Body text.
- **body-sm:** system-ui 16px at weight 400, line height 1.5. Secondary and small text.
- **caption:** system-ui 15px at weight 300. Captions and fine print.

## Layout

Spacing does not follow a strict grid: 45% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 5px, md 16px, lg 17px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1200px.
- **Breakpoints:** 500px, 650px, 720px, 768px, 900px, 1020px, 1200px, 1250px, 1400px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.2) 0px 0px 4px 0px`

Hairline rings and inset highlights also appear: `rgb(243, 87, 116) 0px 0px 0px 2px inset`.

## Shapes

Most elements use 7px corners. Measured radii, most used first:

- **sm (7px):** 92 elements.
- **lg (12px):** 44 elements.
- **md (10px):** 32 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Download Latest 4.7.2”):** #FFFFFF fill, #333F67 text, 18px/800, 12px radius, padding 0px, shadow `rgba(0, 0, 0, 0.2) 0px 0px 4px 0px`.
- **button-secondary (“What's new”):** #818181A8 fill, #FFFFFF text, 18px/800, 12px radius, padding 16px 32px, shadow `rgba(0, 0, 0, 0.2) 0px 0px 4px 0px`.
- **button-tertiary (“More news”):** #FFFFFF fill, #546B99 text, 18px/800, 12px radius, padding 16px 32px, shadow `rgba(0, 0, 0, 0.2) 0px 0px 4px 0px`.
- **card:** #FFFFFF fill, #3689C9 text, 18px/400, 7px radius, padding 17px.
- **link:** transparent fill, #2C2C2C text, padding 0px.

## Do's and Don'ts

- Do use #333F67 for the page.
- Do keep text in 4 levels: #FFFFFF, #F5F5F7, #DEE0E7, #B0C4DE.
- Do use #F57389 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (5px, 16px, 17px).
- Do use 7px corners on most elements; larger surfaces also use 12px and 10px.
- Don't introduce new font families beyond Montserrat and system-ui.
- Don't use #F57389 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.1s, 0.5s.

- **Easing:** `ease-in-out`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/godotengine.org/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
