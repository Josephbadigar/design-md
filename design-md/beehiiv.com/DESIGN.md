---
version: alpha
name: beehiiv
description: "Dark interface measured from beehiiv.com: ClashGroteskFont type with SatoshiFont, indigo accents, tonal surfaces and 6px corners."
colors:
  background: "#060419"
  surface: "#060419"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#F7F5FF"
  on-surface-muted: "#DDDCE8"
  on-surface-subtle: "#9393A9"
  surface-container-low: "#0D0B28"
  outline: "#FFFFFF0F"
  outline-variant: "#FFFFFF33"
  primary: "#2F39BA"
  on-primary: "#FFFFFF"
  secondary: "#FF5EC4"
  tertiary: "#511F4D"
typography:
  display-hero:
    fontFamily: ClashGroteskFont
    fontSize: 64px
    fontWeight: 700
    lineHeight: 1.06
  headline-display:
    fontFamily: ClashGroteskFont
    fontSize: 60px
    fontWeight: 700
    lineHeight: 1
  headline-lg:
    fontFamily: ClashGroteskFont
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1
  headline-md:
    fontFamily: SatoshiFont
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
  headline-sm:
    fontFamily: SatoshiFont
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.33
  title-lg:
    fontFamily: SatoshiFont
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.4
  body-md:
    fontFamily: SatoshiFont
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.56
  label-lg:
    fontFamily: SatoshiFont
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
  label-md:
    fontFamily: SatoshiFont
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  label-sm:
    fontFamily: SatoshiFont
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
  headline-display-mobile:
    fontFamily: ClashGroteskFont
    fontSize: 42px
    fontWeight: 700
    lineHeight: 1.05
  headline-lg-mobile:
    fontFamily: ClashGroteskFont
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.11
rounded:
  sm: 6px
  md: 8px
  lg: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 64px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 0px
    height: 50px
  button-outline:
    backgroundColor: "#131125"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 0px
    height: 50px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
    height: 36px
  button-ghost:
    textColor: "#000000"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  input-field:
    textColor: "#000000"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#000000"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# beehiiv Design System

## Overview

beehiiv describes itself as: “beehiiv is the newsletter platform built for creators, publishers, and businesses. Grow, publish, and monetize your audience in one place.” The interface is dark, built on **Deep Indigo (#060419)** with **White (#FFFFFF)** text, and **Indigo (#2F39BA)** as the main accent.

Type is set in **ClashGroteskFont** and **SatoshiFont**. Headlines run large; body text is 18px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 6px.

Measured from [beehiiv.com](https://www.beehiiv.com/) on November 4, 2026 at 1440×900 and 390×844 from 435 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #FFDCFF, #FF5EC4.

- **Deep Indigo (#060419):** Page background, seen 12 times. Token `background`, CSS `--surface-page`.
- **White (#FFFFFF):** Primary text and headings, seen 51 times. Token `on-surface`, CSS `--tw-ring-offset-color`.
- **Cool Snow (#F7F5FF):** Secondary text, seen 8 times. Token `on-surface-variant`, CSS `--text-secondary`.
- **Cool Mist (#DDDCE8):** Muted text and metadata, seen 5 times. Token `on-surface-muted`, CSS `--action-ghost-text`.
- **Indigo (#9393A9):** Subtle text and placeholders, seen 32 times. Token `on-surface-subtle`.
- **Deep Indigo (#0D0B28):** Raised areas one step from the page, seen 24 times. Token `surface-container-low`, CSS `--surface-1`.
- **White 6% (#FFFFFF0F):** Borders and dividers, seen 11 times. Token `outline`, CSS `--border-subtle`.
- **White 20% (#FFFFFF33):** Secondary dividers, seen 3 times. Token `outline-variant`, CSS `--border-strong`.
- **Indigo (#2F39BA):** Primary buttons and calls to action, seen 5 times. Token `primary`, CSS `--button-primary-fill`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Pink (#FF5EC4):** Accent (CSS variable), seen 8 times. Token `secondary`, CSS `--button-accent-fill`.
- **Deep Purple (#511F4D):** Accent (CSS variable). Token `tertiary`.

## Typography

**ClashGroteskFont** and **SatoshiFont** share the interface. Fallback stack: `ClashGroteskFont, ClashGroteskFont Fallback, sans-serif`.

- **display-hero:** ClashGroteskFont 64px at weight 700, line height 1.06. Oversized hero statements.
- **headline-display:** ClashGroteskFont 60px at weight 700, line height 1, uppercase (42px on mobile). Page title (h1).
- **headline-lg:** ClashGroteskFont 48px at weight 700, line height 1, uppercase (36px on mobile). Section headings (h2).
- **headline-md:** SatoshiFont 30px at weight 500, line height 1.2. Sub-section headings.
- **headline-sm:** SatoshiFont 24px at weight 700, line height 1.33. Card and feature titles.
- **title-lg:** SatoshiFont 20px at weight 700, line height 1.4. Small titles.
- **body-md:** SatoshiFont 18px at weight 500, line height 1.56. Body text.
- **label-lg:** SatoshiFont 16px at weight 700, line height 1.5. Large buttons and tabs.
- **label-md:** SatoshiFont 14px at weight 500, line height 1.43. Buttons, navigation and labels.
- **label-sm:** SatoshiFont 12px at weight 500, line height 1.33. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (86% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 600px, 639px, 640px, 650px, 768px, 1024px, 1280px, 1283px, 1284px, 1536px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#0D0B28) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(255, 94, 196) 0px 0px 0px 2px inset, rgb(6, 4, 25) 0px 0px 0px 4px inset`

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **sm (6px):** 168 elements.
- **lg (12px):** 120 elements.
- **md (8px):** 40 elements.
- **full (9999px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up with Google”):** #2F39BA fill, #FFFFFF text, 16px/400, 6px radius, padding 0px.
- **button-outline (“Sign up with email”):** #131125 fill, #FFFFFF text, 16px/400, 6px radius, padding 0px.
- **button-secondary (“Sign up for free”):** #FFFFFF fill, #060419 text, 14px/600, 6px radius, padding 8px 12px, border 1px solid #FFFFFF.
- **button-ghost (“Product”):** transparent fill, #000000 text, 16px/400, padding 0px.
- **input-field (“Subscribers”):** transparent fill, #000000 text, 16px/400, padding 0px.
- **card:** #0D0B28 fill, #000000 text, 16px/400, 12px radius, padding 0px, border 1px solid #FFFFFF0F.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #060419 for the page and lift surfaces in small steps: #0D0B28.
- Do keep text in 4 levels: #FFFFFF, #F7F5FF, #DDDCE8, #9393A9.
- Do reserve #2F39BA for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 6px corners on most elements; larger surfaces also use 12px and 8px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond ClashGroteskFont and SatoshiFont.
- Don't use #2F39BA for large backgrounds or body text.
- Don't make interface transitions slower than 0.35s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.35s, 0.125s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`, `cubic-bezier(0.65, 0, 0.35, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/beehiiv.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
