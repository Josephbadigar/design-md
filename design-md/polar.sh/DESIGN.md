---
version: alpha
name: Polar
description: "Dark monochrome interface measured from polar.sh: PP Neue Montreal type, tonal surfaces and square corners."
colors:
  background: "#090909"
  surface: "#090909"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#858585"
  surface-container-low: "#212121"
  outline: "#212121"
  outline-variant: "#2A2A2A"
  primary: "#FFFFFF"
  on-primary: "#000000"
typography:
  display-hero:
    fontFamily: PP Neue Montreal
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.25
  headline-display:
    fontFamily: PP Neue Montreal
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.25
  headline-lg:
    fontFamily: PP Neue Montreal
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.38
  body-md:
    fontFamily: PP Neue Montreal
    fontSize: 16px
    fontWeight: 450
    lineHeight: 1.5
    letterSpacing: 0.015em
  body-lg:
    fontFamily: PP Neue Montreal
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: 0.01em
  body-sm:
    fontFamily: PP Neue Montreal
    fontSize: 14px
    fontWeight: 450
    lineHeight: 1.5
    letterSpacing: 0.017em
  caption:
    fontFamily: PP Neue Montreal
    fontSize: 12px
    fontWeight: 450
    lineHeight: 1.38
    letterSpacing: 0.02em
  label-md:
    fontFamily: PP Neue Montreal
    fontSize: 14px
    fontWeight: 550
    lineHeight: 1.43
    letterSpacing: 0.01em
  code:
    fontFamily: GeistMono
    fontSize: 12px
    fontWeight: 450
    lineHeight: 1.38
    letterSpacing: 0.02em
  headline-display-mobile:
    fontFamily: PP Neue Montreal
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.25
  headline-lg-mobile:
    fontFamily: PP Neue Montreal
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.38
rounded:
  none: 0px
spacing:
  base: 4px
  xs: 2px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 38.23px
  gutter: 8px
  section: 96px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    padding: 12px 20px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    padding: 12px 20px
  link:
    textColor: "{colors.primary}"
---

# Polar Design System

## Overview

Polar describes itself as: “Polar is the Merchant of Record for developers building AI-era software: payments, subscriptions, and usage-based billing, with global tax handled for you.” The interface is dark, built on **Near Black (#090909)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **PP Neue Montreal**, with **GeistMono** for code. Headlines run large; body text is 16px. The surface language is flat. Corners are square.

Measured from [polar.sh](https://polar.sh/) on November 4, 2026 at 1440×900 and 390×844 from 359 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Near Black (#090909):** Page background, seen 1 time. Token `background`, CSS `--xaxq9ro`.
- **White (#FFFFFF):** Primary text and headings, seen 77 times. Token `on-surface`, CSS `--color-white`.
- **Gray (#858585):** Secondary text, seen 61 times. Token `on-surface-variant`.
- **Charcoal (#212121):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--border`.
- **Charcoal (#212121):** Borders and dividers, seen 12 times. Token `outline`, CSS `--border`.
- **Graphite (#2A2A2A):** Secondary dividers, seen 10 times. Token `outline-variant`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 107 times. Token `primary`, CSS `--color-white`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.

## Typography

**PP Neue Montreal** and **GeistMono** (monospace) share the interface. Fallback stack: `PP Neue Montreal, InterDisplay, sans-serif`.

- **display-hero:** PP Neue Montreal 48px at weight 400, line height 1.25. Oversized hero statements.
- **headline-display:** PP Neue Montreal 36px at weight 400, line height 1.25 (30px on mobile). Page title (h1).
- **headline-lg:** PP Neue Montreal 30px at weight 400, line height 1.38 (24px on mobile). Section headings (h2).
- **body-md:** PP Neue Montreal 16px at weight 450, line height 1.5, tracking 0.015em. Body text.
- **body-lg:** PP Neue Montreal 24px at weight 400, line height 1.38, tracking 0.01em. Lead paragraphs.
- **body-sm:** PP Neue Montreal 14px at weight 450, line height 1.5, tracking 0.017em. Secondary and small text.
- **caption:** PP Neue Montreal 12px at weight 450, line height 1.38, tracking 0.02em. Captions and fine print.
- **label-md:** PP Neue Montreal 14px at weight 550, line height 1.43, tracking 0.01em. Buttons, navigation and labels.
- **code:** GeistMono 12px at weight 450, line height 1.38, tracking 0.02em. Code and technical values.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 2px, sm 8px, md 12px, lg 20px, xl 38.23px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 480px, 640px, 768px, 1024px, 1280px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#212121) and #212121 borders.

## Shapes

Corners are square. Measured radii, most used first:

- **none (0px):** measured.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #FFFFFF fill, #000000 text, 14px/550, 3.35544e+07px radius, padding 12px 20px.
- **button-ghost (“Sign in”):** transparent fill, #FFFFFF text, 14px/550, 3.35544e+07px radius, padding 12px 20px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #090909 for the page and lift surfaces in small steps: #212121.
- Do keep text in 2 levels: #FFFFFF, #858585.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #090909.
- Do keep spacing on the 4px grid.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond PP Neue Montreal and GeistMono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.12s, 0.1s, 0.2s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/polar.sh/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
