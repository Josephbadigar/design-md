---
version: alpha
name: Lattice
description: "Light interface measured from lattice.com: Matter type, light teal accents, tonal surfaces and 14.44px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#001F1F"
  on-background: "#001F1F"
  on-surface-variant: "#003D3D"
  on-surface-muted: "#2A4E1C"
  on-surface-subtle: "#455252"
  surface-container-low: "#FAF9F7"
  surface-container: "#F7F6F2"
  surface-container-high: "#FDE5FF"
  surface-container-highest: "#EBE7E1"
  overlay: "#FFFFFFCC"
  overlay-strong: "#001F1F0A"
  outline: "#001F1F14"
  outline-variant: "#6BB85F"
  primary: "#B1F0E7"
  on-primary: "#000000"
  secondary: "#D9ADFF"
  tertiary: "#515C0B"
  success: "#046645"
  warning: "#A36A14"
typography:
  headline-display:
    fontFamily: Matter
    fontSize: 72px
    fontWeight: 500
    lineHeight: 0.9
    letterSpacing: -0.024em
  headline-lg:
    fontFamily: Matter
    fontSize: 47px
    fontWeight: 500
    lineHeight: 0.9
    letterSpacing: -0.024em
  headline-md:
    fontFamily: Matter
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.3
  body-md:
    fontFamily: Matter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.3
  body-sm:
    fontFamily: Matter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
  caption:
    fontFamily: Matter
    fontSize: 14.5px
    fontWeight: 400
    lineHeight: 1.3
  label-md:
    fontFamily: Matter
    fontSize: 14.5px
    fontWeight: 500
    lineHeight: 1
  label-sm:
    fontFamily: Matter
    fontSize: 12.5px
    fontWeight: 500
    lineHeight: 1.3
  headline-display-mobile:
    fontFamily: Matter
    fontSize: 54.5px
    fontWeight: 500
    lineHeight: 0.9
    letterSpacing: -0.024em
  headline-lg-mobile:
    fontFamily: Matter
    fontSize: 33px
    fontWeight: 500
    lineHeight: 0.9
    letterSpacing: -0.024em
rounded:
  xs: 11.55px
  sm: 14.44px
  md: 18.05px
  lg: 21.66px
  xl: 28.88px
spacing:
  xs: 3.61px
  sm: 7.22px
  md: 14.44px
  lg: 18.05px
  xl: 43.32px
  gutter: 8.66px
  section: 72.19px
  container: 1660.42px
components:
  button-primary:
    backgroundColor: "#6A7878"
    textColor: "{colors.on-surface-subtle}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xs}"
    padding: 10.11px 8.66px 10.11px 11.55px
    height: 39px
  button-primary-hover:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
  button-secondary:
    backgroundColor: "{colors.success}"
    textColor: "#CDFACE"
    typography: "{typography.label-md}"
    rounded: "{rounded.xs}"
    padding: 10.11px 17.33px
    height: 38px
  button-outline:
    backgroundColor: "#CDFACE"
    textColor: "#366625"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 8.66px 8.66px 8.66px 17.33px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: 5.12px
    padding: 0px
  card:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Lattice Design System

## Overview

Lattice describes itself as: “Join 5,000+ forward-thinking teams using Lattice’s HR and AI tools to manage people and performance — all on one trusted platform.” The interface is light, built on **White (#FFFFFF)** with **Deep Cyan (#001F1F)** text, and **Light Teal (#B1F0E7)** as the main accent.

Type is set in **Matter**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 14.44px.

Measured from [lattice.com](https://lattice.com/) on October 21, 2026 at 1440×900 and 390×844 from 346 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 19 roles, plus gradient stops #D0FF64, #52E5FF, #FBE3FF.

- **White (#FFFFFF):** Page background, seen 9 times. Token `background`, CSS `--osano-info-dialog-gpc-background-color`.
- **Deep Cyan (#001F1F):** Primary text and headings, seen 25 times. Token `on-surface`, CSS `--osano-dialog-gpc-foreground-color`.
- **Deep Cyan (#003D3D):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Deep Green (#2A4E1C):** Muted text and metadata, seen 3 times. Token `on-surface-muted`, CSS `--color--green-1000`.
- **Cool Graphite (#455252):** Subtle text and placeholders, seen 12 times. Token `on-surface-subtle`.
- **Snow (#FAF9F7):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#F7F6F2):** Cards and panels, seen 2 times. Token `surface-container`, CSS `--_theme---cards--background`.
- **Pale Purple (#FDE5FF):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Warm Mist (#EBE7E1):** Highest raised elements, seen 7 times. Token `surface-container-highest`, CSS `--color--sand-200`.
- **White 80% (#FFFFFFCC):** Translucent fill for cards and controls, seen 9 times. Token `overlay`.
- **Deep Cyan 4% (#001F1F0A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Deep Cyan 8% (#001F1F14):** Borders and dividers, seen 4 times. Token `outline`.
- **Green (#6BB85F):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Light Teal (#B1F0E7):** Brand color on large areas, seen 1 time. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Light Violet (#D9ADFF):** Brand color in the header, seen 49 times. Token `secondary`, CSS `--color--violet-200`.
- **Deep Lime (#515C0B):** Most used accent color, seen 9 times. Token `tertiary`.
- **Deep Teal (#046645):** Success and positive states, seen 8 times. Token `success`, CSS `--osano-button-background-color`.
- **Dark Orange (#A36A14):** Warnings and highlights, seen 3 times. Token `warning`.

## Typography

**Matter** carries the whole interface. Fallback stack: `Matter, sans-serif`. Other loaded fonts: Latticon.

- **headline-display:** Matter 72px at weight 500, line height 0.9, tracking -0.024em (54.5px on mobile). Page title (h1).
- **headline-lg:** Matter 47px at weight 500, line height 0.9, tracking -0.024em (33px on mobile). Section headings (h2).
- **headline-md:** Matter 22px at weight 400, line height 1.3. Sub-section headings.
- **body-md:** Matter 18px at weight 400, line height 1.3. Body text.
- **body-sm:** Matter 16px at weight 400, line height 1.3. Secondary and small text.
- **caption:** Matter 14.5px at weight 400, line height 1.3. Captions and fine print.
- **label-md:** Matter 14.5px at weight 500, line height 1. Buttons, navigation and labels.
- **label-sm:** Matter 12.5px at weight 500, line height 1.3. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 0% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.61px, sm 7.22px, md 14.44px, lg 18.05px, xl 43.32px.
- **Sections:** 72.19px vertical padding between major sections.
- **Gaps:** 8.66px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1660.42px.
- **Breakpoints:** 376px, 478px, 479px, 767px, 768px, 820px, 991px, 992px, 1200px, 1920px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 64px 64px -32px, rgba(0, 0, 0, 0) 0px 32px 32px -16px, rgba(0, 0, 0, 0) 0px 16px 16px -8px, color(srgb 0 0.121569 0.121569 / 0.04) 0px 12px 12px -6px, color(srgb 0 0.121569 0.121569 / 0.04) 0px 6px 6px -3px, color(srgb 0 0.121569 0.121569 / 0.04) 0px 3px 3px -1.5px, color(srgb 0 0.121569 0.121569 / 0.08) 0px 1px 1px -0.5px, color(srgb 0 0.121569 0.121569 / 0.04) 0px 0px 0px 1px`

## Shapes

Most elements use 14.44px corners. Measured radii, most used first:

- **sm (14.44px):** 56 elements.
- **lg (21.66px):** 52 elements.
- **xl (28.88px):** 52 elements.
- **md (18.05px):** 32 elements.
- **xs (11.55px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Platform”):** #6A7878 fill, #455252 text, 14.4384px/500, 11.5507px radius, padding 10.11px 8.66px 10.11px 11.55px.
- **button-primary-hover:** background #FAF9F7, text #001F1F on hover.
- **button-secondary (“Request a demo”):** #046645 fill, #CDFACE text, 14.4384px/500, 11.5507px radius, padding 10.11px 17.33px.
- **button-outline (“Platform overview → →”):** #CDFACE fill, #366625 text, 14.4384px/500, 28.8768px radius, padding 8.66px 8.66px 8.66px 17.33px.
- **button-ghost (“Close this consent banner”):** transparent fill, #001F1F text, 12.8px/400, 5.12px radius, padding 0px.
- **card:** #B1F0E7 fill, #003D3D text, 18.048px/400, 21.6576px radius, padding 0px.
- **link:** transparent fill, #001F1F text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAF9F7, #F7F6F2, #FDE5FF, #EBE7E1.
- Do keep text in 4 levels: #001F1F, #003D3D, #2A4E1C, #455252.
- Do use #B1F0E7 as the brand accent: header, logo and key highlights.
- Do set headlines in Matter with tight tracking (-0.024em).
- Do reuse the measured spacing steps (7.22px, 14.44px, 18.05px).
- Do use 14.44px corners on most elements; larger surfaces also use 21.66px, 28.88px and 18.05px.
- Don't introduce new font families beyond Matter.
- Don't use #B1F0E7 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.5s, 0.2s, 0.24s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0.165, 0.84, 0.44, 1)`, `cubic-bezier(0.215, 0.61, 0.355, 1)`, `cubic-bezier(0.23, 1, 0.32, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/lattice.com/), the free DESIGN.md generator.
