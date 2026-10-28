---
version: alpha
name: DeepL
description: "Light interface measured from deepl.com: robotoLatin type, deep blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#191919"
  on-background: "#191919"
  on-surface-variant: "#091A2B"
  on-surface-muted: "#0A1B2C"
  on-surface-subtle: "#292929"
  surface-container-low: "#F8F8F8"
  surface-container: "#DEFDEE"
  surface-container-high: "#F5F5F5"
  surface-container-highest: "#DEF5FF"
  overlay: "#FFFFFF4D"
  primary: "#0F2B46"
  on-primary: "#F5F5F5"
  secondary: "#42A2FF"
  tertiary: "#0070C9"
  success: "#004730"
typography:
  display-hero:
    fontFamily: robotoLatin
    fontSize: 56px
    fontWeight: 300
    lineHeight: 1.05
    letterSpacing: -0.021em
  headline-display:
    fontFamily: robotoLatin
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.05
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: robotoLatin
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.05
    letterSpacing: -0.018em
  headline-md:
    fontFamily: robotoLatin
    fontSize: 28px
    fontWeight: 300
    lineHeight: 1.15
    letterSpacing: -0.017em
  body-md:
    fontFamily: robotoLatin
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: robotoLatin
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.4
  label-md:
    fontFamily: robotoLatin
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: robotoLatin
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: robotoLatin
    fontSize: 28px
    fontWeight: 300
    lineHeight: 1.15
    letterSpacing: -0.017em
rounded:
  sm: 8px
  md: 12px
  lg: 16px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 6px 12px
    height: 32px
  button-secondary:
    backgroundColor: "#3B435C"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 12px 20px
    height: 48px
  button-secondary-hover:
    backgroundColor: "#474E66"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 4px 0px 0px 0px
  card:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "#3B435C"
---

# DeepL Design System

## Overview

DeepL describes itself as: “Explore our AI suite and get more done: Translate speech, text, and media, or integrate the DeepL API.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#191919)** text, and **Deep Blue (#0F2B46)** as the main accent.

Type is set in **robotoLatin**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [deepl.com](https://www.deepl.com/en) on October 21, 2026 at 1440×900 and 390×844 from 434 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **White (#FFFFFF):** Page background, seen 15 times. Token `background`.
- **Charcoal (#191919):** Primary text and headings, seen 11 times. Token `on-surface`.
- **Deep Blue (#091A2B):** Secondary text, seen 11 times. Token `on-surface-variant`.
- **Deep Blue (#0A1B2C):** Muted text and metadata, seen 3 times. Token `on-surface-muted`.
- **Graphite (#292929):** Subtle text and placeholders, seen 27 times. Token `on-surface-subtle`.
- **Snow (#F8F8F8):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Pale Teal (#DEFDEE):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--dui-color-green-50-hex`.
- **Snow (#F5F5F5):** Hover and pressed fills, seen 1 time. Token `surface-container-high`, CSS `--dui-color-background-action-basic-raised-hover`.
- **Pale Cyan (#DEF5FF):** Highest raised elements, seen 11 times. Token `surface-container-highest`.
- **White 30% (#FFFFFF4D):** Translucent fill for cards and controls, seen 34 times. Token `overlay`.
- **Deep Blue (#0F2B46):** Primary buttons and calls to action, seen 29 times. Token `primary`.
- **Snow (#F5F5F5):** Text and icons on primary. Token `on-primary`.
- **Blue (#42A2FF):** Most used accent color, seen 15 times. Token `secondary`.
- **Blue (#0070C9):** Most used accent color, seen 14 times. Token `tertiary`, CSS `--dui-color-chart-status-info`.
- **Deep Teal (#004730):** Success and positive states, seen 1 time. Token `success`.

## Typography

**robotoLatin** carries the whole interface. Fallback stack: `robotoLatin, robotoLatin Fallback, sans-serif`. Other loaded fonts: robotoLatin Fallback.

- **display-hero:** robotoLatin 56px at weight 300, line height 1.05, tracking -0.021em. Oversized hero statements.
- **headline-display:** robotoLatin 48px at weight 300, line height 1.05, tracking -0.02em (28px on mobile). Page title (h1).
- **headline-lg:** robotoLatin 40px at weight 300, line height 1.05, tracking -0.018em. Section headings (h2).
- **headline-md:** robotoLatin 28px at weight 300, line height 1.15, tracking -0.017em. Sub-section headings.
- **body-md:** robotoLatin 16px at weight 400, line height 1.5. Body text.
- **body-lg:** robotoLatin 24px at weight 400, line height 1.4. Lead paragraphs.
- **label-md:** robotoLatin 16px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** robotoLatin 14px at weight 600, line height 1.43. Small labels and badges.

## Layout

Spacing follows a 4px grid: 91% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 512px, 767px, 869px, 1023px, 1280px, 1400px, 1615px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 4px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 216 elements.
- **sm (8px):** 160 elements.
- **md (12px):** 20 elements.
- **lg (16px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Close”):** #0F2B46 fill, #F5F5F5 text, 14px/600, 8px radius, padding 6px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 1px inset`.
- **button-secondary (“Contact Sales”):** #3B435C fill, #FFFFFF text, 16px/600, 8px radius, padding 12px 20px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 1px inset`.
- **button-secondary-hover:** background #474E66, text #FFFFFF on hover.
- **button-ghost (“Products”):** transparent fill, #191919 text, 16px/500, padding 4px 0px 0px 0px.
- **card:** #091A2B fill, #191919 text, 16px/400, 16px radius, padding 0px.
- **link:** transparent fill, #3B435C text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8F8F8, #DEFDEE, #F5F5F5, #DEF5FF.
- Do keep text in 4 levels: #191919, #091A2B, #0A1B2C, #292929.
- Do reserve #0F2B46 for primary actions and key highlights.
- Do set headlines in robotoLatin with tight tracking (-0.02em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't introduce new font families beyond robotoLatin.
- Don't use #0F2B46 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.25s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/deepl.com/), the free DESIGN.md generator.
