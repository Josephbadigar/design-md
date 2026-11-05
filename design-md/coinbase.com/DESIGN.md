---
version: alpha
name: Coinbase
description: "Light interface measured from coinbase.com: CoinbaseDisplay type with CoinbaseSans, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#5B616E"
  on-background: "#5B616E"
  on-surface-strong: "#0A0B0D"
  on-surface-variant: "#8A919E"
  surface-container-low: "#EEF0F3"
  primary: "#0052FF"
  on-primary: "#FFFFFF"
  success: "#27AD75"
typography:
  headline-display:
    fontFamily: CoinbaseDisplay
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
  headline-lg:
    fontFamily: CoinbaseDisplay
    fontSize: 52px
    fontWeight: 400
    lineHeight: 1
  headline-md:
    fontFamily: CoinbaseDisplay
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1.09
  headline-sm:
    fontFamily: CoinbaseSans
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.11
  title-lg:
    fontFamily: CoinbaseSans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.4
  body-md:
    fontFamily: CoinbaseText
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: CoinbaseText
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-sm:
    fontFamily: CoinbaseText
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.54
  label-md:
    fontFamily: CoinbaseSans
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.15
  headline-display-mobile:
    fontFamily: CoinbaseDisplay
    fontSize: 52px
    fontWeight: 400
    lineHeight: 1
  headline-md-mobile:
    fontFamily: CoinbaseDisplay
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.11
rounded:
  sm: 40px
  md: 56px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  md: 12px
  lg: 32px
  gutter: 12px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 24px
    height: 44px
  button-primary-hover:
    backgroundColor: "#0048E0E0"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 16px 32px
    height: 56px
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px
    height: 44px
  input-field:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 16px
  link:
    textColor: "{colors.on-surface}"
---

# Coinbase Design System

## Overview

Coinbase describes itself as: “Coinbase is a secure online platform for buying, selling, transferring, and storing cryptocurrency.” The interface is light, built on **White (#FFFFFF)** with **Cool Slate (#5B616E)** text, and **Vivid Blue (#0052FF)** as the main accent.

Type is set in **CoinbaseDisplay** and **CoinbaseSans**. Headlines run large; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [coinbase.com](https://www.coinbase.com/) on November 4, 2026 at 1440×900 and 390×844 from 234 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **White (#FFFFFF):** Page background, seen 16 times. Token `background`.
- **Cool Slate (#5B616E):** Primary text and headings, seen 51 times. Token `on-surface`.
- **Charcoal (#0A0B0D):** Headings and emphasis, seen 30 times. Token `on-surface-strong`.
- **Cool Gray (#8A919E):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Mist (#EEF0F3):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`.
- **Vivid Blue (#0052FF):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Teal (#27AD75):** Success and positive states, seen 4 times. Token `success`.

## Typography

**CoinbaseDisplay**, **CoinbaseSans** and **CoinbaseText** share the interface. Fallback stack: `CoinbaseDisplay, -apple-system, BlinkMacSystemFont, Segoe UI`. Other loaded fonts: CoinbaseIcons.

- **headline-display:** CoinbaseDisplay 80px at weight 400, line height 1 (52px on mobile). Page title (h1).
- **headline-lg:** CoinbaseDisplay 52px at weight 400, line height 1. Section headings (h2).
- **headline-md:** CoinbaseDisplay 44px at weight 400, line height 1.09 (36px on mobile). Sub-section headings.
- **headline-sm:** CoinbaseSans 36px at weight 400, line height 1.11. Card and feature titles.
- **title-lg:** CoinbaseSans 20px at weight 600, line height 1.4. Small titles.
- **body-md:** CoinbaseText 16px at weight 400, line height 1.5. Body text.
- **body-lg:** CoinbaseText 18px at weight 400, line height 1.56. Lead paragraphs.
- **body-sm:** CoinbaseText 13px at weight 400, line height 1.54. Secondary and small text.
- **label-md:** CoinbaseSans 16px at weight 600, line height 1.15. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 98% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, md 12px, lg 32px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 425px, 426px, 500px, 550px, 560px, 576px, 600px, 640px, 767px, 768px, 896px, 1024px, 1279px, 1280px, 1439px, 1600px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#EEF0F3).

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (56px):** 88 elements.
- **full (9999px):** 40 elements.
- **sm (40px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #0052FF fill, #FFFFFF text, 16px/600, 56px radius, padding 0px 24px.
- **button-primary-hover:** background #0048E0E0, text #FFFFFF on hover.
- **button-outline (“Claim your VIP3”):** #FFFFFF fill, #0A0B0D text, 16px/600, 56px radius, padding 16px 32px.
- **button-ghost (“󰝊”):** #EEF0F3 fill, #0A0B0D text, 16px/600, 56px radius, padding 0px.
- **input-field (“satoshi@nakamoto.com”):** transparent fill, #0A0B0D text, 16px/400, padding 16px.
- **link:** transparent fill, #5B616E text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #EEF0F3.
- Do keep text in 3 levels: #5B616E, #0A0B0D, #8A919E.
- Do reserve #0052FF for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 56px corners.
- Don't use #8A919E for body text; it reaches 3.17:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond CoinbaseDisplay, CoinbaseSans and CoinbaseText.
- Don't use #0052FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s.

- **Easing:** `cubic-bezier(0.33, 0, 0, 1)`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/coinbase.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
