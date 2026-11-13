---
version: alpha
name: Plain
description: "Light interface measured from plain.com: ABC Favorit Medium type with ABC Favorit Regular, dark teal accents, flat surfaces and 100px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#252D2A"
  on-background: "#252D2A"
  on-surface-strong: "#0A2414"
  on-surface-variant: "#1F1F28"
  on-surface-muted: "#636370"
  outline: "#E7E7EF"
  primary: "#1B6646"
  on-primary: "#FFFFFF"
  secondary: "#00AB5F"
  tertiary: "#1AD379"
  success: "#9AF6BB"
typography:
  headline-display:
    fontFamily: ABC Favorit Medium
    fontSize: 48px
    fontWeight: 500
    lineHeight: 0.96
    letterSpacing: -0.021em
  headline-lg:
    fontFamily: ABC Favorit Medium
    fontSize: 38px
    fontWeight: 500
    lineHeight: 1.16
    letterSpacing: -0.02em
  headline-md:
    fontFamily: ABC Favorit Medium
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.13
    letterSpacing: -0.028em
  headline-sm:
    fontFamily: ABC Favorit Medium
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.017em
  body-md:
    fontFamily: ABC Favorit Regular
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: -0.01em
  body-lg:
    fontFamily: ABC Favorit Regular
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.75
  body-sm:
    fontFamily: sans-serif
    fontSize: 12px
    fontWeight: 400
  code:
    fontFamily: Geist Mono
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.54
    letterSpacing: 0.015em
  headline-display-mobile:
    fontFamily: ABC Favorit Medium
    fontSize: 38px
    fontWeight: 500
    lineHeight: 1.11
    letterSpacing: -0.021em
  headline-lg-mobile:
    fontFamily: ABC Favorit Medium
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.017em
  headline-md-mobile:
    fontFamily: ABC Favorit Medium
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.021em
rounded:
  sm: 3.83px
  md: 6px
  lg: 16px
  xl: 100px
spacing:
  xs: 3px
  sm: 8px
  md: 16px
  lg: 24px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.xl}"
    padding: 8px 16px
    height: 36px
  button-primary-hover:
    backgroundColor: "#2C9266"
  button-ghost:
    textColor: "#000000"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.success}"
---

# Plain Design System

## Overview

Plain describes itself as: “Plain is the AI support stack built for B2B teams. Composable infrastructure that gives you complete flexibility to build a support motion that grows with your business — no-code or all-code.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#252D2A)** text, and **Dark Teal (#1B6646)** as the main accent.

Type is set in **ABC Favorit Medium** and **ABC Favorit Regular**, with **Geist Mono** for code. Headlines run large with tight negative tracking; body text is 15px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 100px.

Measured from [plain.com](https://www.plain.com/) on November 13, 2026 at 1440×900 and 390×844 from 308 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 6 times. Token `background`.
- **Graphite (#252D2A):** Primary text and headings, seen 35 times. Token `on-surface`.
- **Deep Green (#0A2414):** Headings and emphasis, seen 6 times. Token `on-surface-strong`.
- **Cool Charcoal (#1F1F28):** Secondary text, seen 33 times. Token `on-surface-variant`.
- **Cool Slate (#636370):** Muted text and metadata, seen 5 times. Token `on-surface-muted`.
- **Cool Mist (#E7E7EF):** Borders and dividers, seen 1 time. Token `outline`.
- **Dark Teal (#1B6646):** Primary buttons and calls to action, seen 6 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Teal (#00AB5F):** Accent, seen 5 times. Token `secondary`.
- **Teal (#1AD379):** Accent, seen 4 times. Token `tertiary`.
- **Light Green (#9AF6BB):** Success and positive states, seen 38 times. Token `success`.

## Typography

**ABC Favorit Medium**, **ABC Favorit Regular**, **sans-serif** and **Geist Mono** (monospace) share the interface. Fallback stack: `ABC Favorit Medium, ABC Favorit Medium Placeholder, sans-serif`. Other loaded fonts: Inter.

- **headline-display:** ABC Favorit Medium 48px at weight 500, line height 0.96, tracking -0.021em (38px on mobile). Page title (h1).
- **headline-lg:** ABC Favorit Medium 38px at weight 500, line height 1.16, tracking -0.02em (30px on mobile). Section headings (h2).
- **headline-md:** ABC Favorit Medium 32px at weight 500, line height 1.13, tracking -0.028em (24px on mobile). Sub-section headings.
- **headline-sm:** ABC Favorit Medium 24px at weight 500, line height 1.25, tracking -0.017em. Card and feature titles.
- **body-md:** ABC Favorit Regular 15px at weight 400, line height 1.33, tracking -0.01em. Body text.
- **body-lg:** ABC Favorit Regular 16px at weight 400, line height 1.75. Lead paragraphs.
- **body-sm:** sans-serif 12px at weight 400. Secondary and small text.
- **code:** Geist Mono 13px at weight 500, line height 1.54, tracking 0.015em, uppercase. Code and technical values.

## Layout

Spacing does not follow a strict grid: 69% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 8px, md 16px, lg 24px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 576px, 959px, 960px, 998px, 999px, 999.98px, 1000px, 1035.98px, 1036px, 1069px, 1070px, 1199.98px, 1271px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgb(232, 230, 225) 0px 0px 0px 1.62069px`
- `rgba(0, 0, 0, 0.08) 0px 0px 0px 1px inset`

## Shapes

Most elements use 100px corners. Measured radii, most used first:

- **xl (100px):** 84 elements.
- **md (6px):** 20 elements.
- **lg (16px):** 12 elements.
- **sm (3.83px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“BOOK A DEMO”):** #1B6646 fill, #FFFFFF text, 12px/400, 100px radius, padding 8px 16px.
- **button-primary-hover:** background #2C9266, text #FFFFFF on hover.
- **button-ghost (“Investigate before you open the ”):** transparent fill, #000000 text, 12px/400, padding 0px.
- **card:** #FFFFFF fill, #252D2A text, 12px/400, 16px radius, padding 0px, shadow `rgb(232, 230, 225) 0px 0px 0px 1.62069px`.
- **link:** transparent fill, #9AF6BB text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 4 levels: #252D2A, #0A2414, #1F1F28, #636370.
- Do reserve #1B6646 for primary actions and key highlights.
- Do set headlines in ABC Favorit Medium with tight tracking (-0.021em).
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 100px corners on most elements; larger surfaces also use 6px, 16px and 3.83px.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond ABC Favorit Medium, ABC Favorit Regular, sans-serif and Geist Mono.
- Don't use #1B6646 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.4s, 0.3s, 0.1s.

- **Easing:** `cubic-bezier(0.2, 0, 0, 1)`, `cubic-bezier(0.22, 1, 0.36, 1)`, `cubic-bezier(0.4, 0, 1, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/plain.com/), the free DESIGN.md generator (engine 2026.10.29+f0c146f7cdfd).
