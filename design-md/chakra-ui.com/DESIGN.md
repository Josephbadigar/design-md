---
version: alpha
name: Chakra UI
description: "Light interface measured from chakra-ui.com: Wix Madefor Text type, dark teal accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#09090B"
  on-background: "#09090B"
  on-surface-variant: "#27272A"
  on-surface-muted: "#52525B"
  on-surface-subtle: "#A1A1AA"
  surface-container-low: "#F4F4F5"
  surface-container: "#E4E4E7"
  overlay: "#00000029"
  overlay-strong: "#14B8A61A"
  outline: "#E4E4E7"
  outline-variant: "#14B8A6"
  primary: "#0D9488"
  on-primary: "#FFFFFF"
  secondary: "#9CDCFE"
  tertiary: "#0C5D56"
typography:
  headline-display:
    fontFamily: Wix Madefor Text
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1.28
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Wix Madefor Text
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Wix Madefor Text
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
  body-md:
    fontFamily: Wix Madefor Text
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Wix Madefor Text
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Wix Madefor Text
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Wix Madefor Text
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  headline-lg-mobile:
    fontFamily: Wix Madefor Text
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.22
    letterSpacing: -0.025em
rounded:
  sm: 4px
  md: 6px
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 48px
  gutter: 8px
  section: 80px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 20px
    height: 48px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.tertiary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
    height: 40px
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
    height: 40px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Chakra UI Design System

## Overview

Chakra UI describes itself as: “Simple, Modular & Accessible UI Components for your React Applications” The interface is light, built on **White (#FFFFFF)** with **Near Black (#09090B)** text, and **Dark Teal (#0D9488)** as the main accent.

Type is set in **Wix Madefor Text**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [chakra-ui.com](https://chakra-ui.com/) on November 4, 2026 at 1440×900 and 390×844 from 326 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`, CSS `--ring-offset-color`.
- **Near Black (#09090B):** Primary text and headings, seen 29 times. Token `on-surface`, CSS `--chakra-colors-bg-inverted`.
- **Graphite (#27272A):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Cool Slate (#52525B):** Muted text and metadata, seen 21 times. Token `on-surface-muted`, CSS `--chakra-colors-gray-600`.
- **Cool Gray (#A1A1AA):** Subtle text and placeholders, seen 2 times. Token `on-surface-subtle`, CSS `--chakra-colors-fg-subtle`.
- **Snow (#F4F4F5):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Mist (#E4E4E7):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--chakra-colors-gray-border`.
- **Near Black 16% (#00000029):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Teal 10% (#14B8A61A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Mist (#E4E4E7):** Borders and dividers, seen 85 times. Token `outline`, CSS `--chakra-colors-gray-border`.
- **Teal (#14B8A6):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Dark Teal (#0D9488):** Primary buttons and calls to action, seen 9 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Blue (#9CDCFE):** Accent in text, fills and borders, seen 12 times. Token `secondary`.
- **Deep Teal (#0C5D56):** Accent in text, fills and borders, seen 9 times. Token `tertiary`.

## Typography

**Wix Madefor Text** carries the whole interface. Fallback stack: `Wix Madefor Text, Wix Madefor Text Fallback`. Other loaded fonts: geistMono.

- **headline-display:** Wix Madefor Text 72px at weight 500, line height 1.28, tracking -0.025em. Page title (h1).
- **headline-lg:** Wix Madefor Text 48px at weight 600, line height 1.25, tracking -0.025em (36px on mobile). Section headings (h2).
- **headline-md:** Wix Madefor Text 20px at weight 400, line height 1.5. Sub-section headings.
- **body-md:** Wix Madefor Text 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Wix Madefor Text 14px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Wix Madefor Text 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Wix Madefor Text 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing follows a 8px grid: 91% of measured gaps and paddings are multiples of 8px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 48px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `color(srgb 0.0941176 0.0941176 0.105882 / 0.1) 0px 2px 4px 0px, color(srgb 0.0941176 0.0941176 0.105882 / 0.3) 0px 0px 1px 0px`
- `color(srgb 0.0941176 0.0941176 0.105882 / 0.1) 0px 1px 2px 0px, color(srgb 0.0941176 0.0941176 0.105882 / 0.2) 0px 0px 1px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 72 elements.
- **md (6px):** 20 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start Building”):** #0D9488 fill, #FFFFFF text, 16px/500, 4px radius, padding 0px 20px.
- **button-outline (“Chakra”):** #FFFFFF fill, #0C5D56 text, 14px/500, 4px radius, padding 8px 16px, shadow `color(srgb 0.0941176 0.0941176 0.105882 / 0.1) 0px 1px 2px 0px, color(srgb 0.0941176 0.0941176 0.105882 / 0.2) 0px 0px 1px 0px`.
- **button-ghost (“Tokens”):** #F4F4F5 fill, #27272A text, 14px/500, 4px radius, padding 8px 16px.
- **input-field:** #FFFFFF fill, #09090B text, 16px/400, padding 0px.
- **link:** transparent fill, #09090B text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F4F4F5, #E4E4E7.
- Do keep text in 4 levels: #09090B, #27272A, #52525B, #A1A1AA.
- Do reserve #0D9488 for primary actions and key highlights.
- Do set headlines in Wix Madefor Text with tight tracking (-0.025em).
- Do keep spacing on the 8px grid.
- Do use 4px corners on most elements; larger surfaces also use 6px.
- Don't use #A1A1AA for body text; it reaches 2.56:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Wix Madefor Text.
- Don't use #0D9488 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/chakra-ui.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
