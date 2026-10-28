---
version: alpha
name: Oura Ring
description: "Light interface measured from ouraring.com: Editorial New type with AkkuratLL, blue accents, tonal surfaces and 8px corners."
colors:
  background: "#F7F1E8"
  surface: "#F7F1E8"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#4A4741"
  on-surface-muted: "#A8A5A0"
  surface-container-low: "#FFFFFF"
  outline: "#4A474140"
  outline-variant: "#FFFFFF"
  primary: "#2A72DE"
  on-primary: "#FFFFFF"
  secondary: "#253B80"
  success: "#34A853"
  warning: "#FBBC04"
  error: "#EA4335"
typography:
  headline-display:
    fontFamily: Editorial New
    fontSize: 80px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: Editorial New
    fontSize: 68px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-md:
    fontFamily: AkkuratLL
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1
  headline-sm:
    fontFamily: AkkuratLL
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.25
  title-lg:
    fontFamily: AkkuratLL
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.5
  body-md:
    fontFamily: AkkuratLL
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: AkkuratLL
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-lg:
    fontFamily: AkkuratLL
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: AkkuratLL
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.5
  label-sm:
    fontFamily: AkkuratLL
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0.01em
  headline-display-mobile:
    fontFamily: Editorial New
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.05em
  headline-sm-mobile:
    fontFamily: AkkuratLL
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
rounded:
  sm: 8px
  md: 12px
  lg: 90px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 80px
  margin: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    padding: 12px 24px
    height: 48px
  button-primary-hover:
    backgroundColor: "#2056A6"
  button-secondary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.background}"
    typography: "{typography.label-lg}"
    padding: 12px 24px
    height: 48px
  button-secondary-hover:
    backgroundColor: "#1C1B1A"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 12px 16px
    height: 42px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    padding: 12px 24px
  input-field:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 8px 48px 8px 20px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 24px
  link:
    textColor: "{colors.background}"
---

# Oura Ring Design System

## Overview

Oura Ring describes itself as: “Enhance your health journey with Oura. The Oura Ring provides round-the-clock insights into sleep, fitness, and stress for wellness. Now HSA/FSA eligible.” The interface is light, built on **Warm Mist (#F7F1E8)** with **Near Black (#000000)** text, and **Blue (#2A72DE)** as the main accent.

Type is set in **Editorial New** and **AkkuratLL**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [ouraring.com](https://ouraring.com/) on October 21, 2026 at 1440×900 and 903×1955 from 236 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Warm Mist (#F7F1E8):** Page background, seen 6 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 12 times. Token `on-surface`.
- **Warm Graphite (#4A4741):** Secondary text, seen 15 times. Token `on-surface-variant`, CSS `--color-sandstone-500`.
- **Warm Gray (#A8A5A0):** Muted text and metadata, seen 13 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--color-white`.
- **Warm Graphite 25% (#4A474140):** Borders and dividers, seen 1 time. Token `outline`.
- **White (#FFFFFF):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--color-white`.
- **Blue (#2A72DE):** Primary buttons and calls to action, seen 5 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#253B80):** Accent, seen 3 times. Token `secondary`.
- **Green (#34A853):** Success and positive states, seen 1 time. Token `success`.
- **Vivid Amber (#FBBC04):** Warnings and highlights, seen 1 time. Token `warning`.
- **Vivid Red (#EA4335):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**Editorial New** and **AkkuratLL** share the interface. Fallback stack: `Editorial New, serif`.

- **headline-display:** Editorial New 80px at weight 300, line height 1.1, tracking -0.05em (48px on mobile). Page title (h1).
- **headline-lg:** Editorial New 68px at weight 400, line height 1.1, tracking -0.03em. Section headings (h2).
- **headline-md:** AkkuratLL 40px at weight 300, line height 1. Sub-section headings.
- **headline-sm:** AkkuratLL 24px at weight 400, line height 1.25 (12px on mobile). Card and feature titles.
- **title-lg:** AkkuratLL 20px at weight 700, line height 1.5. Small titles.
- **body-md:** AkkuratLL 14px at weight 400, line height 1.5. Body text.
- **body-sm:** AkkuratLL 12px at weight 400, line height 1.33. Secondary and small text.
- **label-lg:** AkkuratLL 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** AkkuratLL 14px at weight 700, line height 1.5. Buttons, navigation and labels.
- **label-sm:** AkkuratLL 13px at weight 600, line height 1.2, tracking 0.01em. Small labels and badges.

## Layout

Spacing follows a 4px grid: 95% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 48px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 320px, 419px, 420px, 768px, 1024px, 1280px, 1440px, 1568px, 1920px, 1999px, 2000px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#FFFFFF) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(255, 255, 255, 0.06) 0px 1px 0px 0px inset`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 16 elements.
- **lg (90px):** 12 elements.
- **md (12px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Shop Now”):** #2A72DE fill, #FFFFFF text, 16px/700, 3.35544e+07px radius, padding 12px 24px.
- **button-primary-hover:** background #2056A6, text #FFFFFF on hover.
- **button-secondary (“Why Oura”):** #4A4741 fill, #F7F1E8 text, 16px/400, 3.35544e+07px radius, padding 12px 24px.
- **button-secondary-hover:** background #1C1B1A, text #F7F1E8 on hover.
- **button-outline (“Manage”):** #FFFFFF fill, #4A4741 text, 13.008px/600, 90px radius, padding 12px 16px, border 1px solid #4A4741.
- **button-ghost (“Shop”):** transparent fill, #000000 text, 16px/400, 3.35544e+07px radius, padding 12px 24px.
- **input-field:** #4A4741 fill, #FFFFFF text, 16px/400, 12px radius, padding 8px 48px 8px 20px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(255, 255, 255, 0.06) 0px 1px 0px 0px inset`.
- **card:** #F7F1E8 fill, #000000 text, 16px/400, 8px radius, padding 24px.
- **link:** transparent fill, #F7F1E8 text, padding 0px.

## Do's and Don'ts

- Do use #F7F1E8 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 3 levels: #000000, #4A4741, #A8A5A0.
- Do reserve #2A72DE for primary actions and key highlights.
- Do set headlines in Editorial New with tight tracking (-0.05em).
- Do keep spacing on the 4px grid.
- Do use 8px corners on most elements; larger surfaces also use 90px and 12px.
- Don't use #A8A5A0 for body text; it reaches 2.2:1 on #F7F1E8. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Editorial New and AkkuratLL.
- Don't use #2A72DE for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.2s, 0.5s. Longer ambient animations run 0.7s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/ouraring.com/), the free DESIGN.md generator.
