---
version: alpha
name: WIRED
description: "Light interface measured from wired.com: WiredDisplay type with Apercu, purple accents, flat surfaces and 4px corners."
colors:
  background: "#E5E5E5"
  surface: "#E5E5E5"
  on-surface: "#1A1A1A"
  on-background: "#1A1A1A"
  on-surface-strong: "#000000"
  overlay: "#000000D9"
  primary: "#9320B8"
  on-primary: "#FFFFFF"
  secondary: "#C146FF"
typography:
  headline-display:
    fontFamily: WiredDisplay
    fontSize: 64px
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: -0.008em
  headline-lg:
    fontFamily: WiredDisplay
    fontSize: 58px
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: -0.009em
  headline-md:
    fontFamily: WiredDisplay
    fontSize: 26px
    fontWeight: 400
    lineHeight: 1.08
  headline-sm:
    fontFamily: Apercu
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.015em
  body-md:
    fontFamily: Apercu
    fontSize: 17px
    fontWeight: 700
    lineHeight: 1.29
    letterSpacing: -0.006em
  body-sm:
    fontFamily: Proxima Nova
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  caption:
    fontFamily: Proxima Nova
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.45
  label-md:
    fontFamily: Breve Text
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.47
    letterSpacing: 0.005em
  label-sm:
    fontFamily: Apercu
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.13
    letterSpacing: 0.019em
  code:
    fontFamily: WIRED Mono
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.23
rounded:
  md: 4px
spacing:
  xs: 4px
  sm: 8px
  md: 14.11px
  lg: 32px
  xl: 64px
  gutter: 8px
  margin: 64px
  container: 1600px
components:
  button-ghost:
    textColor: "{colors.primary}"
    typography: "{typography.code}"
    rounded: 0px
    padding: 12px 8px
  card:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 8px
  link:
    textColor: "#999999"
---

# WIRED Design System

## Overview

WIRED describes itself as: “We bring you the future as it happens. From the latest in science and technology to the big stories in business and culture, we've got you covered.” The interface is light, built on **Mist (#E5E5E5)** with **Charcoal (#1A1A1A)** text, and **Purple (#9320B8)** as the main accent.

Type is set in **WiredDisplay** and **Apercu**, with **WIRED Mono** for code. Headlines run large with tight negative tracking; body text is 17px. The surface language is flat. Corners are mostly 4px.

Measured from [wired.com](https://www.wired.com/) on October 29, 2026 at 1440×900 and 390×844 from 438 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **Mist (#E5E5E5):** Page background, seen 1 time. Token `background`.
- **Charcoal (#1A1A1A):** Primary text and headings, seen 99 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 9 times. Token `on-surface-strong`.
- **Near Black 85% (#000000D9):** Translucent fill for cards and controls, seen 15 times. Token `overlay`.
- **Purple (#9320B8):** Brand color in the logo, seen 11 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Violet (#C146FF):** Accent in text, fills and borders, seen 18 times. Token `secondary`.

## Typography

**WiredDisplay**, **Apercu**, **Proxima Nova**, **Breve Text** and **WIRED Mono** (monospace) share the interface. Fallback stack: `WiredDisplay, helvetica, sans-serif`.

- **headline-display:** WiredDisplay 64px at weight 400, line height 0.93, tracking -0.008em. Page title (h1).
- **headline-lg:** WiredDisplay 58px at weight 400, line height 0.93, tracking -0.009em. Section headings (h2).
- **headline-md:** WiredDisplay 26px at weight 400, line height 1.08. Sub-section headings.
- **headline-sm:** Apercu 20px at weight 700, line height 1.2, tracking -0.015em. Card and feature titles.
- **body-md:** Apercu 17px at weight 700, line height 1.29, tracking -0.006em. Body text.
- **body-sm:** Proxima Nova 12px at weight 400, line height 1.33. Secondary and small text.
- **caption:** Proxima Nova 11px at weight 400, line height 1.45. Captions and fine print.
- **label-md:** Breve Text 19px at weight 400, line height 1.47, tracking 0.005em. Buttons, navigation and labels.
- **label-sm:** Apercu 16px at weight 700, line height 1.13, tracking 0.019em. Small labels and badges.
- **code:** WIRED Mono 13px at weight 700, line height 1.23. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (73% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 14.11px, lg 32px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1600px.
- **Page margin:** 64px on each side of full-width sections.
- **Breakpoints:** 0px, 320px, 767px, 768px, 1023px, 1024px, 1025px, 1280px, 1600px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 60 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Menu”):** transparent fill, #9320B8 text, 13px/400, padding 12px 8px.
- **card:** #C146FF fill, #000000 text, 12px/400, padding 8px.
- **link:** transparent fill, #999999 text, padding 0px.

## Do's and Don'ts

- Do use #E5E5E5 for the page.
- Do keep text in 2 levels: #1A1A1A, #000000.
- Do use #9320B8 as the brand accent: header, logo and key highlights.
- Do set headlines in WiredDisplay with tight tracking (-0.008em).
- Do reuse the measured spacing steps (8px, 14.11px, 32px).
- Do use 4px corners on most elements.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond WiredDisplay, Apercu, Proxima Nova, Breve Text and WIRED Mono.
- Don't use #9320B8 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.1s. Longer ambient animations run 1s.

- **Easing:** `ease-in-out`, `cubic-bezier(0.37, 0, 0.63, 1)`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/wired.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
