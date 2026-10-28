---
version: alpha
name: Apple
description: "Light interface measured from apple.com: SF Pro Display type with SF Pro Text, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#F5F5F7"
  surface: "#F5F5F7"
  on-surface: "#1D1D1F"
  on-background: "#1D1D1F"
  on-surface-variant: "#313131"
  on-surface-muted: "#444445"
  on-surface-subtle: "#6E6E73"
  surface-container-low: "#FAFAFC"
  surface-container: "#FFFFFF"
  overlay: "#0000007A"
  overlay-strong: "#D2D2D7A3"
  outline: "#0000000A"
  outline-variant: "#00000029"
  primary: "#0071E3"
  on-primary: "#FFFFFF"
  inverse-surface: "#000000"
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
  sm: 8px
  md: 11px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 9.6px
  lg: 21px
  gutter: 12px
  section: 114px
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
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 15px
    height: 36px
  button-secondary-hover:
    backgroundColor: "#272729"
  button-outline:
    textColor: "{colors.secondary}"
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
    textColor: "#000000B8"
---

# Apple Design System

## Overview

The interface is light, built on **Snow (#F5F5F7)** with **Charcoal (#1D1D1F)** text, and **Vivid Blue (#0071E3)** as the main accent.

Type is set in **SF Pro Display** and **SF Pro Text**. Headlines run large with tight negative tracking; body text is 21px. The surface language is flat. Controls are pill-shaped.

Measured from [apple.com](https://www.apple.com/) on October 21, 2026 at 1440×900 and 390×844 from 386 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles.

- **Snow (#F5F5F7):** Page background, seen 1 time. Token `background`, CSS `--sk-fill-tertiary`.
- **Charcoal (#1D1D1F):** Primary text and headings, seen 15 times. Token `on-surface`, CSS `--sk-body-text-color`.
- **Graphite (#313131):** Secondary text, seen 15 times. Token `on-surface-variant`.
- **Graphite (#444445):** Muted text and metadata, seen 21 times. Token `on-surface-muted`, CSS `--sk-glyph-gray-secondary-alt-alpha`.
- **Slate (#6E6E73):** Subtle text and placeholders, seen 2 times. Token `on-surface-subtle`.
- **Snow (#FAFAFC):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--r-globalnav-background-opened`.
- **White (#FFFFFF):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--sk-fill`.
- **Near Black 48% (#0000007A):** Translucent fill for cards and controls, seen 7 times. Token `overlay`.
- **Silver 64% (#D2D2D7A3):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Near Black 4% (#0000000A):** Borders and dividers, seen 1 time. Token `outline`.
- **Near Black 16% (#00000029):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--sk-fill-gray-tertiary-alpha`.
- **Vivid Blue (#0071E3):** Primary buttons and calls to action, seen 9 times. Token `primary`, CSS `--sk-focus-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000000):** High-contrast fills, seen 19 times. Token `inverse-surface`, CSS `--sk-focus-color-alt`.
- **Blue (#0066CC):** Most used accent color, seen 15 times. Token `secondary`, CSS `--sk-body-link-color`.
- **Vivid Blue (#2997FF):** Most used accent color, seen 9 times. Token `tertiary`.

## Typography

**SF Pro Display** and **SF Pro Text** share the interface. Fallback stack: `SF Pro Display, SF Pro Icons, Helvetica Neue, Helvetica`. Other loaded fonts: SF Pro Icons.

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

- **Scale:** xs 4px, sm 8px, md 9.6px, lg 21px.
- **Sections:** 114px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 2560px.
- **Page margin:** 12px on each side of full-width sections.
- **Breakpoints:** 480px, 640px, 641px, 734px, 833px, 834px, 1023px, 1044px, 1068px, 1441px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FAFAFC → #FFFFFF) and #0000000A borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 68 elements.
- **sm (8px):** 4 elements.
- **md (11px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Learn more”):** #0071E3 fill, #FFFFFF text, 17px/400, 980px radius, padding 11px 21px.
- **button-primary-hover:** background #0076DF, text #FFFFFF on hover.
- **button-secondary (“Continue”):** #1D1D1F fill, #FFFFFF text, 14px/400, 8px radius, padding 8px 15px.
- **button-secondary-hover:** background #272729, text #FFFFFF on hover.
- **button-outline (“Pre-order”):** transparent fill, #0066CC text, 17px/400, 980px radius, padding 11px 21px, border 1px solid #0066CC.
- **button-ghost (“0 +”):** transparent fill, #000000CC text, 12px/400, padding 0px 8px.
- **link:** transparent fill, #000000B8 text, padding 0px.

## Do's and Don'ts

- Do use #F5F5F7 for the page and lift surfaces in small steps: #FAFAFC, #FFFFFF.
- Do keep text in 4 levels: #1D1D1F, #313131, #444445, #6E6E73.
- Do reserve #0071E3 for primary actions and key highlights.
- Do set headlines in SF Pro Display with tight tracking (-0.005em).
- Do reuse the measured spacing steps (8px, 9.6px, 21px).
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond SF Pro Display and SF Pro Text.
- Don't use #0071E3 for large backgrounds or body text.
- Don't make interface transitions slower than 0.32s.

## Motion

Interface transitions are quick: 0.32s, 0.25s, 0.24s, 0.1s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.6, 1)`, `ease-in-out`, `linear`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/apple.com/), the free DESIGN.md generator.
