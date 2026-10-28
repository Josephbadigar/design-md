---
version: alpha
name: Raycast
description: "Dark interface measured from raycast.com: Inter type with Segoe UI Variable, red accents, tonal surfaces and 20px corners."
colors:
  background: "#07080A"
  surface: "#07080A"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#9C9C9D"
  on-surface-muted: "#6A6B6C"
  on-surface-subtle: "#434345"
  surface-container-low: "#130D0E"
  surface-container: "#111214"
  overlay: "#FFFFFF1A"
  overlay-strong: "#FFFFFF05"
  outline: "#FFFFFF0F"
  outline-variant: "#FFFFFF0D"
  primary: "#FF6363"
  on-primary: "#000000"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 64px
    fontWeight: 600
    lineHeight: 1.1
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: 0.008em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 500
    letterSpacing: 0.01em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.78
  body-sm:
    fontFamily: Segoe UI Variable
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.23
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: 0.008em
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.6
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    letterSpacing: 0.014em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: 0.008em
  code:
    fontFamily: GeistMono
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: 0.021em
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.1
  headline-md-mobile:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: 0.011em
rounded:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 20px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "#E6E6E6"
    textColor: "#2F3031"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
    height: 36px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 4px 12px
    height: 30px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.caption}"
    rounded: "{rounded.xs}"
    padding: 0px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px 8px 0px 4px
  card:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Raycast Design System

## Overview

Raycast describes itself as: “A collection of powerful productivity tools all within an extendable launcher.” The interface is dark, built on **Near Black (#07080A)** with **White (#FFFFFF)** text, and **Red (#FF6363)** as the main accent.

Type is set in **Inter** and **Segoe UI Variable**, with **GeistMono** for code. Headlines run large; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 20px.

Measured from [raycast.com](https://www.raycast.com/) on October 21, 2026 at 1440×900 and 390×844 from 390 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #043F96B3, #523091B3, #20235BB3.

- **Near Black (#07080A):** Page background, seen 1 time. Token `background`, CSS `--grey-900`.
- **White (#FFFFFF):** Primary text and headings, seen 61 times. Token `on-surface`, CSS `--reverse-background`.
- **Gray (#9C9C9D):** Secondary text, seen 31 times. Token `on-surface-variant`, CSS `--grey-200`.
- **Slate (#6A6B6C):** Muted text and metadata, seen 6 times. Token `on-surface-muted`, CSS `--grey-300`.
- **Graphite (#434345):** Subtle text and placeholders, seen 12 times. Token `on-surface-subtle`, CSS `--grey-400`.
- **Warm Charcoal (#130D0E):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Charcoal (#111214):** Cards and panels, seen 1 time. Token `surface-container`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 5 times. Token `overlay`.
- **White 2% (#FFFFFF05):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **White 6% (#FFFFFF0F):** Borders and dividers, seen 9 times. Token `outline`.
- **White 5% (#FFFFFF0D):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Red (#FF6363):** Brand color in the logo, seen 3 times. Token `primary`, CSS `--red-dark`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.

## Typography

**Inter**, **Segoe UI Variable** and **GeistMono** (monospace) share the interface. Fallback stack: `Inter, Inter Fallback, sans-serif`. Other loaded fonts: Inter Fallback, jetBrainsMono, jetBrainsMono Fallback.

- **headline-display:** Inter 64px at weight 600, line height 1.1 (36px on mobile). Page title (h1).
- **headline-lg:** Inter 24px at weight 500, line height 1.6, tracking 0.008em. Section headings (h2).
- **headline-md:** Inter 20px at weight 500, tracking 0.01em (18px on mobile). Sub-section headings.
- **body-md:** Inter 16px at weight 400, line height 1.15. Body text.
- **body-lg:** Inter 18px at weight 400, line height 1.78. Lead paragraphs.
- **body-sm:** Segoe UI Variable 13px at weight 400, line height 1.23. Secondary and small text.
- **caption:** Inter 12px at weight 400, line height 1.15, tracking 0.008em. Captions and fine print.
- **label-lg:** Inter 16px at weight 500, line height 1.6. Large buttons and tabs.
- **label-md:** Inter 14px at weight 500, tracking 0.014em. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 600, line height 1.15, tracking 0.008em. Small labels and badges.
- **code:** GeistMono 14px at weight 500, line height 1.6, tracking 0.021em. Code and technical values.

## Layout

Spacing follows a 4px grid: 96% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 480px, 540px, 548px, 640px, 720px, 767px, 768px, 800px, 840px, 880px, 1000px, 1024px, 1064px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#130D0E → #111214):

- `rgba(255, 255, 255, 0.05) 0px 1px 0px 0px inset, rgba(255, 255, 255, 0.25) 0px 0px 0px 1px, rgba(0, 0, 0, 0.2) 0px -1px 0px 0px inset`
- `rgb(27, 28, 30) 0px 0px 0px 1px, rgb(7, 8, 10) 0px 0px 0px 1px inset`
- `rgba(255, 255, 255, 0.1) 0px 1px 0px 0px inset`

A few raised panels add a soft drop shadow: `rgba(215, 201, 175, 0.05) 0px 0px 20px 5px, rgba(215, 201, 175, 0.05) 0px 0px 16px -7px`.

## Shapes

Most elements use 20px corners. Measured radii, most used first:

- **xl (20px):** 136 elements.
- **lg (16px):** 96 elements.
- **sm (8px):** 92 elements.
- **md (12px):** 92 elements.
- **xs (4px):** 68 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Download”):** #E6E6E6 fill, #2F3031 text, 14px/500, 8px radius, padding 8px 12px, shadow `rgba(0, 0, 0, 0.5) 0px 0px 0px 2px, rgba(255, 255, 255, 0.19) 0px 0px 14px 0px, rgba(0, 0, 0, 0.2) 0px -1px 0.4px 0px inset, rgb(255, 255, 255) 0px 1px 0.4px 0px inset`.
- **button-primary-hover:** background #FFFFFF, text #2F3031 on hover.
- **button-outline (“The Raycast Keyboard”):** #130D0E fill, #FFFFFF text, 14px/500, 1000px radius, padding 4px 12px.
- **button-ghost (“Install via WinGet”):** transparent fill, #9C9C9D text, 12px/400, 4px radius, padding 0px.
- **input-field (“Ask anything, @ tools, or / for ”):** transparent fill, #FFFFFF text, 14px/400, padding 0px 8px 0px 4px.
- **card:** transparent fill, #FFFFFF text, 16px/400, 20px radius, padding 0px, shadow `rgba(255, 255, 255, 0.1) 0px 1px 0px 0px inset, rgba(7, 13, 79, 0.05) 0px 0px 20px 3px, rgba(7, 13, 79, 0.05) 0px 0px 40px 20px, rgba(255, 255, 255, 0.06) 0px 0px 0px 1px inset`.
- **link:** transparent fill, #9C9C9D text, padding 0px.

## Do's and Don'ts

- Do use #07080A for the page and lift surfaces in small steps: #130D0E, #111214.
- Do keep text in 4 levels: #FFFFFF, #9C9C9D, #6A6B6C, #434345.
- Do use #FF6363 as the brand accent: header, logo and key highlights.
- Do keep spacing on the 4px grid.
- Do use 20px corners on most elements; larger surfaces also use 16px, 8px and 12px.
- Don't use #6A6B6C for body text; it reaches 3.8:1 on #07080A. Keep it for large text or metadata.
- Don't use #434345 for body text; it reaches 2.0:1 on #07080A. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Inter, Segoe UI Variable and GeistMono.
- Don't use #FF6363 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.1s, 0.15s. Longer ambient animations run 1.1s, 1s.

- **Easing:** `ease`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/raycast.com/), the free DESIGN.md generator.
