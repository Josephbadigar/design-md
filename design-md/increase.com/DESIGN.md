---
version: alpha
name: Increase
description: "Light interface measured from increase.com: TT Interphases Pro type, vivid teal accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1D2A36"
  on-background: "#1D2A36"
  on-surface-strong: "#132030"
  on-surface-variant: "#687887"
  on-surface-muted: "#A6B0BA"
  surface-container-low: "#FFFFFFF2"
  surface-container: "#FCFCFC"
  surface-container-high: "#EDF1F5"
  outline: "#D5DEE5"
  outline-variant: "#F5F6F7"
  primary: "#31F2BF"
  on-primary: "#1D2A36"
  secondary: "#34BCFF"
  tertiary: "#E4FF33"
typography:
  headline-display:
    fontFamily: TT Interphases Pro
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: TT Interphases Pro
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.004em
  headline-md:
    fontFamily: TT Interphases Pro
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.01em
  body-md:
    fontFamily: TT Interphases Pro
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: TT Interphases Pro
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: TT Interphases Pro
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  code:
    fontFamily: Input Mono
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: TT Interphases Pro
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.004em
  headline-lg-mobile:
    fontFamily: TT Interphases Pro
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.01em
rounded:
  md: 8px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 10px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 46px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 46px
  button-secondary:
    backgroundColor: "#1A2B3B"
    textColor: "{colors.background}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 5px 10px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 4px 8px
  link:
    textColor: "#334352"
---

# Increase Design System

## Overview

Increase describes itself as: “Banking for ambitious technology companies. Build great financial products with an API-first bank.” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#1D2A36)** text, and **Vivid Teal (#31F2BF)** as the main accent.

Type is set in **TT Interphases Pro**, with **Input Mono** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [increase.com](https://increase.com/) on November 4, 2026 at 1440×900 and 390×844 from 355 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **White (#FFFFFF):** Page background, seen 10 times. Token `background`, CSS `--shiki-token-builtin`.
- **Deep Blue (#1D2A36):** Primary text and headings, seen 29 times. Token `on-surface`.
- **Deep Blue (#132030):** Headings and emphasis, seen 14 times. Token `on-surface-strong`.
- **Blue (#687887):** Secondary text, seen 9 times. Token `on-surface-variant`.
- **Blue (#A6B0BA):** Muted text and metadata, seen 24 times. Token `on-surface-muted`.
- **White 95% (#FFFFFFF2):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#FCFCFC):** Cards and panels, seen 2 times. Token `surface-container`.
- **Cool Mist (#EDF1F5):** Hover and pressed fills, seen 7 times. Token `surface-container-high`.
- **Cool Silver (#D5DEE5):** Borders and dividers, seen 10 times. Token `outline`.
- **Snow (#F5F6F7):** Secondary dividers, seen 8 times. Token `outline-variant`.
- **Vivid Teal (#31F2BF):** Primary buttons and calls to action, seen 26 times. Token `primary`, CSS `--shiki-token-string-expression`.
- **Deep Blue (#1D2A36):** Text and icons on primary. Token `on-primary`.
- **Vivid Cyan (#34BCFF):** Accent in logos and imagery, seen 2 times. Token `secondary`.
- **Vivid Yellow (#E4FF33):** Secondary buttons, seen 3 times. Token `tertiary`.

## Typography

**TT Interphases Pro** and **Input Mono** (monospace) share the interface. Fallback stack: `TT Interphases Pro-c98a05336328a01f, TT Interphases Pro-c98a05336328a01f fallback: Arial, Arial, sans-serif`. Other loaded fonts: TT Interphases Pro-c98a05336328a01f, Input Mono-4c4a0ba0f7fa02b9.

- **headline-display:** TT Interphases Pro 32px at weight 600, line height 1.2, tracking -0.01em (24px on mobile). Page title (h1).
- **headline-lg:** TT Interphases Pro 24px at weight 500, line height 1.2, tracking -0.004em (20px on mobile). Section headings (h2).
- **headline-md:** TT Interphases Pro 20px at weight 400, line height 1.4, tracking -0.01em. Sub-section headings.
- **body-md:** TT Interphases Pro 14px at weight 400, line height 1.43. Body text.
- **label-md:** TT Interphases Pro 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** TT Interphases Pro 14px at weight 500, line height 1.43. Small labels and badges.
- **code:** Input Mono 16px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing does not follow a strict grid: 62% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Gaps:** 10px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(21, 30, 41, 0.05) 0px 1px 2px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 104 elements.
- **full (9999px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Contact sales”):** #31F2BF fill, #1D2A36 text, 16px/500, 8px radius, padding 12px 16px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(21, 30, 41, 0.05) 0px 1px 2px 0px`.
- **button-outline (“Sign up”):** #FFFFFF fill, #1D2A36 text, 16px/500, 8px radius, padding 12px 16px, border 1px solid #D5DEE5, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(21, 30, 41, 0.05) 0px 1px 2px 0px`.
- **button-secondary (“Sign up”):** #1A2B3B fill, #FFFFFF text, 14px/500, 8px radius, padding 5px 10px.
- **button-ghost (“Products”):** transparent fill, #687887 text, 14px/500, 8px radius, padding 4px 8px.
- **link:** transparent fill, #334352 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FFFFFFF2, #FCFCFC, #EDF1F5.
- Do keep text in 4 levels: #1D2A36, #132030, #687887, #A6B0BA.
- Do reserve #31F2BF for primary actions and key highlights.
- Do set headlines in TT Interphases Pro with tight tracking (-0.01em).
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 8px corners on most elements.
- Don't use #A6B0BA for body text; it reaches 2.20:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond TT Interphases Pro and Input Mono.
- Don't use #31F2BF for large backgrounds or body text.
- Don't make interface transitions slower than 0.34s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.34s, 0.2s. Longer ambient animations run 1.6s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.23, 1, 0.32, 1)`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/increase.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
