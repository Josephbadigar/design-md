---
version: alpha
name: Product Hunt
description: "Light interface measured from producthunt.com: system-ui type, red accents, tonal surfaces and 12px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#101828"
  on-background: "#101828"
  on-surface-variant: "#344054"
  on-surface-muted: "#4B587C"
  on-surface-subtle: "#98A2B3"
  surface-container-low: "#F2F4F7"
  outline: "#EAECF0"
  outline-variant: "#D9E1EC"
  primary: "#FF6154"
  on-primary: "#FFFFFF"
  secondary: "#DB5246"
typography:
  headline-display:
    fontFamily: system-ui
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
  body-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1
  headline-display-mobile:
    fontFamily: system-ui
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.5
rounded:
  sm: 4px
  md: 12px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 16px
  container: 900px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px 16px
    height: 40px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 8px 16px
    height: 44px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px 16px
    height: 40px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px 40px
  link:
    textColor: "{colors.on-primary}"
---

# Product Hunt Design System

## Overview

Product Hunt describes itself as: “Product Hunt is a curation of the best new products, every day. Discover the latest mobile apps, websites, and technology products that everyone's talking about.” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#101828)** text, and **Red (#FF6154)** as the main accent.

Type is set in **system-ui**. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 12px.

Measured from [producthunt.com](https://www.producthunt.com/) on November 4, 2026 at 1440×900 and 390×844 from 449 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 6 times. Token `background`, CSS `--nav-menu-item-bg`.
- **Deep Blue (#101828):** Primary text and headings, seen 64 times. Token `on-surface`, CSS `--text-primary`.
- **Dark Blue (#344054):** Secondary text, seen 48 times. Token `on-surface-variant`, CSS `--text-secondary`.
- **Blue (#4B587C):** Muted text and metadata, seen 28 times. Token `on-surface-muted`.
- **Blue (#98A2B3):** Subtle text and placeholders, seen 4 times. Token `on-surface-subtle`.
- **Snow (#F2F4F7):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--background-tertiary`.
- **Cool Mist (#EAECF0):** Borders and dividers, seen 4 times. Token `outline`, CSS `--border-primary`.
- **Pale Blue (#D9E1EC):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Red (#FF6154):** Primary buttons and calls to action, seen 4 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Red (#DB5246):** Accent, seen 1 time. Token `secondary`.

## Typography

**system-ui** carries the whole interface. Fallback stack: `-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica`.

- **headline-display:** system-ui 24px at weight 600, line height 1.33 (20px on mobile). Page title (h1).
- **body-md:** system-ui 14px at weight 400, line height 1.71. Body text.
- **label-md:** system-ui 16px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** system-ui 14px at weight 600, line height 1. Small labels and badges.

## Layout

Spacing follows a 4px grid: 96% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 900px.
- **Breakpoints:** 359px, 375px, 758px, 759px, 1098px, 1099px, 1439px, 1536px, 1728px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F2F4F7) and #EAECF0 borders.

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **md (12px):** 236 elements.
- **full (9999px):** 20 elements.
- **sm (4px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign in”):** #FF6154 fill, #FFFFFF text, 16px/600, 9999px radius, padding 0px 16px.
- **button-outline (“View all”):** #FFFFFF fill, #344054 text, 16px/600, 9999px radius, padding 8px 16px, border 2px solid #EAECF0.
- **button-ghost (“Subscribe”):** transparent fill, #344054 text, 16px/600, 9999px radius, padding 0px 16px, border 2px solid #EAECF0.
- **input-field (“Search ( ctrl + k )”):** #F2F4F7 fill, #4B587C text, 16px/400, 9999px radius, padding 0px 40px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F2F4F7.
- Do keep text in 4 levels: #101828, #344054, #4B587C, #98A2B3.
- Do reserve #FF6154 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do use 12px corners on most elements; larger surfaces also use 4px.
- Don't use #98A2B3 for body text; it reaches 2.58:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond system-ui.
- Don't use #FF6154 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s.

- **Easing:** `cubic-bezier(0, 0, 0.2, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.23, 1, 0.32, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/producthunt.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
