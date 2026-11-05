---
version: alpha
name: Mantine
description: "Light interface measured from mantine.dev: Outfit type with system-ui, vivid blue accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#1F2328"
  on-surface-muted: "#495057"
  on-surface-subtle: "#6E7781"
  surface-container-low: "#F8F9FA"
  surface-container: "#F1F3F5"
  surface-container-high: "#E9ECEF"
  overlay: "#FFFFFFD9"
  outline: "#CED4DA"
  outline-variant: "#DEE2E6"
  primary: "#339AF0"
  on-primary: "#000000"
  inverse-surface: "#242424"
  secondary: "#A5D8FF"
  tertiary: "#CF222E"
typography:
  display-hero:
    fontFamily: Outfit
    fontSize: 54px
    fontWeight: 450
    lineHeight: 1.1
  headline-display:
    fontFamily: Outfit
    fontSize: 44px
    fontWeight: 600
    lineHeight: 1.2
  headline-lg:
    fontFamily: Outfit
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.55
  headline-md:
    fontFamily: Outfit
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.4
  headline-sm:
    fontFamily: system-ui
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.4
  title-lg:
    fontFamily: system-ui
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.55
  body-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.55
  body-lg:
    fontFamily: system-ui
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.55
  body-sm:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.55
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.55
  label-sm:
    fontFamily: Outfit
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.4
  code:
    fontFamily: Menlo
    fontSize: 12px
    fontWeight: 700
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Outfit
    fontSize: 26px
    fontWeight: 600
    lineHeight: 1.2
  display-hero-mobile:
    fontFamily: Outfit
    fontSize: 38px
    fontWeight: 450
    lineHeight: 1.1
rounded:
  sm: 4px
  md: 8px
  lg: 15px
  xl: 16px
  full: 9999px
spacing:
  xs: 2px
  sm: 5px
  md: 12px
  lg: 20px
  xl: 48px
  gutter: 20px
  section: 120px
components:
  button-primary:
    textColor: "{colors.background}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 3px 20px 0px 20px
    height: 60px
  button-secondary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 3px 20px 0px 20px
    height: 60px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "#868E96"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 4px 0px 12px
    height: 34px
  button-ghost:
    textColor: "#E7F5FF"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 10px 20px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 0px 16.67px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 20px
  link:
    textColor: "{colors.on-surface}"
---

# Mantine Design System

## Overview

Mantine describes itself as: “A fully featured React components library with 120+ customizable components, hooks, and utilities. Build accessible web applications faster.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Blue (#339AF0)** as the main accent.

Type is set in **Outfit** and **system-ui**, with **Menlo** for code. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [mantine.dev](https://mantine.dev/) on November 4, 2026 at 1440×900 and 390×844 from 431 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #228BE6, #1C7ED6, #5865F2, #535ED4.

- **White (#FFFFFF):** Page background, seen 83 times. Token `background`, CSS `--mantine-color-white-light-hover`.
- **Near Black (#000000):** Primary text and headings, seen 86 times. Token `on-surface`, CSS `--mantine-color-adaptive-light`.
- **Cool Charcoal (#1F2328):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Cool Slate (#495057):** Muted text and metadata, seen 13 times. Token `on-surface-muted`, CSS `--mantine-color-gray-filled-hover`.
- **Cool Slate (#6E7781):** Subtle text and placeholders, seen 3 times. Token `on-surface-subtle`.
- **Snow (#F8F9FA):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`, CSS `--mantine-color-gray-0`.
- **Mist (#F1F3F5):** Cards and panels, seen 2 times. Token `surface-container`.
- **Cool Mist (#E9ECEF):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **White 85% (#FFFFFFD9):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Cool Silver (#CED4DA):** Borders and dividers, seen 50 times. Token `outline`.
- **Cool Mist (#DEE2E6):** Secondary dividers, seen 30 times. Token `outline-variant`.
- **Vivid Blue (#339AF0):** Brand color in the logo, seen 1 time. Token `primary`, CSS `--mantine-color-blue-5`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Graphite (#242424):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Light Blue (#A5D8FF):** Accent (CSS variable). Token `secondary`.
- **Red (#CF222E):** Accent in text, fills and borders, seen 7 times. Token `tertiary`.

## Typography

**Outfit**, **system-ui** and **Menlo** (monospace) share the interface. Fallback stack: `Outfit, sans-serif`.

- **display-hero:** Outfit 54px at weight 450, line height 1.1 (38px on mobile). Oversized hero statements.
- **headline-display:** Outfit 44px at weight 600, line height 1.2 (26px on mobile). Page title (h1).
- **headline-lg:** Outfit 32px at weight 400, line height 1.55. Section headings (h2).
- **headline-md:** Outfit 28px at weight 400, line height 1.4. Sub-section headings.
- **headline-sm:** system-ui 22px at weight 400, line height 1.4. Card and feature titles.
- **title-lg:** system-ui 20px at weight 400, line height 1.55. Small titles.
- **body-md:** system-ui 14px at weight 400, line height 1.55. Body text.
- **body-lg:** system-ui 18px at weight 600, line height 1.55. Lead paragraphs.
- **body-sm:** system-ui 12px at weight 400, line height 1.55. Secondary and small text.
- **label-md:** system-ui 16px at weight 400, line height 1.55. Buttons, navigation and labels.
- **label-sm:** Outfit 14px at weight 600, line height 1.4. Small labels and badges.
- **code:** Menlo 12px at weight 700, line height 1. Code and technical values.

## Layout

Spacing does not follow a strict grid: 57% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 5px, md 12px, lg 20px, xl 48px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Breakpoints:** 750px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#F8F9FA → #F1F3F5 → #E9ECEF):

- `rgba(0, 0, 0, 0.1) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.15) 0px 0px 4px 0px inset`

A few raised panels add a soft drop shadow: `color(srgb 0.133333 0.545098 0.901961 / 0.2) 0px 0px 15px 2px`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 278 elements.
- **xl (16px):** 52 elements.
- **sm (4px):** 34 elements.
- **full (9999px):** 28 elements.
- **lg (15px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** transparent fill, #FFFFFF text, 18px/600, 8px radius, padding 3px 20px 0px 20px, shadow `color(srgb 0.133333 0.545098 0.901961 / 0.2) 0px 0px 15px 2px`.
- **button-secondary (“GitHub”):** #242424 fill, #FFFFFF text, 18px/600, 8px radius, padding 3px 20px 0px 20px.
- **button-outline (“Search Ctrl + K”):** #FFFFFF fill, #868E96 text, 16px/400, 8px radius, padding 0px 4px 0px 12px, border 1px solid #DEE2E6.
- **button-ghost (“Documentation”):** transparent fill, #E7F5FF text, 18px/600, 8px radius, padding 10px 20px.
- **input-field (“Text input”):** #FFFFFF fill, #000000 text, 18px/400, 8px radius, padding 0px 16.67px, border 1px solid #CED4DA.
- **card:** #FFFFFF fill, #000000 text, 16px/400, 16px radius, padding 20px, border 1px solid #E9ECEF.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8F9FA, #F1F3F5, #E9ECEF.
- Do keep text in 4 levels: #000000, #1F2328, #495057, #6E7781.
- Do use #339AF0 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (5px, 12px, 20px).
- Do use 8px corners on most elements; larger surfaces also use 16px, 4px and 15px.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Outfit, system-ui and Menlo.
- Don't use #339AF0 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.1s, 0.15s, 0.2s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mantine.dev/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
