---
version: alpha
name: TradingView
description: "Dark interface measured from tradingview.com: EuclidCircularSemibold type with system-ui, dark teal accents, tonal surfaces and 16px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#DBDBDB"
  on-surface-muted: "#8C8C8C"
  surface-container-low: "#222222"
  overlay: "#FFFFFF1A"
  overlay-strong: "#63636326"
  outline: "#FFFFFF1A"
  primary: "#06806B"
  on-primary: "#FFFFFF"
  inverse-surface: "#F2F2F2"
  secondary: "#2962FF"
  tertiary: "#FF9800"
  error: "#CC2F3C"
typography:
  headline-display:
    fontFamily: EuclidCircularSemibold
    fontSize: 56px
    fontWeight: 600
    lineHeight: 1.14
  headline-lg:
    fontFamily: system-ui
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.22
  headline-md:
    fontFamily: system-ui
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.29
  body-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
  body-lg:
    fontFamily: system-ui
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.33
  body-sm:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: EuclidCircularSemibold
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.13
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: system-ui
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.29
  headline-md-mobile:
    fontFamily: system-ui
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
rounded:
  xs: 4px
  sm: 6px
  md: 8px
  lg: 16px
  xl: 36px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 45px
  gutter: 12px
components:
  button-primary:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-md}"
    rounded: 40px
    padding: 6px
    height: 40px
  button-ghost:
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 2px 4px
  card:
    backgroundColor: "#707070"
    textColor: "#9C9C9C"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.background}"
---

# TradingView Design System

## Overview

TradingView describes itself as: “Where the world charts, chats, and trades markets. We're a supercharged super-charting platform and social network for traders and investors. Free to sign up.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Dark Teal (#06806B)** as the main accent.

Type is set in **EuclidCircularSemibold** and **system-ui**. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 16px.

Measured from [tradingview.com](https://www.tradingview.com/) on November 4, 2026 at 1440×900 and 390×844 from 500 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Near Black (#000000):** Page background. Token `background`, CSS `--color-popup-element-text-hover`.
- **White (#FFFFFF):** Primary text and headings, seen 10 times. Token `on-surface`, CSS `--_3-1Dsj`.
- **Silver (#DBDBDB):** Secondary text, seen 2 times. Token `on-surface-variant`, CSS `--color-tag-active-bg`.
- **Gray (#8C8C8C):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Charcoal (#222222):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--color-container-fill-secondary-neutral-bold`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Slate 15% (#63636326):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 1 time. Token `outline`.
- **Dark Teal (#06806B):** Brand accent (CSS variable), seen 5 times. Token `primary`, CSS `--color-content-primary-positive`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Mist (#F2F2F2):** High-contrast fills, seen 8 times. Token `inverse-surface`, CSS `--color-filter-select-fill_border-not-checked-hover`.
- **Vivid Blue (#2962FF):** Accent in text, fills and borders, seen 13 times. Token `secondary`, CSS `--color-text-field-border-focus-read-only`.
- **Vivid Orange (#FF9800):** Accent in text, fills and borders, seen 9 times. Token `tertiary`, CSS `--color-ad`.
- **Red (#CC2F3C):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**EuclidCircularSemibold** and **system-ui** share the interface. Fallback stack: `EuclidCircularSemibold, sans-serif`.

- **headline-display:** EuclidCircularSemibold 56px at weight 600, line height 1.14 (32px on mobile). Page title (h1).
- **headline-lg:** system-ui 36px at weight 600, line height 1.22 (28px on mobile). Section headings (h2).
- **headline-md:** system-ui 28px at weight 600, line height 1.29 (24px on mobile). Sub-section headings.
- **body-md:** system-ui 14px at weight 400. Body text.
- **body-lg:** system-ui 18px at weight 600, line height 1.33. Lead paragraphs.
- **body-sm:** system-ui 12px at weight 400, line height 1.33. Secondary and small text.
- **label-md:** system-ui 16px at weight 400, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 45px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 548px, 702px, 767px, 768px, 958px, 1019px, 1024px, 1214px, 1280px, 1374px, 1439px, 1440px, 1854px, 1920px, 2494px, 2560px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#222222) and #FFFFFF1A borders.

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **lg (16px):** 228 elements.
- **md (8px):** 68 elements.
- **sm (6px):** 28 elements.
- **xl (36px):** 24 elements.
- **xs (4px):** 20 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Search”):** #222222 fill, #8C8C8C text, 14px/400, 40px radius, padding 6px.
- **button-ghost (“Skip to main content”):** transparent fill, #000000 text, 14px/400, padding 2px 4px.
- **card:** #707070 fill, #9C9C9C text, 16px/500, padding 0px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #222222.
- Do keep text in 3 levels: #FFFFFF, #DBDBDB, #8C8C8C.
- Do use #06806B as the brand accent: header, logo and key highlights.
- Do keep spacing on the 4px grid.
- Do use 16px corners on most elements; larger surfaces also use 8px, 6px and 36px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond EuclidCircularSemibold and system-ui.
- Don't use #06806B for large backgrounds or body text.
- Don't make interface transitions slower than 0.45s.

## Motion

Interface transitions are quick: 0.45s, 0.15s. Longer ambient animations run 0.7s, 2s.

- **Easing:** `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/tradingview.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
