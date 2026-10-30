---
version: alpha
name: Datadog
description: "Light interface measured from datadoghq.com: NationalWeb type, violet accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#212529"
  on-background: "#212529"
  on-surface-variant: "#555555"
  on-surface-muted: "#969696"
  surface-container-low: "#F6F6F6"
  outline: "#FFFFFF80"
  primary: "#632CA6"
  on-primary: "#FFFFFF"
  inverse-surface: "#000000"
  secondary: "#9EC5FE"
typography:
  headline-display:
    fontFamily: NationalWeb
    fontSize: 68px
    fontWeight: 600
    lineHeight: 1
  headline-lg:
    fontFamily: NationalWeb
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.11
  body-md:
    fontFamily: NationalWeb
    fontSize: 14px
    fontWeight: 300
    lineHeight: 1.29
  body-lg:
    fontFamily: NationalWeb
    fontSize: 22px
    fontWeight: 300
    lineHeight: 1.43
  label-md:
    fontFamily: NationalWeb
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.25
  headline-display-mobile:
    fontFamily: NationalWeb
    fontSize: 38px
    fontWeight: 600
    lineHeight: 1.11
  headline-lg-mobile:
    fontFamily: NationalWeb
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.14
rounded:
  md: 4px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 48px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: 16px 24px
    height: 54px
  button-primary-hover:
    backgroundColor: "#7700FF"
  button-outline:
    textColor: "{colors.primary}"
    rounded: "{rounded.md}"
    padding: 14px 24px 16px 24px
    height: 54px
  button-outline-hover:
    backgroundColor: "#7700FF"
    textColor: "{colors.on-primary}"
  button-ghost:
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: 11px 24px 12px 24px
    height: 51px
  link:
    textColor: "#E2E2E2"
---

# Datadog Design System

## Overview

Datadog describes itself as: “See inside any stack, any app, at any scale, anywhere.” The interface is light, built on **White (#FFFFFF)** with **Cool Graphite (#212529)** text, and **Violet (#632CA6)** as the main accent.

Type is set in **NationalWeb**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [datadoghq.com](https://www.datadoghq.com/) on October 29, 2026 at 1440×900 and 390×844 from 360 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles, plus gradient stops #B37BFF, #4BB3FF, #3023AE, #C024B6.

- **White (#FFFFFF):** Page background, seen 5 times. Token `background`, CSS `--bs-white`.
- **Cool Graphite (#212529):** Primary text and headings, seen 11 times. Token `on-surface`, CSS `--bs-highlight-color`.
- **Slate (#555555):** Secondary text, seen 9 times. Token `on-surface-variant`.
- **Gray (#969696):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Snow (#F6F6F6):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **White 50% (#FFFFFF80):** Borders and dividers, seen 1 time. Token `outline`.
- **Violet (#632CA6):** Primary buttons and calls to action, seen 6 times. Token `primary`, CSS `--bs-purple`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000000):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Light Blue (#9EC5FE):** Accent (CSS variable). Token `secondary`.

## Typography

**NationalWeb** carries the whole interface. Fallback stack: `NationalWeb, Helvetica, Arial, sans-serif`. Other loaded fonts: nationalweb, robotomono-regular, iconfont.

- **headline-display:** NationalWeb 68px at weight 600, line height 1 (38px on mobile). Page title (h1).
- **headline-lg:** NationalWeb 36px at weight 600, line height 1.11 (28px on mobile). Section headings (h2).
- **body-md:** NationalWeb 14px at weight 300, line height 1.29. Body text.
- **body-lg:** NationalWeb 22px at weight 300, line height 1.43. Lead paragraphs.
- **label-md:** NationalWeb 16px at weight 700, line height 1.25. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (72% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 425px, 480px, 575.98px, 576px, 767px, 767.98px, 768px, 991px, 991.98px, 992px, 1199.98px, 1200px, 1399.98px, 1400px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.07) 0px 0px 8px 8px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 20 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“FREE TRIAL”):** #632CA6 fill, #FFFFFF text, 18px/700, 4px radius, padding 16px 24px.
- **button-primary-hover:** background #7700FF, text #FFFFFF on hover.
- **button-outline (“SEE THE PLATFORM”):** transparent fill, #632CA6 text, 18px/700, 4px radius, padding 14px 24px 16px 24px, border 1px solid #632CA6.
- **button-outline-hover:** background #7700FF, text #FFFFFF on hover.
- **button-ghost (“GET THE EBOOK”):** transparent fill, #FFFFFF text, 18px/600, 4px radius, padding 11px 24px 12px 24px, border 1px solid #FFFFFF.
- **link:** transparent fill, #E2E2E2 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F6F6F6.
- Do keep text in 3 levels: #212529, #555555, #969696.
- Do reserve #632CA6 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 4px corners on most elements.
- Don't use #969696 for body text; it reaches 2.96:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond NationalWeb.
- Don't use #632CA6 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s.

- **Easing:** `ease-in-out`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/datadoghq.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
