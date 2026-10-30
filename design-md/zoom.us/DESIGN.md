---
version: alpha
name: Zoom
description: "Light interface measured from zoom.com: Newsreader type with Inter, vivid blue accents, tonal surfaces and 12px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#00053D"
  on-background: "#00053D"
  on-surface-strong: "#00031F"
  on-surface-variant: "#181819"
  surface-container-low: "#F3F8FF"
  surface-container: "#E6F0FF"
  surface-container-high: "#E0E0E6"
  overlay: "#FFFFFF1A"
  outline: "#E6F0FF"
  outline-variant: "#D1DEF2"
  primary: "#0B5CFF"
  on-primary: "#FFFFFF"
  secondary: "#1722F6"
typography:
  headline-display:
    fontFamily: Newsreader
    fontSize: 54px
    fontWeight: 500
    lineHeight: 1.12
  headline-lg:
    fontFamily: Newsreader
    fontSize: 46px
    fontWeight: 500
    lineHeight: 1.14
  headline-md:
    fontFamily: Inter
    fontSize: 22px
    fontWeight: 450
    lineHeight: 1
  headline-sm:
    fontFamily: Newsreader
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.02em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.21
  caption:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.35
  label-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.2
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Newsreader
    fontSize: 34px
    fontWeight: 500
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: Newsreader
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.14
rounded:
  xs: 8px
  sm: 10px
  md: 12px
  lg: 16px
  xl: 20px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 20px
  xl: 40px
  gutter: 12px
  section: 60px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 4px 20px
    height: 46px
  button-primary-hover:
    backgroundColor: "#0B5CFF9B"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 4px 20px
    height: 46px
  button-secondary-hover:
    backgroundColor: "#00053D99"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 4px 20px
    height: 46px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 10px 26px 10px 10px
  link:
    textColor: "{colors.on-primary}"
---

# Zoom Design System

## Overview

Zoom describes itself as: “Modernize workflows with Zoom's trusted collaboration tools: including video meetings, Zoom Chat, VoIP phone, webinars, whiteboard, contact center, and events.” The interface is light, built on **White (#FFFFFF)** with **Deep Indigo (#00053D)** text, and **Vivid Blue (#0B5CFF)** as the main accent.

Type is set in **Newsreader** and **Inter**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 12px.

Measured from [zoom.com](https://www.zoom.com/) on October 29, 2026 at 1440×900 and 390×844 from 344 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #0B5CFF, #011067, #00031D, #FB327E.

- **White (#FFFFFF):** Page background, seen 8 times. Token `background`.
- **Deep Indigo (#00053D):** Primary text and headings, seen 35 times. Token `on-surface`.
- **Deep Indigo (#00031F):** Headings and emphasis, seen 4 times. Token `on-surface-strong`.
- **Charcoal (#181819):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Cool Snow (#F3F8FF):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **Pale Blue (#E6F0FF):** Cards and panels, seen 2 times. Token `surface-container`.
- **Cool Mist (#E0E0E6):** Hover and pressed fills, seen 4 times. Token `surface-container-high`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Pale Blue (#E6F0FF):** Borders and dividers, seen 2 times. Token `outline`.
- **Pale Blue (#D1DEF2):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Vivid Blue (#0B5CFF):** Primary buttons and calls to action, seen 43 times. Token `primary`, CSS `--wm-blue`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#1722F6):** Accent, seen 1 time. Token `secondary`.

## Typography

**Newsreader** and **Inter** share the interface. Fallback stack: `Newsreader, Helvetica, Arial, Noto Sans JP`. Other loaded fonts: icozm.

- **headline-display:** Newsreader 54px at weight 500, line height 1.12 (34px on mobile). Page title (h1).
- **headline-lg:** Newsreader 46px at weight 500, line height 1.14 (28px on mobile). Section headings (h2).
- **headline-md:** Inter 22px at weight 450, line height 1. Sub-section headings.
- **headline-sm:** Newsreader 20px at weight 500, line height 1.15, tracking -0.02em. Card and feature titles.
- **body-md:** Inter 16px at weight 400, line height 1. Body text.
- **body-sm:** Inter 14px at weight 400, line height 1.21. Secondary and small text.
- **caption:** Inter 10px at weight 400, line height 1. Captions and fine print.
- **label-lg:** Inter 16px at weight 500, line height 1.35. Large buttons and tabs.
- **label-md:** Inter 15px at weight 500, line height 1.2. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 67% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 16px, lg 20px, xl 40px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 426px, 476px, 530px, 550px, 600px, 767px, 768px, 800px, 896px, 1024px, 1025px, 1100px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.05) 0px 6px 80px 0px, rgba(0, 0, 0, 0.03) 0px 1.34px 17.869px 0px, rgba(0, 0, 0, 0.02) 0px 0.399px 5.32px 0px`

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **md (12px):** 96 elements.
- **xs (8px):** 64 elements.
- **sm (10px):** 16 elements.
- **lg (16px):** 16 elements.
- **xl (20px):** 16 elements.
- **full (9999px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign Up Free”):** #0B5CFF fill, #FFFFFF text, 14px/600, 12px radius, padding 4px 20px, border 1px solid #0B5CFF.
- **button-primary-hover:** background #0B5CFF9B, text #FFFFFF on hover.
- **button-secondary (“Explore products Explore product”):** #00053D fill, #FFFFFF text, 16px/600, 12px radius, padding 4px 20px, border 1px solid #00053D.
- **button-secondary-hover:** background #00053D99, text #FFFFFF on hover.
- **button-outline (“Find your plan Find your plan”):** #F3F8FF fill, #00053D text, 16px/600, 12px radius, padding 4px 20px, border 1px solid #D1DEF2.
- **button-ghost (“Products”):** transparent fill, #FFFFFF text, 14px/500, 12px radius, padding 10px 26px 10px 10px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F3F8FF, #E6F0FF, #E0E0E6.
- Do keep text in 3 levels: #00053D, #00031F, #181819.
- Do reserve #0B5CFF for primary actions and key highlights.
- Do reuse the measured spacing steps (6px, 16px, 20px).
- Do use 12px corners on most elements; larger surfaces also use 8px, 10px and 16px.
- Don't introduce new font families beyond Newsreader and Inter.
- Don't use #0B5CFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.3s, 0.6s, 0.15s, 0.25s. Longer ambient animations run 0.8s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-in`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/zoom.us/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
