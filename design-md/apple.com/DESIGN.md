---
version: alpha
name: Apple
description: "Dark interface measured from apple.com: SF Pro Display type with SF Pro Text, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#F5F5F7"
  on-background: "#F5F5F7"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#CCCCCC"
  on-surface-muted: "#86868B"
  surface-container-low: "#1D1D1F"
  overlay: "#0000007A"
  overlay-strong: "#D2D2D7A3"
  outline: "#00000029"
  primary: "#0071E3"
  on-primary: "#FFFFFF"
  secondary: "#0066CC"
  tertiary: "#2997FF"
typography:
  headline-display:
    fontFamily: SF Pro Display
    fontSize: 56px
    fontWeight: 600
    lineHeight: 1.07
    letterSpacing: -0.005em
  headline-lg:
    fontFamily: SF Pro Display
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.1
  headline-md:
    fontFamily: SF Pro Text
    fontSize: 34px
    fontWeight: 600
    lineHeight: 1.47
    letterSpacing: -0.011em
  headline-sm:
    fontFamily: SF Pro Display
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.14
    letterSpacing: 0.007em
  body-md:
    fontFamily: SF Pro Display
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1.19
    letterSpacing: 0.011em
  body-sm:
    fontFamily: SF Pro Text
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: -0.01em
  label-md:
    fontFamily: SF Pro Text
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.47
    letterSpacing: -0.022em
  label-sm:
    fontFamily: SF Pro Text
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.29
    letterSpacing: -0.016em
  headline-display-mobile:
    fontFamily: SF Pro Display
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.13
    letterSpacing: 0.002em
rounded:
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 9.6px
  lg: 21px
  xl: 33.22px
  gutter: 12px
  margin: 12px
  container: 2560px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 11px 21px
    height: 44px
  button-primary-hover:
    backgroundColor: "#0076DF"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 11px 21px
    height: 44px
  button-secondary-hover:
    backgroundColor: "{colors.on-surface-strong}"
  button-outline:
    textColor: "{colors.tertiary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 11px 21px
    height: 44px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px 8px
  link:
    textColor: "{colors.background}"
---

# Apple Design System

## Overview

The interface is dark, built on **Near Black (#000000)** with **Snow (#F5F5F7)** text, and **Vivid Blue (#0071E3)** as the main accent.

Type is set in **SF Pro Display** and **SF Pro Text**. Headlines run large with tight negative tracking; body text is 21px. The surface language is flat. Controls are pill-shaped.

Measured from [apple.com](https://www.apple.com/) on October 29, 2026 at 1440×900 and 390×844 from 385 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #FDD30F, #90CEEE, #48A7F4, #2789FF.

- **Near Black (#000000):** Page background, seen 19 times. Token `background`, CSS `--sk-focus-color-alt`.
- **Snow (#F5F5F7):** Primary text and headings, seen 34 times. Token `on-surface`, CSS `--sk-fill-tertiary`.
- **White (#FFFFFF):** Headings and emphasis, seen 9 times. Token `on-surface-strong`, CSS `--sk-fill`.
- **Silver (#CCCCCC):** Secondary text, seen 12 times. Token `on-surface-variant`.
- **Gray (#86868B):** Muted text and metadata, seen 2 times. Token `on-surface-muted`, CSS `--sk-fill-gray-secondary`.
- **Charcoal (#1D1D1F):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--sk-body-text-color`.
- **Near Black 48% (#0000007A):** Translucent fill for cards and controls, seen 7 times. Token `overlay`.
- **Silver 64% (#D2D2D7A3):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Near Black 16% (#00000029):** Borders and dividers, seen 1 time. Token `outline`, CSS `--sk-fill-gray-tertiary-alpha`.
- **Vivid Blue (#0071E3):** Primary buttons and calls to action, seen 9 times. Token `primary`, CSS `--sk-focus-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#0066CC):** Accent in text, fills and borders, seen 17 times. Token `secondary`, CSS `--sk-body-link-color`.
- **Vivid Blue (#2997FF):** Accent in text, fills and borders, seen 8 times. Token `tertiary`.

## Typography

**SF Pro Display** and **SF Pro Text** share the interface. Fallback stack: `SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica`.

- **headline-display:** SF Pro Display 56px at weight 600, line height 1.07, tracking -0.005em (32px on mobile). Page title (h1).
- **headline-lg:** SF Pro Display 40px at weight 600, line height 1.1. Section headings (h2).
- **headline-md:** SF Pro Text 34px at weight 600, line height 1.47, tracking -0.011em. Sub-section headings.
- **headline-sm:** SF Pro Display 28px at weight 400, line height 1.14, tracking 0.007em. Card and feature titles.
- **body-md:** SF Pro Display 21px at weight 400, line height 1.19, tracking 0.011em. Body text.
- **body-sm:** SF Pro Text 12px at weight 400, line height 1.33, tracking -0.01em. Secondary and small text.
- **label-md:** SF Pro Text 17px at weight 400, line height 1.47, tracking -0.022em. Buttons, navigation and labels.
- **label-sm:** SF Pro Text 14px at weight 600, line height 1.29, tracking -0.016em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 43% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 9.6px, lg 21px, xl 33.22px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 2560px.
- **Page margin:** 12px on each side of full-width sections.
- **Breakpoints:** 480px, 640px, 641px, 734px, 833px, 834px, 1023px, 1044px, 1068px, 1441px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#1D1D1F) and #00000029 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 76 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Learn more”):** #0071E3 fill, #FFFFFF text, 17px/400, 980px radius, padding 11px 21px.
- **button-primary-hover:** background #0076DF, text #FFFFFF on hover.
- **button-secondary (“Watch the film”):** #F5F5F7 fill, #000000 text, 17px/400, 980px radius, padding 11px 21px.
- **button-secondary-hover:** background #FFFFFF, text #000000 on hover.
- **button-outline (“Pre-order”):** transparent fill, #2997FF text, 17px/400, 980px radius, padding 11px 21px, border 1px solid #2997FF.
- **button-ghost (“0 +”):** transparent fill, #FFFFFFCC text, 12px/400, padding 0px 8px.
- **link:** transparent fill, #000000B8 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #1D1D1F.
- Do keep text in 4 levels: #F5F5F7, #FFFFFF, #CCCCCC, #86868B.
- Do reserve #0071E3 for primary actions and key highlights.
- Do set headlines in SF Pro Display with tight tracking (-0.005em).
- Do reuse the measured spacing steps (8px, 9.6px, 21px).
- Do make buttons and chips fully rounded (9999px).
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond SF Pro Display and SF Pro Text.
- Don't use #0071E3 for large backgrounds or body text.
- Don't make interface transitions slower than 0.32s.

## Motion

Interface transitions are quick: 0.32s, 0.25s, 0.1s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.6, 1)`, `ease-in-out`, `linear`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/apple.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
