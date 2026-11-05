---
version: alpha
name: Checkout.com
description: "Dark interface measured from checkout.com: Inter type, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  surface-container-low: "#181818"
  surface-container: "#272932"
  primary: "#186AFF"
  on-primary: "#FFFFFF"
  secondary: "#006CFF"
typography:
  headline-display:
    fontFamily: Checkout Apercu SemiMono
    fontSize: 80px
    fontWeight: 700
    lineHeight: 0.9
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.18
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
  body-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.44
  body-sm:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
    letterSpacing: 0.05em
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.37
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: 500
    lineHeight: 2
  code:
    fontFamily: Checkout Apercu SemiMono
    fontSize: 48px
    fontWeight: 700
    lineHeight: 0.9
    letterSpacing: -0.04em
  headline-display-mobile:
    fontFamily: Checkout Apercu SemiMono
    fontSize: 40px
    fontWeight: 700
    lineHeight: 0.9
  headline-md-mobile:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.18
rounded:
  sm: 6px
  md: 12px
  lg: 16px
  xl: 24px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 16px
  section: 80px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 12px 0px
    height: 48px
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 11px 23px
    height: 45px
  button-outline-hover:
    backgroundColor: "#F0F7FF80"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 1px 0px 0px 0px
  card:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.surface-container}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 16px
  link:
    textColor: "{colors.background}"
---

# Checkout.com Design System

## Overview

Checkout.com describes itself as: “Boost your acceptance rate, cut processing costs, fight fraud, and create extraordinary customer experiences with Checkout.com's payment solutions.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Vivid Blue (#186AFF)** as the main accent.

Type is set in **Inter**, with **Checkout Apercu SemiMono** for code. Headlines run large; body text is 18px. The surface language is flat. Controls are pill-shaped.

Measured from [checkout.com](https://www.checkout.com/) on November 4, 2026 at 1440×900 and 390×844 from 340 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **Near Black (#000000):** Page background, seen 23 times. Token `background`, CSS `--component-library-checkout-x-flowninja-2026_theme---color--text--body--strong`.
- **White (#FFFFFF):** Primary text and headings, seen 30 times. Token `on-surface`, CSS `--rb-neutral`.
- **Charcoal (#181818):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Cool Graphite (#272932):** Cards and panels, seen 2 times. Token `surface-container`.
- **Vivid Blue (#186AFF):** Primary buttons and calls to action, seen 13 times. Token `primary`, CSS `--component-library-checkout-x-flowninja-2026_theme---color--surface--button--tertiary-hover`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#006CFF):** Accent in the logo, seen 1 time. Token `secondary`.

## Typography

**Checkout Apercu SemiMono** (monospace) and **Inter** share the interface. Fallback stack: `Checkout Apercu SemiMono, Arial, sans-serif`.

- **headline-display:** Checkout Apercu SemiMono 80px at weight 700, line height 0.9, uppercase (40px on mobile). Page title (h1).
- **headline-lg:** Inter 32px at weight 500, line height 1.18, tracking -0.03em. Section headings (h2).
- **headline-md:** Inter 24px at weight 500, line height 1.33 (20px on mobile). Sub-section headings.
- **body-md:** Inter 18px at weight 400, line height 1.44. Body text.
- **body-sm:** Inter 16px at weight 400, line height 1.5. Secondary and small text.
- **caption:** Inter 14px at weight 400, line height 1.71, tracking 0.05em. Captions and fine print.
- **label-lg:** Inter 16px at weight 500, line height 1.37. Large buttons and tabs.
- **label-md:** Inter 14px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Inter 11px at weight 500, line height 2. Small labels and badges.
- **code:** Checkout Apercu SemiMono 48px at weight 700, line height 0.9, tracking -0.04em, uppercase. Code and technical values.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 425px, 426px, 479px, 500px, 550px, 600px, 640px, 767px, 768px, 896px, 991px, 992px, 1440px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#181818 → #272932).

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **xl (24px):** 88 elements.
- **lg (16px):** 72 elements.
- **full (9999px):** 56 elements.
- **sm (6px):** 32 elements.
- **md (12px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Products”):** #186AFF fill, #FFFFFF text, 16px/500, padding 12px 0px.
- **button-outline (“Sign in”):** transparent fill, #FFFFFF text, 14px/500, 6px radius, padding 11px 23px, border 1px solid #FFFFFF.
- **button-outline-hover:** background #F0F7FF80, text #FFFFFF on hover.
- **button-ghost (“Business”):** transparent fill, #FFFFFF text, 11px/500, padding 1px 0px 0px 0px.
- **card:** #FFFFFF fill, #272932 text, 18px/400, 24px radius, padding 16px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #181818, #272932.
- Do reserve #186AFF for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 24px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Checkout Apercu SemiMono and Inter.
- Don't use #186AFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.25s, 0.1s.

- **Easing:** `ease`, `cubic-bezier(0.23, 1, 0.32, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/checkout.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
