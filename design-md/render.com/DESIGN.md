---
version: alpha
name: Render
description: "Dark interface measured from render.com: Roobert type with PPNeueMontreal, deep violet accents, flat surfaces and square corners."
colors:
  background: "#0D0D0D"
  surface: "#0D0D0D"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#E3E3E3"
  on-surface-muted: "#6B6B6B"
  outline: "#272727"
  primary: "#1C0037"
  on-primary: "#FFFFFF"
  secondary: "#D1B8FF"
  tertiary: "#8A05FF"
  success: "#5CFFB8"
  warning: "#FAF1A3"
  error: "#F0989E"
typography:
  headline-display:
    fontFamily: Roobert
    fontSize: 80px
    fontWeight: 300
    lineHeight: 1
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Roobert
    fontSize: 64px
    fontWeight: 300
    lineHeight: 1.06
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Roobert
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.015em
  headline-sm:
    fontFamily: Roobert
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: -0.025em
  body-md:
    fontFamily: Roobert
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  body-sm:
    fontFamily: PPNeueMontreal
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.44
    letterSpacing: 0.005em
  caption:
    fontFamily: PPNeueMontreal
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: -0.01em
  label-md:
    fontFamily: PPNeueMontreal
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0.01em
  headline-display-mobile:
    fontFamily: Roobert
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.08
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Roobert
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.015em
rounded:
  none: 0px
spacing:
  xs: 2px
  sm: 6px
  md: 16px
  lg: 20px
  xl: 60px
  gutter: 10px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.none}"
    padding: 24px 30px
    height: 66px
  button-primary-hover:
    textColor: "{colors.on-surface}"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.secondary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.none}"
    padding: 0px
    height: 25px
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.none}"
    padding: 0px 24px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.none}"
    padding: 0px 24px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Render Design System

## Overview

Render describes itself as: “Deploy and scale any app or agent from your first user to your billionth. Build faster on intuitive cloud infrastructure for the modern web.” The interface is dark, built on **Charcoal (#0D0D0D)** with **White (#FFFFFF)** text, and **Deep Violet (#1C0037)** as the main accent.

Type is set in **Roobert** and **PPNeueMontreal**. Headlines run large with tight negative tracking; body text is 20px. The surface language is flat. Corners are square.

Measured from [render.com](https://render.com/) on October 21, 2026 at 1440×900 and 390×844 from 341 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #9B52FB, #B8FFD7, #1C0037.

- **Charcoal (#0D0D0D):** Page background, seen 5 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 51 times. Token `on-surface`, CSS `--osano-toggle-on-thumb-color`.
- **Mist (#E3E3E3):** Secondary text, seen 3 times. Token `on-surface-variant`, CSS `--color-text-secondary`.
- **Slate (#6B6B6B):** Muted text and metadata, seen 46 times. Token `on-surface-muted`, CSS `--color-gray-500`.
- **Graphite (#272727):** Borders and dividers, seen 6 times. Token `outline`.
- **Deep Violet (#1C0037):** Brand color in the header, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Pale Violet (#D1B8FF):** Secondary buttons, seen 43 times. Token `secondary`, CSS `--color-purple-200`.
- **Vivid Violet (#8A05FF):** Brand color on large areas, seen 7 times. Token `tertiary`.
- **Teal (#5CFFB8):** Success and positive states, seen 2 times. Token `success`.
- **Light Yellow (#FAF1A3):** Warnings and highlights, seen 1 time. Token `warning`.
- **Light Red (#F0989E):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**Roobert** and **PPNeueMontreal** share the interface. Fallback stack: `Roobert, Roobert Fallback, sans-serif`. Other loaded fonts: PPNeueMontrealMono, PPNeueMontrealMono Fallback, PPNeueMontreal Fallback, Roobert Fallback.

- **headline-display:** Roobert 80px at weight 300, line height 1, tracking -0.03em (48px on mobile). Page title (h1).
- **headline-lg:** Roobert 64px at weight 300, line height 1.06, tracking -0.02em (40px on mobile). Section headings (h2).
- **headline-md:** Roobert 40px at weight 300, line height 1.1, tracking -0.015em. Sub-section headings.
- **headline-sm:** Roobert 32px at weight 400, line height 1.15, tracking -0.025em. Card and feature titles.
- **body-md:** Roobert 20px at weight 400, line height 1.2, tracking -0.01em. Body text.
- **body-sm:** PPNeueMontreal 18px at weight 400, line height 1.44, tracking 0.005em. Secondary and small text.
- **caption:** PPNeueMontreal 14px at weight 400, line height 1.38, tracking -0.01em. Captions and fine print.
- **label-md:** PPNeueMontreal 16px at weight 400, line height 1.25, tracking 0.01em. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 50% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 16px, lg 20px, xl 60px.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Breakpoints:** 376px, 420px, 600px, 640px, 768px, 1024px, 1180px, 1200px, 1440px, 1522px, 1600px, 1760px, 1920px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #272727 borders.

## Shapes

Corners are square. Measured radii, most used first:

- **none (0px):** measured.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #FFFFFF fill, #0D0D0D text, 16px/400, padding 24px 30px.
- **button-primary-hover:** background #FFFFFF, text #FFFFFF on hover.
- **button-secondary (“See customer stories”):** #D1B8FF fill, #D1B8FF text, 16px/400, padding 0px.
- **button-outline (“Talk to sales”):** transparent fill, #FFFFFF text, 16px/400, padding 0px 24px, border 1px solid #FFFFFF.
- **button-ghost (“HIPAA on Render”):** transparent fill, #FFFFFF text, 16px/400, padding 0px 24px, border 1px solid #FFFFFF.
- **link:** transparent fill, #6B6B6B text, padding 0px.

## Do's and Don'ts

- Do use #0D0D0D for the page.
- Do keep text in 3 levels: #FFFFFF, #E3E3E3, #6B6B6B.
- Do use #1C0037 as the brand accent: header, logo and key highlights.
- Do set headlines in Roobert with tight tracking (-0.03em).
- Do reuse the measured spacing steps (6px, 16px, 20px).
- Don't use #6B6B6B for body text; it reaches 3.6:1 on #0D0D0D. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Roobert and PPNeueMontreal.
- Don't use #1C0037 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/render.com/), the free DESIGN.md generator.
