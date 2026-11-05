---
version: alpha
name: Material Design
description: "Light interface measured from m3.material.io: Google Sans type with Google Sans Text, violet accents, tonal surfaces and 4px corners."
colors:
  background: "#F8F1F6"
  surface: "#F8F1F6"
  on-surface: "#4D4256"
  on-background: "#4D4256"
  on-surface-strong: "#1C1B1D"
  surface-container-low: "#DCDAF5"
  primary: "#6442D6"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: Google Sans
    fontSize: 96px
    fontWeight: 475
    lineHeight: 1
  headline-lg:
    fontFamily: Google Sans
    fontSize: 57px
    fontWeight: 475
    lineHeight: 1.12
  headline-md:
    fontFamily: Google Sans Text
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.36
  body-md:
    fontFamily: Google Sans Text
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Google Sans Text
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Google Sans Text
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Google Sans
    fontSize: 45px
    fontWeight: 475
    lineHeight: 1.16
  headline-lg-mobile:
    fontFamily: Google Sans
    fontSize: 36px
    fontWeight: 475
    lineHeight: 1.22
rounded:
  sm: 4px
  md: 16px
  lg: 24px
  xl: 48px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 10px
  lg: 20px
  xl: 64px
  gutter: 20px
  section: 64px
  margin: 40px
  container: 1200px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 1px
    height: 82px
  button-outline:
    backgroundColor: "#F1D3F9"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 2px
    height: 56px
  button-outline-hover:
    textColor: "#271430"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 2px
  link:
    textColor: "{colors.on-surface-strong}"
---

# Material Design Design System

## Overview

Material Design describes itself as: “Material Design 3 - Google's open-source design system, provides comprehensive guidelines, styles, & components to create user-friendly interfaces.” The interface is light, built on **Snow (#F8F1F6)** with **Dark Violet (#4D4256)** text, and **Violet (#6442D6)** as the main accent.

Type is set in **Google Sans** and **Google Sans Text**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [m3.material.io](https://m3.material.io/) on November 4, 2026 at 1440×900 and 390×844 from 204 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 6 roles.

- **Snow (#F8F1F6):** Page background, seen 20 times. Token `background`.
- **Dark Violet (#4D4256):** Primary text and headings, seen 33 times. Token `on-surface`.
- **Charcoal (#1C1B1D):** Headings and emphasis, seen 31 times. Token `on-surface-strong`.
- **Pale Indigo (#DCDAF5):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Violet (#6442D6):** Primary buttons and calls to action, seen 22 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**Google Sans** and **Google Sans Text** share the interface. Fallback stack: `Google Sans, sans-serif`. Other loaded fonts: Google Symbols.

- **headline-display:** Google Sans 96px at weight 475, line height 1 (45px on mobile). Page title (h1).
- **headline-lg:** Google Sans 57px at weight 475, line height 1.12 (36px on mobile). Section headings (h2).
- **headline-md:** Google Sans Text 22px at weight 400, line height 1.36. Sub-section headings.
- **body-md:** Google Sans Text 16px at weight 400, line height 1.5. Body text.
- **label-md:** Google Sans Text 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Google Sans Text 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 61% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 10px, lg 20px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1200px.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 600px, 601px, 960px, 961px, 1294px, 1295px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.3) 0px 1px 2px 0px, rgba(0, 0, 0, 0.15) 0px 1px 3px 1px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 120 elements.
- **lg (24px):** 80 elements.
- **md (16px):** 36 elements.
- **xl (48px):** 8 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #6442D6 fill, #FFFFFF text, 16px/500, 48px radius, padding 1px.
- **button-outline (“search”):** #F1D3F9 fill, #4D4256 text, 16px/500, 16px radius, padding 2px.
- **button-outline-hover:** background #F1D3F9, text #271430 on hover.
- **button-ghost (“code Develop”):** transparent fill, #4D4256 text, 16px/500, 4px radius, padding 2px.
- **link:** transparent fill, #1C1B1D text, padding 0px.

## Do's and Don'ts

- Do use #F8F1F6 for the page and lift surfaces in small steps: #DCDAF5.
- Do keep text in 2 levels: #4D4256, #1C1B1D.
- Do reserve #6442D6 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 10px, 20px).
- Do use 4px corners on most elements; larger surfaces also use 24px, 16px and 48px.
- Don't introduce new font families beyond Google Sans and Google Sans Text.
- Don't use #6442D6 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s.

- **Easing:** `cubic-bezier(0.2, 0, 0, 1)`, `linear`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/m3.material.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
