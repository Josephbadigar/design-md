---
version: alpha
name: Coolors
description: "Light interface measured from coolors.co: Inter type, vivid blue accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0A0A0A"
  on-background: "#0A0A0A"
  on-surface-strong: "#000000"
  on-surface-variant: "#525252"
  on-surface-muted: "#737373"
  surface-container-low: "#F5F5F5"
  surface-container: "#DCFCE7"
  surface-container-high: "#FCE7F3"
  surface-container-highest: "#F3E8FF"
  overlay: "#0000000F"
  outline: "#00000012"
  primary: "#2563EB"
  on-primary: "#FFFFFF"
  secondary: "#93C5FD"
  tertiary: "#1E40AF"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 110px
    fontWeight: 800
    lineHeight: 0.9
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: 800
    lineHeight: 1
    letterSpacing: -0.035em
  body-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 450
    lineHeight: 1
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 450
    lineHeight: 1.3
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
  label-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 500
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0.25em
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 60px
    fontWeight: 800
    lineHeight: 0.9
    letterSpacing: -0.035em
rounded:
  sm: 8px
  md: 10px
  lg: 14px
spacing:
  xs: 4px
  sm: 5px
  md: 10px
  lg: 30px
  xl: 40px
  gutter: 20px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 0px 21px
    height: 46px
  button-primary-hover:
    backgroundColor: "#1D4ED8"
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
  link:
    textColor: "{colors.on-surface}"
---

# Coolors Design System

## Overview

Coolors describes itself as: “Generate or browse beautiful color combinations for your designs.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#0A0A0A)** text, and **Vivid Blue (#2563EB)** as the main accent.

Type is set in **Inter**. Headlines run large with tight negative tracking; body text is 15px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [coolors.co](https://coolors.co/) on November 4, 2026 at 1440×900 and 390×844 from 237 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **White (#FFFFFF):** Page background, seen 3 times. Token `background`, CSS `--color-white`.
- **Near Black (#0A0A0A):** Primary text and headings, seen 76 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 4 times. Token `on-surface-strong`, CSS `--button-transparent-text`.
- **Slate (#525252):** Secondary text, seen 8 times. Token `on-surface-variant`, CSS `--color-neutral-600`.
- **Slate (#737373):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Snow (#F5F5F5):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`.
- **Pale Green (#DCFCE7):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--color-smart-green-100`.
- **Pale Pink (#FCE7F3):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Pale Violet (#F3E8FF):** Highest raised elements, seen 1 time. Token `surface-container-highest`.
- **Near Black 6% (#0000000F):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Near Black 7% (#00000012):** Borders and dividers, seen 2 times. Token `outline`.
- **Vivid Blue (#2563EB):** Primary buttons and calls to action, seen 4 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Blue (#93C5FD):** Accent (CSS variable). Token `secondary`.
- **Blue (#1E40AF):** Accent (CSS variable). Token `tertiary`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, sans-serif`. Other loaded fonts: Nucleo, InterFont.

- **headline-display:** Inter 110px at weight 800, line height 0.9, tracking -0.035em (60px on mobile). Page title (h1).
- **headline-lg:** Inter 40px at weight 800, line height 1, tracking -0.035em. Section headings (h2).
- **body-md:** Inter 15px at weight 450, line height 1. Body text.
- **body-lg:** Inter 16px at weight 450, line height 1.3. Lead paragraphs.
- **label-lg:** Inter 16px at weight 600. Large buttons and tabs.
- **label-md:** Inter 15px at weight 500. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1.4, tracking 0.25em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 54% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 5px, md 10px, lg 30px, xl 40px.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Breakpoints:** 340px, 500px, 576px, 639px, 640px, 650px, 767px, 768px, 840px, 991px, 992px, 1200px, 1500px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#F5F5F5 → #DCFCE7 → #FCE7F3 → #F3E8FF):

- `rgba(0, 0, 0, 0.07) 0px 0px 0px 2px inset`
- `rgba(0, 0, 0, 0.07) 0px 0px 0px 1px inset`
- `rgba(0, 0, 0, 0.07) 0px 0px 0px 1px`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0.07) 0px 1px 0px 0px`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 176 elements.
- **lg (14px):** 72 elements.
- **md (10px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start the Generator”):** #2563EB fill, #FFFFFF text, 16px/600, 10px radius, padding 0px 21px.
- **button-primary-hover:** background #1D4ED8, text #FFFFFF on hover.
- **button-ghost (“Tools”):** transparent fill, #000000 text, 15px/500, 8px radius, padding 0px 12px.
- **link:** transparent fill, #0A0A0A text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5F5F5, #DCFCE7, #FCE7F3, #F3E8FF.
- Do keep text in 4 levels: #0A0A0A, #000000, #525252, #737373.
- Do reserve #2563EB for primary actions and key highlights.
- Do set headlines in Inter with tight tracking (-0.035em).
- Do reuse the measured spacing steps (5px, 10px, 30px).
- Do use 8px corners on most elements; larger surfaces also use 14px and 10px.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Inter.
- Don't use #2563EB for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.1s.

- **Easing:** `cubic-bezier(0.6, 0.4, 0, 1)`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/coolors.co/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
