---
version: alpha
name: Luma
description: "Dark monochrome interface measured from lumalabs.ai: graphik type, flat surfaces and 24px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#B3B3B3"
  on-surface-muted: "#8C8C8C"
  on-surface-subtle: "#737373"
  primary: "#FFFFFF"
  on-primary: "#000000"
  secondary: "#D97757"
typography:
  headline-display:
    fontFamily: graphik
    fontSize: 52px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: graphik
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.04em
  headline-md:
    fontFamily: graphik
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.04em
  headline-sm:
    fontFamily: graphik
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: -0.03em
  body-md:
    fontFamily: graphik
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.025em
  body-lg:
    fontFamily: graphik
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.03em
  body-sm:
    fontFamily: graphik
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
    letterSpacing: -0.029em
  label-md:
    fontFamily: graphik
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.025em
  label-sm:
    fontFamily: graphik
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
  headline-display-mobile:
    fontFamily: graphik
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.04em
  headline-lg-mobile:
    fontFamily: graphik
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.04em
  headline-sm-mobile:
    fontFamily: graphik
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: -0.03em
rounded:
  sm: 8px
  md: 24px
spacing:
  sm: 6px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 20px
  section: 160px
  margin: 32px
  container: 1280px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    padding: 0px 12px
    height: 32px
  input-field:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    padding: 0px 24px
  link:
    textColor: "{colors.on-primary}"
---

# Luma Design System

## Overview

Luma describes itself as: “Luma AI is the creative AI platform for video generation and image creation. Powered by the world's leading video generation models, Ray and Uni, and creative agents handling end-to-end workflows. Trusted by leading agen” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **graphik**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 24px.

Measured from [lumalabs.ai](https://lumalabs.ai/) on November 4, 2026 at 1440×900 and 390×844 from 239 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Near Black (#000000):** Page background, seen 2 times. Token `background`, CSS `--tw-mask-bottom-from-color`.
- **White (#FFFFFF):** Primary text and headings, seen 22 times. Token `on-surface`, CSS `--tw-ring-offset-color`.
- **Gray (#B3B3B3):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Gray (#8C8C8C):** Muted text and metadata, seen 10 times. Token `on-surface-muted`.
- **Slate (#737373):** Subtle text and placeholders, seen 15 times. Token `on-surface-subtle`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 53 times. Token `primary`, CSS `--tw-ring-offset-color`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Red (#D97757):** Accent, seen 1 time. Token `secondary`.

## Typography

**graphik** carries the whole interface. Fallback stack: `__graphik_7126cf, __graphik_Fallback_7126cf`. Other loaded fonts: __graphik_7126cf.

- **headline-display:** graphik 52px at weight 500, line height 1.2, tracking -0.04em (32px on mobile). Page title (h1).
- **headline-lg:** graphik 48px at weight 500, line height 1.2, tracking -0.04em (28px on mobile). Section headings (h2).
- **headline-md:** graphik 32px at weight 500, line height 1.2, tracking -0.04em. Sub-section headings.
- **headline-sm:** graphik 22px at weight 500, line height 1.4, tracking -0.03em (18px on mobile). Card and feature titles.
- **body-md:** graphik 16px at weight 400, line height 1.5, tracking -0.025em. Body text.
- **body-lg:** graphik 18px at weight 400, line height 1.4, tracking -0.03em. Lead paragraphs.
- **body-sm:** graphik 14px at weight 400, line height 1.71, tracking -0.029em. Secondary and small text.
- **label-md:** graphik 16px at weight 500, line height 1.5, tracking -0.025em. Buttons, navigation and labels.
- **label-sm:** graphik 14px at weight 500, line height 1. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (87% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** sm 6px, md 12px, lg 20px, xl 40px.
- **Sections:** 160px vertical padding between major sections.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1280px.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 500px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast.

## Shapes

Most elements use 24px corners. Measured radii, most used first:

- **md (24px):** 52 elements.
- **sm (8px):** 32 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign In”):** #FFFFFF fill, #000000 text, 14px/500, 3.35544e+07px radius, padding 0px 12px.
- **input-field:** transparent fill, #000000 text, 18px/400, padding 0px.
- **card:** #000000 fill, #FFFFFF text, 16px/500, 3.35544e+07px radius, padding 0px 24px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page.
- Do keep text in 4 levels: #FFFFFF, #B3B3B3, #8C8C8C, #737373.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #000000.
- Do set headlines in graphik with tight tracking (-0.04em).
- Do reuse the measured spacing steps (6px, 12px, 20px).
- Do use 24px corners on most elements; larger surfaces also use 8px.
- Don't use #737373 for body text; it reaches 4.43:1 on #000000. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond graphik.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/lumalabs.ai/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
