---
version: alpha
name: Google Fonts
description: "Light interface measured from fonts.google.com: Arial type with Google Sans Flex, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#444746"
  on-background: "#444746"
  on-surface-strong: "#1F1F1F"
  surface-container-low: "#F8FAFD"
  surface-container: "#E9EEF6"
  primary: "#0B57D0"
  on-primary: "#FFFFFF"
  secondary: "#C2E7FF"
  tertiary: "#1A73E8"
typography:
  headline-display:
    fontFamily: Arial
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1
  body-md:
    fontFamily: Google Sans Flex
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: Google Sans Flex
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Google Sans Flex
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
rounded:
  sm: 16px
  md: 24px
  lg: 50px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 60px
  gutter: 24px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px 24px 0px 16px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-display}"
    rounded: "{rounded.full}"
    padding: 10px
  input-field:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 16px
  link:
    textColor: "{colors.on-surface-strong}"
---

# Google Fonts Design System

## Overview

Google Fonts describes itself as: “Making the web more beautiful, fast, and open through great typography” The interface is light, built on **White (#FFFFFF)** with **Graphite (#444746)** text, and **Vivid Blue (#0B57D0)** as the main accent.

Type is set in **Arial** and **Google Sans Flex**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [fonts.google.com](https://fonts.google.com/) on November 4, 2026 at 1440×900 and 390×844 from 311 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **White (#FFFFFF):** Page background. Token `background`.
- **Graphite (#444746):** Primary text and headings, seen 8 times. Token `on-surface`.
- **Charcoal (#1F1F1F):** Headings and emphasis, seen 3 times. Token `on-surface-strong`.
- **Snow (#F8FAFD):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **Cool Mist (#E9EEF6):** Cards and panels, seen 2 times. Token `surface-container`.
- **Vivid Blue (#0B57D0):** Primary buttons and calls to action, seen 4 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Pale Blue (#C2E7FF):** Accent in the header, seen 7 times. Token `secondary`.
- **Vivid Blue (#1A73E8):** Accent, seen 5 times. Token `tertiary`.

## Typography

**Arial** and **Google Sans Flex** share the interface. Fallback stack: `Arial`. Other loaded fonts: Google Symbols Subset Subset, Tofu, Google Symbols Category Filters, gf_DynaPuff variant0.

- **headline-display:** Arial 24px at weight 400, line height 1. Page title (h1).
- **body-md:** Google Sans Flex 14px at weight 400, line height 1.43. Body text.
- **label-md:** Google Sans Flex 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Google Sans Flex 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing follows a 4px grid: 98% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 60px.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Breakpoints:** 720px, 721px, 960px, 1024px, 1025px, 1240px, 1246px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.2) 0px 3px 5px -1px, rgba(0, 0, 0, 0.14) 0px 6px 10px 0px, rgba(0, 0, 0, 0.12) 0px 1px 18px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 44 elements.
- **md (24px):** 28 elements.
- **sm (16px):** 24 elements.
- **lg (50px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“close Filters”):** #0B57D0 fill, #FFFFFF text, 14px/600, 50px radius, padding 0px 24px 0px 16px.
- **button-ghost (“dark_mode”):** transparent fill, #444746 text, 24px/400, 9999px radius, padding 10px.
- **input-field (“Type something”):** #E9EEF6 fill, #1F1F1F text, 16px/400, 16px radius, padding 16px.
- **link:** transparent fill, #1F1F1F text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8FAFD, #E9EEF6.
- Do keep text in 2 levels: #444746, #1F1F1F.
- Do reserve #0B57D0 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 24px corners.
- Don't introduce new font families beyond Arial and Google Sans Flex.
- Don't use #0B57D0 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s.

- **Easing:** `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/fonts.google.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
