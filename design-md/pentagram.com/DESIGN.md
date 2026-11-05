---
version: alpha
name: Pentagram
description: "Light interface measured from pentagram.com: Plain type, blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#E3E4E5"
  surface: "#E3E4E5"
  on-surface: "#1A1A1A"
  on-background: "#1A1A1A"
  on-surface-strong: "#000000"
  on-surface-variant: "#767676"
  on-surface-muted: "#8C8C8C"
  surface-container-low: "#FFFFFF"
  overlay: "#00000012"
  overlay-strong: "#FFFFFF1F"
  outline: "#FFFFFF"
  primary: "#6993BB"
  on-primary: "#000000"
  inverse-surface: "#222222"
typography:
  headline-display:
    fontFamily: Plain
    fontSize: 52px
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plain
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Plain
    fontSize: 19px
    fontWeight: 500
    lineHeight: 1.32
  body-md:
    fontFamily: Plain
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.32
  label-md:
    fontFamily: Plain
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.25
  headline-md-mobile:
    fontFamily: Plain
    fontSize: 17px
    fontWeight: 500
    lineHeight: 1.47
rounded:
  md: 4px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  gutter: 12px
components:
  button-ghost:
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 11px 12px
  input-field:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.surface-container-low}"
    typography: "{typography.headline-lg}"
    rounded: 0px
    padding: 0px
  card:
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 24px 0px 0px 0px
  link:
    textColor: "{colors.on-surface}"
---

# Pentagram Design System

## Overview

Pentagram describes itself as: “Pentagram is the world’s largest independent design consultancy. The firm is owned and run by 24 partners, each of whom are leaders in their individual fields.” The interface is light, built on **Mist (#E3E4E5)** with **Charcoal (#1A1A1A)** text, and **Blue (#6993BB)** as the main accent.

Type is set in **Plain**. Headlines run large with tight negative tracking; body text is 19px. The surface language is flat. Controls are pill-shaped.

Measured from [pentagram.com](https://www.pentagram.com/) on November 5, 2026 at 1440×900 and 390×844 from 425 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Mist (#E3E4E5):** Page background. Token `background`.
- **Charcoal (#1A1A1A):** Primary text and headings, seen 105 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 2 times. Token `on-surface-strong`, CSS `--black`.
- **Slate (#767676):** Secondary text, seen 14 times. Token `on-surface-variant`, CSS `--gray-550`.
- **Gray (#8C8C8C):** Muted text and metadata, seen 4 times. Token `on-surface-muted`, CSS `--gray-450`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 32 times. Token `surface-container-low`, CSS `--tw-ring-offset-color`.
- **Near Black 7% (#00000012):** Translucent fill for cards and controls, seen 30 times. Token `overlay`.
- **White 12% (#FFFFFF1F):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White (#FFFFFF):** Borders and dividers, seen 3 times. Token `outline`, CSS `--tw-ring-offset-color`.
- **Blue (#6993BB):** Brand color in logos and imagery. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#222222):** High-contrast fills, seen 1 time. Token `inverse-surface`.

## Typography

**Plain** carries the whole interface. Fallback stack: `Plain, Arial, sans-serif`.

- **headline-display:** Plain 52px at weight 400, line height 1.05, tracking -0.02em. Page title (h1).
- **headline-lg:** Plain 32px at weight 400, line height 1.2, tracking -0.01em. Section headings (h2).
- **headline-md:** Plain 19px at weight 500, line height 1.32 (17px on mobile). Sub-section headings.
- **body-md:** Plain 19px at weight 400, line height 1.32. Body text.
- **label-md:** Plain 16px at weight 400, line height 1.25. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 93% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 374px, 599px, 600px, 666px, 799px, 800px, 1039px, 1040px, 1599px, 1800px, 1920px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF) and #FFFFFF borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (4px):** 136 elements.
- **full (9999px):** 48 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Customise”):** transparent fill, #FFFFFF text, 16px/400, 4px radius, padding 11px 12px, border 1px solid #FFFFFF.
- **input-field (“Add your email address”):** #222222 fill, #FFFFFF text, 32px/400, padding 0px.
- **card:** transparent fill, #FFFFFF text, 16px/400, padding 24px 0px 0px 0px, border 1px solid #333333.
- **link:** transparent fill, #1A1A1A text, padding 0px.

## Do's and Don'ts

- Do use #E3E4E5 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 4 levels: #1A1A1A, #000000, #767676, #8C8C8C.
- Do use #6993BB as the brand accent: header, logo and key highlights.
- Do set headlines in Plain with tight tracking (-0.02em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't use #767676 for body text; it reaches 3.57:1 on #E3E4E5. Keep it for large text or metadata.
- Don't use #8C8C8C for body text; it reaches 2.64:1 on #E3E4E5. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Plain.
- Don't use #6993BB for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.5s.

- **Easing:** `ease-in-out`, `cubic-bezier(0.25, 0.46, 0.45, 0.94)`, `cubic-bezier(0.59, 0.01, 0.28, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/pentagram.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
