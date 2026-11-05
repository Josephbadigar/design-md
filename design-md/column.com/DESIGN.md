---
version: alpha
name: Column
description: "Light interface measured from column.com: SuisseIntl type with Inter, deep indigo accents, tonal surfaces and 8px corners."
colors:
  background: "#F6F6F8"
  surface: "#F6F6F8"
  on-surface: "#111A4A"
  on-background: "#111A4A"
  on-surface-strong: "#12161E"
  on-surface-variant: "#7C7F88"
  on-surface-muted: "#A9ACB6"
  surface-container-low: "#FFFFFF"
  overlay: "#111A4A08"
  overlay-strong: "#FFFFFF80"
  outline: "#FFFFFF"
  primary: "#111A4A"
  on-primary: "#FFFFFF"
  secondary: "#44B48B"
  tertiary: "#9F7AEE"
typography:
  headline-display:
    fontFamily: SuisseIntl
    fontSize: 52px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: SuisseIntl
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: -0.03em
  headline-sm:
    fontFamily: SuisseIntl
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.01em
  body-md:
    fontFamily: SuisseIntl
    fontSize: 14px
    fontWeight: 300
    lineHeight: 1.5
  body-lg:
    fontFamily: SuisseIntl
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.38
  body-sm:
    fontFamily: SuisseIntl
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.1
  label-lg:
    fontFamily: SuisseIntl
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: SuisseIntl
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.01em
  label-sm:
    fontFamily: SuisseIntl
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.5
  code:
    fontFamily: SuisseIntlMono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: SuisseIntl
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.01em
rounded:
  md: 8px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 48px
  gutter: 12px
  section: 140px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 0px 16px
    height: 36px
  button-outline:
    backgroundColor: "{colors.overlay-strong}"
    textColor: "#232730"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 0px 16px
    height: 36px
  button-outline-hover:
    backgroundColor: "{colors.surface-container-low}"
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px 16px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Column Design System

## Overview

Column describes itself as: “The only nationally chartered bank built to enable developers and builders to create new financial services.” The interface is light, built on **Snow (#F6F6F8)** with **Deep Indigo (#111A4A)** text, and **Deep Indigo (#111A4A)** as the main accent.

Type is set in **SuisseIntl** and **Inter**, with **SuisseIntlMono** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [column.com](https://column.com/) on November 4, 2026 at 1440×900 and 390×844 from 333 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #3E5199, #5568AD.

- **Snow (#F6F6F8):** Page background, seen 1 time. Token `background`.
- **Deep Indigo (#111A4A):** Primary text and headings, seen 23 times. Token `on-surface`.
- **Cool Charcoal (#12161E):** Headings and emphasis, seen 5 times. Token `on-surface-strong`.
- **Cool Gray (#7C7F88):** Secondary text, seen 53 times. Token `on-surface-variant`, CSS `--text-color-duotone-secondary`.
- **Cool Gray (#A9ACB6):** Muted text and metadata, seen 6 times. Token `on-surface-muted`, CSS `--color-gray-400`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`, CSS `--color-white`.
- **Deep Indigo 3% (#111A4A08):** Translucent fill for cards and controls, seen 17 times. Token `overlay`.
- **White 50% (#FFFFFF80):** Stronger translucent fill, seen 4 times. Token `overlay-strong`.
- **White (#FFFFFF):** Borders and dividers, seen 4 times. Token `outline`, CSS `--color-white`.
- **Deep Indigo (#111A4A):** Primary buttons and calls to action, seen 51 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Teal (#44B48B):** Accent in text, fills and borders, seen 26 times. Token `secondary`.
- **Light Violet (#9F7AEE):** Accent in text, fills and borders, seen 2 times. Token `tertiary`.

## Typography

**SuisseIntl**, **Inter** and **SuisseIntlMono** (monospace) share the interface. Fallback stack: `SuisseIntl, ui-sans-serif, system-ui, -apple-system`.

- **headline-display:** SuisseIntl 52px at weight 600, line height 1.1, tracking -0.03em (32px on mobile). Page title (h1).
- **headline-lg:** SuisseIntl 28px at weight 500, line height 1.1, tracking -0.01em. Section headings (h2).
- **headline-md:** Inter 24px at weight 600, line height 1.5, tracking -0.03em. Sub-section headings.
- **headline-sm:** SuisseIntl 20px at weight 500, line height 1.1, tracking -0.01em. Card and feature titles.
- **body-md:** SuisseIntl 14px at weight 300, line height 1.5. Body text.
- **body-lg:** SuisseIntl 16px at weight 300, line height 1.38. Lead paragraphs.
- **body-sm:** SuisseIntl 12px at weight 400, line height 1.1. Secondary and small text.
- **label-lg:** SuisseIntl 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** SuisseIntl 14px at weight 500, line height 1.1, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** SuisseIntl 12px at weight 500, line height 1.5. Small labels and badges.
- **code:** SuisseIntlMono 12px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing follows a 4px grid: 96% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 32px, xl 48px.
- **Sections:** 140px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 374px, 479px, 480px, 640px, 768px, 870px, 1024px, 1112px, 1200px, 1280px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.05) 0px 4px 8px 0px, rgba(0, 0, 0, 0.1) 0px 2px 4px 0px, rgba(0, 0, 0, 0.1) 0px 1px 1px 0px`
- `rgba(0, 0, 0, 0.1) 0px 1px 2px 0px`
- `rgb(17, 26, 74) 0px 0px 0px 1px, rgba(0, 0, 0, 0.25) 0px 2px 4px 0px, rgba(0, 0, 0, 0.25) 0px 1px 2px 0px`

Hairline rings and inset highlights also appear: `rgba(255, 255, 255, 0) 0px 1px 1px 0px, rgba(87, 90, 100, 0.12) 0px 0px 0px 1px`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 152 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #111A4A fill, #FFFFFF text, 16px/500, 8px radius, padding 0px 16px, shadow `rgb(17, 26, 74) 0px 0px 0px 1px, rgba(0, 0, 0, 0.25) 0px 2px 4px 0px, rgba(0, 0, 0, 0.25) 0px 1px 2px 0px`.
- **button-outline (“Get started”):** #FFFFFF80 fill, #232730 text, 16px/500, 8px radius, padding 0px 16px, shadow `rgba(255, 255, 255, 0) 0px 1px 1px 0px, rgba(87, 90, 100, 0.12) 0px 0px 0px 1px`.
- **button-outline-hover:** background #FFFFFF, text #232730 on hover.
- **button-ghost (“Products”):** transparent fill, #12161E text, 14px/500, 8px radius, padding 8px 16px.
- **link:** transparent fill, #7C7F88 text, padding 0px.

## Do's and Don'ts

- Do use #F6F6F8 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 4 levels: #111A4A, #12161E, #7C7F88, #A9ACB6.
- Do reserve #111A4A for primary actions and key highlights.
- Do set headlines in SuisseIntl with tight tracking (-0.03em).
- Do keep spacing on the 4px grid.
- Do use 8px corners on most elements.
- Don't use #7C7F88 for body text; it reaches 3.71:1 on #F6F6F8. Keep it for large text or metadata.
- Don't use #A9ACB6 for body text; it reaches 2.10:1 on #F6F6F8. Keep it for large text or metadata.
- Don't introduce new font families beyond SuisseIntl, Inter and SuisseIntlMono.
- Don't use #111A4A for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.5s, 0.1s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.76, 0, 0.24, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/column.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
