---
version: alpha
name: Lucide
description: "Light interface measured from lucide.dev: Inter type, light red accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#3C3C43"
  on-background: "#3C3C43"
  on-surface-variant: "#67676C"
  surface-container-low: "#F6F6F7"
  surface-container: "#EBEBEF"
  overlay: "#8E96AA24"
  outline: "#E2E2E3"
  outline-variant: "#C2C2C4"
  primary: "#F67373"
  on-primary: "#3C3C43"
  secondary: "#F56565"
  tertiary: "#DC5A5A"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 21px
    fontWeight: 500
    lineHeight: 1.14
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.71
  label-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.54
  code:
    fontFamily: ui-monospace
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.85
    letterSpacing: 0.077em
rounded:
  sm: 6px
  md: 8px
  lg: 12px
  xl: 20px
  full: 9999px
spacing:
  base: 4px
  xs: 2px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
  margin: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 2px
    padding: 0px 12px
    height: 64px
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 0px 20px
    height: 40px
  button-outline-hover:
    backgroundColor: "#E4E4E9"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 0px 20px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.code}"
    rounded: 0px
    padding: 0px 12px
  input-field:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.code}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 24px
---

# Lucide Design System

## Overview

Lucide describes itself as: “Beautiful & consistent icon toolkit made by the community.” The interface is light, built on **White (#FFFFFF)** with **Cool Graphite (#3C3C43)** text, and **Light Red (#F67373)** as the main accent.

Type is set in **Inter**, with **ui-monospace** for code. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [lucide.dev](https://lucide.dev/) on November 4, 2026 at 1440×900 and 390×844 from 315 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 70 times. Token `background`, CSS `--vp-local-nav-bg-color`.
- **Cool Graphite (#3C3C43):** Primary text and headings, seen 38 times. Token `on-surface`, CSS `--vp-code-tab-hover-text-color`.
- **Slate (#67676C):** Secondary text, seen 21 times. Token `on-surface-variant`, CSS `--vp-code-block-color`.
- **Snow (#F6F6F7):** Raised areas one step from the page, seen 8 times. Token `surface-container-low`, CSS `--vp-code-block-bg`.
- **Mist (#EBEBEF):** Cards and panels, seen 3 times. Token `surface-container`, CSS `--vp-c-default-3`.
- **Blue 14% (#8E96AA24):** Translucent fill for cards and controls, seen 2 times. Token `overlay`, CSS `--vp-badge-info-bg`.
- **Mist (#E2E2E3):** Borders and dividers, seen 9 times. Token `outline`, CSS `--vp-code-block-divider-color`.
- **Silver (#C2C2C4):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Light Red (#F67373):** Primary buttons and calls to action, seen 7 times. Token `primary`, CSS `--vp-c-note-1`.
- **Cool Graphite (#3C3C43):** Text and icons on primary. Token `on-primary`.
- **Red (#F56565):** Secondary buttons, seen 3 times. Token `secondary`, CSS `--vp-c-tip-3`.
- **Red (#DC5A5A):** Accent (CSS variable). Token `tertiary`.

## Typography

**Inter** and **ui-monospace** (monospace) share the interface. Fallback stack: `Inter, ui-sans-serif, system-ui, sans-serif`.

- **headline-display:** Inter 21px at weight 500, line height 1.14. Page title (h1).
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **label-lg:** Inter 16px at weight 600, line height 1.5. Large buttons and tabs.
- **label-md:** Inter 14px at weight 500, line height 1.71. Buttons, navigation and labels.
- **label-sm:** Inter 13px at weight 600, line height 1.54. Small labels and badges.
- **code:** ui-monospace 13px at weight 400, line height 1.85, tracking 0.077em. Code and technical values.

## Layout

Spacing follows a 4px grid: 92% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 2px, sm 8px, md 12px, lg 24px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.04) 0px 1px 2px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px`
- `rgba(0, 0, 0, 0.1) 0px 12px 32px 0px, rgba(0, 0, 0, 0.08) 0px 2px 6px 0px`
- `rgba(0, 0, 0, 0.12) 0px 14px 44px 0px, rgba(0, 0, 0, 0.12) 0px 3px 9px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 68 elements.
- **lg (12px):** 32 elements.
- **xl (20px):** 20 elements.
- **sm (6px):** 8 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Icons”):** #F67373 fill, #3C3C43 text, 14px/500, 2px radius, padding 0px 12px.
- **button-outline (“Get Started”):** #EBEBEF fill, #3C3C43 text, 14px/600, 20px radius, padding 0px 20px.
- **button-outline-hover:** background #E4E4E9, text #3C3C43 on hover.
- **button-secondary (“View all icons”):** #F56565 fill, #FFFFFF text, 14px/600, 20px radius, padding 0px 20px.
- **button-ghost (“Resources”):** transparent fill, #3C3C43 text, 13.3333px/400, padding 0px 12px.
- **input-field:** transparent fill, #67676C text, 13.3333px/400, padding 0px.
- **card:** #F6F6F7 fill, #3C3C43 text, 16px/400, 12px radius, padding 24px, border 1px solid #E2E2E3.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F6F6F7, #EBEBEF.
- Do keep text in 2 levels: #3C3C43, #67676C.
- Do reserve #F67373 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do use 8px corners on most elements; larger surfaces also use 12px, 20px and 6px.
- Don't introduce new font families beyond Inter and ui-monospace.
- Don't use #F67373 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.25s, 0.15s, 0.5s, 0.4s.

- **Easing:** `ease`, `ease-in`, `cubic-bezier(0.34, 1.56, 0.64, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/lucide.dev/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
