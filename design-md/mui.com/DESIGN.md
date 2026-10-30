---
version: alpha
name: MUI
description: "Light interface measured from mui.com: General Sans type with IBM Plex Sans, vivid blue accents, tonal surfaces and 18px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1A1E23"
  on-background: "#1A1E23"
  on-surface-strong: "#000000"
  on-surface-variant: "#303741"
  on-surface-muted: "#576375"
  surface-container-low: "#EBF5FF"
  surface-container: "#DFE2E7"
  overlay: "#E8EBED1A"
  overlay-strong: "#1D212633"
  outline: "#E8EAEE"
  outline-variant: "#DFE2E7"
  primary: "#0073E6"
  on-primary: "#FFFFFF"
  secondary: "#809DBA"
  tertiary: "#0061C2"
  success: "#178C46"
typography:
  headline-display:
    fontFamily: General Sans
    fontSize: 56px
    fontWeight: 600
    lineHeight: 1.11
    letterSpacing: -0.004em
  headline-lg:
    fontFamily: General Sans
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.22
    letterSpacing: -0.006em
  headline-md:
    fontFamily: General Sans
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: 0.007em
  headline-sm:
    fontFamily: IBM Plex Sans
    fontSize: 24px
    fontWeight: 400
  title-lg:
    fontFamily: IBM Plex Sans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.5
  body-md:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: IBM Plex Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: IBM Plex Sans
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-md:
    fontFamily: IBM Plex Sans
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.25
  label-sm:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: General Sans
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.11
    letterSpacing: -0.005em
  headline-lg-mobile:
    fontFamily: General Sans
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.22
    letterSpacing: -0.008em
rounded:
  sm: 1px
  md: 10px
  lg: 12px
  xl: 18px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 16px
  lg: 20px
  gutter: 16px
  container: 1200px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px 10px 10px 12px
    height: 40px
  button-primary-hover:
    backgroundColor: "{colors.tertiary}"
  button-outline:
    backgroundColor: "#F6F7F899"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 1px 6px 1px 8px
    height: 32px
  button-outline-hover:
    backgroundColor: "#E8EAEE80"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "#99CCFF"
    rounded: "{rounded.full}"
    padding: 1px 8px
    height: 25px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 6px 8px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "#9D968E"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# MUI Design System

## Overview

MUI describes itself as: “MUI provides a simple, customizable, and accessible library of React components. Follow your own design system, or start with Material Design.” The interface is light, built on **White (#FFFFFF)** with **Cool Charcoal (#1A1E23)** text, and **Vivid Blue (#0073E6)** as the main accent.

Type is set in **General Sans** and **IBM Plex Sans**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 18px.

Measured from [mui.com](https://mui.com/) on October 29, 2026 at 1440×900 and 390×844 from 363 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #3399FF, #0073E6, #004D99, #E0B400.

- **White (#FFFFFF):** Page background, seen 11 times. Token `background`, CSS `--font-color-onDark`.
- **Cool Charcoal (#1A1E23):** Primary text and headings, seen 53 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 6 times. Token `on-surface-strong`, CSS `--mui-palette-common-onBackground`.
- **Cool Graphite (#303741):** Secondary text, seen 28 times. Token `on-surface-variant`.
- **Blue (#576375):** Muted text and metadata, seen 8 times. Token `on-surface-muted`, CSS `--muidocs-palette-Chip-defaultAvatarColor`.
- **Pale Blue (#EBF5FF):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Cool Mist (#DFE2E7):** Cards and panels, seen 1 time. Token `surface-container`.
- **Mist 10% (#E8EBED1A):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Cool Charcoal 20% (#1D212633):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Cool Mist (#E8EAEE):** Borders and dividers, seen 8 times. Token `outline`, CSS `--muidocs-palette-Switch-defaultDisabledColor`.
- **Cool Mist (#DFE2E7):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Vivid Blue (#0073E6):** Primary buttons and calls to action, seen 31 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#809DBA):** Secondary buttons, seen 1 time. Token `secondary`.
- **Blue (#0061C2):** Accent in logos and imagery, seen 2 times. Token `tertiary`.
- **Dark Green (#178C46):** Success and positive states, seen 6 times. Token `success`.

## Typography

**General Sans** and **IBM Plex Sans** share the interface. Fallback stack: `General Sans, -apple-system, BlinkMacSystemFont, Segoe UI`. Other loaded fonts: Roboto.

- **headline-display:** General Sans 56px at weight 600, line height 1.11, tracking -0.004em (40px on mobile). Page title (h1).
- **headline-lg:** General Sans 36px at weight 600, line height 1.22, tracking -0.006em (24px on mobile). Section headings (h2).
- **headline-md:** General Sans 30px at weight 600, line height 1.5, tracking 0.007em. Sub-section headings.
- **headline-sm:** IBM Plex Sans 24px at weight 400. Card and feature titles.
- **title-lg:** IBM Plex Sans 20px at weight 600, line height 1.5. Small titles.
- **body-md:** IBM Plex Sans 14px at weight 400, line height 1.5. Body text.
- **body-lg:** IBM Plex Sans 16px at weight 400, line height 1.5. Lead paragraphs.
- **label-lg:** IBM Plex Sans 16px at weight 600, line height 1.5. Large buttons and tabs.
- **label-md:** IBM Plex Sans 15px at weight 500, line height 1.25. Buttons, navigation and labels.
- **label-sm:** IBM Plex Sans 14px at weight 600, line height 1.5. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 54% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 16px, lg 20px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1200px.
- **Breakpoints:** 0px, 599.95px, 600px, 768px, 899.95px, 900px, 1200px, 1536px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgb(255, 255, 255) 0px 1px 0px 0px inset, rgba(223, 226, 231, 0.4) 0px -1px 0px 0px inset, rgba(223, 226, 231, 0.5) 0px 1px 2px 0px`
- `rgba(51, 153, 255, 0.5) 0px 1px 0px 0px inset, rgba(0, 77, 153, 0.4) 0px -1px 0px 1px inset, rgba(9, 11, 11, 0.1) 0px 2px 4px 0px`
- `rgb(255, 255, 255) 0px 2px 0px 0px inset, rgba(232, 234, 238, 0.3) 0px -2px 0px 0px inset, rgba(223, 226, 231, 0.5) 0px 1px 2px 0px`

## Shapes

Most elements use 18px corners. Measured radii, most used first:

- **xl (18px):** 124 elements.
- **lg (12px):** 120 elements.
- **sm (1px):** 44 elements.
- **md (10px):** 28 elements.
- **full (9999px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Discover the Core libraries”):** #0073E6 fill, #FFFFFF text, 15px/500, 10px radius, padding 8px 10px 10px 12px, border 1px solid #006BD6, shadow `rgba(51, 153, 255, 0.5) 0px 1px 0px 0px inset, rgba(0, 77, 153, 0.4) 0px -1px 0px 1px inset, rgba(9, 11, 11, 0.1) 0px 2px 4px 0px`.
- **button-primary-hover:** background #0061C2, text #FFFFFF on hover.
- **button-outline (“Search… Ctrl+K”):** #F6F7F899 fill, #576375 text, 14px/400, 12px radius, padding 1px 6px 1px 8px, border 1px solid #DFE2E7, shadow `rgb(255, 255, 255) 0px 1px 0px 0px inset, rgba(232, 234, 238, 0.4) 0px -1px 0px 0px inset, rgba(223, 226, 231, 0.5) 0px 1px 2px 0px`.
- **button-outline-hover:** background #E8EAEE80, text #576375 on hover.
- **button-secondary (“Custom theme”):** #003B7580 fill, #99CCFF text, 12px/500, 1188px radius, padding 1px 8px, border 1px solid #003B75B3, shadow `rgba(0, 59, 117, 0.2) 0px 1px 0px 1px inset, rgb(9, 11, 11) 0px -1px 0px 1px inset, rgb(9, 11, 11) 0px 1px 2px 0px`.
- **button-ghost (“Products”):** transparent fill, #303741 text, 14px/600, 12px radius, padding 6px 8px.
- **input-field (“Temperature”):** #FFFFFF fill, #9D968E text, 13.3333px/400, padding 0px.
- **link:** transparent fill, #303741 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #EBF5FF, #DFE2E7.
- Do keep text in 4 levels: #1A1E23, #000000, #303741, #576375.
- Do reserve #0073E6 for primary actions and key highlights.
- Do set headlines in General Sans with tight tracking (-0.004em).
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do use 18px corners on most elements; larger surfaces also use 12px, 1px and 10px.
- Don't introduce new font families beyond General Sans and IBM Plex Sans.
- Don't use #0073E6 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.3s, 0.25s, 0.1s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-in`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mui.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
