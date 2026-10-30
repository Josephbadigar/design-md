---
version: alpha
name: Node.js
description: "Light interface measured from nodejs.org: OPEN SANS type, dark green accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1F2328"
  on-background: "#1F2328"
  on-surface-variant: "#2C3437"
  on-surface-muted: "#556066"
  on-surface-subtle: "#6E7B83"
  surface-container-low: "#F6F7F9"
  surface-container: "#E9F4FA"
  surface-container-high: "#D9E1E4"
  outline: "#E9EDF0"
  outline-variant: "#D9E1E4"
  primary: "#417E38"
  on-primary: "#FFFFFF"
  secondary: "#0A3069"
  tertiary: "#84BA64"
typography:
  headline-display:
    fontFamily: OPEN SANS
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.02em
  body-md:
    fontFamily: OPEN SANS
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: OPEN SANS
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: OPEN SANS
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: OPEN SANS
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  code:
    fontFamily: SFMono-Regular
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.38
  headline-display-mobile:
    fontFamily: OPEN SANS
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.02em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 18px
  gutter: 8px
  margin: 32px
  container: 768px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 10px 18px
    height: 46px
  button-primary-hover:
    backgroundColor: "#2C682C"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    padding: 4px 10px 4px 4px
    height: 30px
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    rounded: "{rounded.sm}"
    padding: 4px 10px
    height: 24px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Node.js Design System

## Overview

Node.js describes itself as: “Node.js® is a free, open-source, cross-platform JavaScript runtime environment that lets developers create servers, web apps, command line tools and scripts.” The interface is light, built on **White (#FFFFFF)** with **Cool Charcoal (#1F2328)** text, and **Dark Green (#417E38)** as the main accent.

Type is set in **OPEN SANS**, with **SFMono-Regular** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [nodejs.org/en](https://nodejs.org/en) (the site sent our reader to its /en version; nodejs.org was asked for) on October 29, 2026 at 1440×900 and 390×844 from 275 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Cool Charcoal (#1F2328):** Primary text and headings, seen 36 times. Token `on-surface`.
- **Cool Graphite (#2C3437):** Secondary text, seen 10 times. Token `on-surface-variant`.
- **Cool Slate (#556066):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Cool Slate (#6E7B83):** Subtle text and placeholders, seen 11 times. Token `on-surface-subtle`.
- **Snow (#F6F7F9):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--color-neutral-100`.
- **Cool Mist (#E9F4FA):** Cards and panels, seen 1 time. Token `surface-container`.
- **Cool Silver (#D9E1E4):** Hover and pressed fills, seen 1 time. Token `surface-container-high`, CSS `--color-neutral-300`.
- **Cool Mist (#E9EDF0):** Borders and dividers, seen 11 times. Token `outline`, CSS `--color-neutral-200`.
- **Cool Silver (#D9E1E4):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--color-neutral-300`.
- **Dark Green (#417E38):** Primary buttons and calls to action, seen 11 times. Token `primary`, CSS `--color-brand-600`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#0A3069):** Accent in text, fills and borders, seen 16 times. Token `secondary`.
- **Green (#84BA64):** Accent (CSS variable). Token `tertiary`.

## Typography

**OPEN SANS** and **SFMono-Regular** (monospace) share the interface. Fallback stack: `OPEN_SANS, OPEN_SANS Fallback`. Other loaded fonts: OPEN_SANS.

- **headline-display:** OPEN SANS 48px at weight 600, line height 1.33, tracking -0.02em (36px on mobile). Page title (h1).
- **body-md:** OPEN SANS 16px at weight 400, line height 1.5. Body text.
- **body-sm:** OPEN SANS 14px at weight 400, line height 1.43. Secondary and small text.
- **label-md:** OPEN SANS 16px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** OPEN SANS 14px at weight 600, line height 1.43. Small labels and badges.
- **code:** SFMono-Regular 14px at weight 400, line height 1.38. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (81% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 18px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 768px.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 896px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#F6F7F9 → #E9F4FA → #D9E1E4):

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(233, 237, 240) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.20991 -0.003893 -0.0339065 / 0.05) 0px 1px 2px 0px`.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 100 elements.
- **lg (8px):** 36 elements.
- **md (6px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Node.js®”):** #417E38 fill, #FFFFFF text, 16px/600, 4px radius, padding 10px 18px, border 1px solid #417E38, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.20991 -0.003893 -0.0339065 / 0.05) 0px 1px 2px 0px`.
- **button-primary-hover:** background #2C682C, text #FFFFFF on hover.
- **button-outline (“v26.13.0 Latest LTS”):** #E9F4FA fill, #FFFFFF text, 14px/500, 3.35544e+07px radius, padding 4px 10px 4px 4px, border 1px solid #BCE6FC.
- **button-ghost (“Copy to clipboard”):** #F6F7F9 fill, #2C3437 text, 12px/500, 4px radius, padding 4px 10px.
- **link:** transparent fill, #556066 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F6F7F9, #E9F4FA, #D9E1E4.
- Do keep text in 4 levels: #1F2328, #2C3437, #556066, #6E7B83.
- Do reserve #417E38 for primary actions and key highlights.
- Do set headlines in OPEN SANS with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 18px).
- Do use 4px corners on most elements; larger surfaces also use 8px and 6px.
- Don't use #6E7B83 for body text; it reaches 4.35:1 on #FFFFFF. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond OPEN SANS and SFMono-Regular.
- Don't use #417E38 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/nodejs.org/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
