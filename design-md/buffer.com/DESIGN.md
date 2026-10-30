---
version: alpha
name: Buffer
description: "Light interface measured from buffer.com: Stolzl type with Figtree, light green accents, flat surfaces and 4px corners."
colors:
  background: "#FEFDFB"
  surface: "#FEFDFB"
  on-surface: "#213130"
  on-background: "#213130"
  on-surface-variant: "#565662"
  on-surface-muted: "#337047"
  on-surface-subtle: "#6E6E68"
  outline: "#B0EC9C"
  outline-variant: "#E0E1E11A"
  primary: "#B0EC9C"
  on-primary: "#213130"
  inverse-surface: "#000000"
  secondary: "#F3BDFF"
typography:
  headline-display:
    fontFamily: Stolzl
    fontSize: 42.5px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Stolzl
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Stolzl
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
  body-md:
    fontFamily: Figtree
    fontSize: 15.5px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.008em
  body-sm:
    fontFamily: Figtree
    fontSize: 13.5px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.009em
  label-lg:
    fontFamily: Figtree
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.007em
  label-md:
    fontFamily: Figtree
    fontSize: 15.5px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0.063em
  label-sm:
    fontFamily: Figtree
    fontSize: 13.5px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: 0.008em
  headline-md-mobile:
    fontFamily: Stolzl
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
rounded:
  sm: 4px
  md: 6px
  lg: 10px
  xl: 20px
  full: 9999px
spacing:
  sm: 5.77px
  md: 9px
  lg: 18px
  xl: 36px
  gutter: 9px
  section: 72px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.headline-md}"
    rounded: "{rounded.full}"
    padding: 0px
    height: 45px
  button-primary-hover:
    backgroundColor: "#90D788"
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    rounded: 2px
    padding: 6px 0px
  input-field:
    backgroundColor: "#FFFFFF"
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-md}"
    rounded: "{rounded.full}"
    padding: 18px 27px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-md}"
    rounded: "{rounded.xl}"
    padding: 0px
  link:
    textColor: "#FFFFFF"
---

# Buffer Design System

## Overview

Buffer describes itself as: “Use Buffer to manage your social media so that you can create and share your content everywhere, consistently. Try our forever free plan or upgrade for more.” The interface is light, built on **Snow (#FEFDFB)** with **Graphite (#213130)** text, and **Light Green (#B0EC9C)** as the main accent.

Type is set in **Stolzl** and **Figtree**. Headlines run large with tight negative tracking; body text is 15.5px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [buffer.com](https://buffer.com/) on October 29, 2026 at 1440×900 and 390×844 from 453 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Snow (#FEFDFB):** Page background, seen 7 times. Token `background`.
- **Graphite (#213130):** Primary text and headings, seen 61 times. Token `on-surface`, CSS `--color-brand-core-dark`.
- **Cool Slate (#565662):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Dark Green (#337047):** Muted text and metadata, seen 4 times. Token `on-surface-muted`, CSS `--color-text-link`.
- **Warm Slate (#6E6E68):** Subtle text and placeholders, seen 4 times. Token `on-surface-subtle`, CSS `--color-text-secondary`.
- **Light Green (#B0EC9C):** Borders and dividers, seen 5 times. Token `outline`, CSS `--color-brand-core-green`.
- **Mist 10% (#E0E1E11A):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Light Green (#B0EC9C):** Brand color on large areas, seen 20 times. Token `primary`, CSS `--color-brand-core-green`.
- **Graphite (#213130):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000000):** High-contrast fills, seen 3 times. Token `inverse-surface`.
- **Pale Purple (#F3BDFF):** Accent on large areas. Token `secondary`.

## Typography

**Stolzl** and **Figtree** share the interface. Fallback stack: `Stolzl, ui-sans-serif, system-ui, sans-serif`. Other loaded fonts: Inter.

- **headline-display:** Stolzl 42.5px at weight 400, line height 1.1, tracking -0.02em. Page title (h1).
- **headline-lg:** Stolzl 24px at weight 400, line height 1.1, tracking -0.02em. Section headings (h2).
- **headline-md:** Stolzl 18px at weight 400, line height 1.1, tracking -0.02em (32px on mobile). Sub-section headings.
- **body-md:** Figtree 15.5px at weight 400, line height 1.4, tracking 0.008em. Body text.
- **body-sm:** Figtree 13.5px at weight 400, line height 1.4, tracking 0.009em. Secondary and small text.
- **label-lg:** Figtree 18px at weight 400, line height 1.4, tracking 0.007em. Large buttons and tabs.
- **label-md:** Figtree 15.5px at weight 500, line height 1.4, tracking 0.063em. Buttons, navigation and labels.
- **label-sm:** Figtree 13.5px at weight 600, line height 1.1, tracking 0.008em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 16% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 5.77px, md 9px, lg 18px, xl 36px.
- **Sections:** 72px vertical padding between major sections.
- **Gaps:** 9px is the most common gap in flex and grid layouts.
- **Breakpoints:** 352px, 425px, 440px, 480px, 576px, 768px, 845px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(23, 23, 23, 0.1) 0px 16px 24px -8px, rgba(23, 23, 23, 0.1) 0px 4px 8px -4px, rgba(23, 23, 23, 0.05) 0px 0px 1px 1px`
- `rgba(23, 23, 23, 0.1) 0px 4px 12px -2px, rgba(23, 23, 23, 0.05) 0px 0px 1px 1px`
- `rgba(0, 0, 0, 0.07) 13.6px 68.16px 64.32px 0px`

Hairline rings and inset highlights also appear: `rgb(85, 85, 83) 0px 0px 0px 1px`.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 232 elements.
- **lg (10px):** 80 elements.
- **full (9999px):** 52 elements.
- **md (6px):** 28 elements.
- **xl (20px):** 22 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started for free”):** #B0EC9C fill, #213130 text, 18px/400, 1440px radius, padding 0px.
- **button-primary-hover:** background #90D788, text #213130 on hover.
- **button-ghost (“Do not sell my personal informat”):** transparent fill, #565662 text, 14px/500, 2px radius, padding 6px 0px.
- **input-field (“Enter your email...”):** #FFFFFF fill, #213130 text, 18px/400, 1440px radius, padding 18px 27px.
- **card:** #FEFDFB fill, #213130 text, 18px/400, 20px radius, padding 0px, shadow `rgba(23, 23, 23, 0.1) 0px 4px 12px -2px, rgba(23, 23, 23, 0.05) 0px 0px 1px 1px`.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FEFDFB for the page.
- Do keep text in 4 levels: #213130, #565662, #337047, #6E6E68.
- Do use #B0EC9C as the brand accent: header, logo and key highlights.
- Do set headlines in Stolzl with tight tracking (-0.02em).
- Do reuse the measured spacing steps (5.77px, 9px, 18px).
- Do use 4px corners on most elements; larger surfaces also use 10px, 6px and 20px.
- Don't introduce new font families beyond Stolzl and Figtree.
- Don't use #B0EC9C for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.5s. Longer ambient animations run 40s.

- **Easing:** `ease-out`, `ease`, `cubic-bezier(0.22, 1, 0.36, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/buffer.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
