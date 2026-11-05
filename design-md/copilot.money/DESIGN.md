---
version: alpha
name: Copilot Money
description: "Light interface measured from copilot.money: Matter type, vivid blue accents, tonal surfaces and 16px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#5A7086"
  on-background: "#5A7086"
  on-surface-variant: "#8B95AC"
  surface-container-low: "#FFFFFFE6"
  surface-container: "#F1F7FE"
  overlay: "#143352B3"
  overlay-strong: "#14335214"
  outline: "#FFFFFFE6"
  outline-variant: "#FFFFFF59"
  primary: "#437CEF"
  on-primary: "#FFFFFF"
  secondary: "#143352"
  tertiary: "#5B7086"
  error: "#FF4334"
  success: "#008A33"
typography:
  headline-display:
    fontFamily: Matter
    fontSize: 64px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.008em
  headline-lg:
    fontFamily: Matter
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Matter
    fontSize: 33.5px
    fontWeight: 600
    lineHeight: 1.29
  headline-sm:
    fontFamily: Matter
    fontSize: 24px
    fontWeight: 550
    lineHeight: 1.25
    letterSpacing: -0.012em
  body-md:
    fontFamily: Matter
    fontSize: 16px
    fontWeight: 430
  body-lg:
    fontFamily: Matter
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.5
  body-sm:
    fontFamily: Matter
    fontSize: 13px
    fontWeight: 430
    lineHeight: 1.38
  label-lg:
    fontFamily: Matter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.38
  label-md:
    fontFamily: Matter
    fontSize: 14px
    fontWeight: 550
    lineHeight: 1.43
    letterSpacing: 0.007em
  label-sm:
    fontFamily: Matter
    fontSize: 13px
    fontWeight: 550
    lineHeight: 1.23
    letterSpacing: 0.08em
  code:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: 430
    lineHeight: 1.36
    letterSpacing: 0.045em
  headline-display-mobile:
    fontFamily: Matter
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.013em
  headline-lg-mobile:
    fontFamily: Matter
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.13
    letterSpacing: -0.013em
rounded:
  xs: 8px
  sm: 16px
  md: 24px
  lg: 32px
  xl: 40px
  full: 9999px
spacing:
  xs: 3px
  sm: 8px
  md: 14px
  lg: 24px
  xl: 64px
  gutter: 18px
  section: 80px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.xl}"
    padding: 8px 20px
    height: 44px
  button-secondary:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px 11.5px 0px 3.5px
    height: 32px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.overlay}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.xl}"
    padding: 8px 20px
    height: 44px
  button-ghost:
    textColor: "{colors.secondary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.full}"
    padding: 8px 14px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.secondary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 12.5px 22.5px 12.5px 16.5px
  link:
    textColor: "{colors.overlay}"
---

# Copilot Money Design System

## Overview

Copilot Money describes itself as: “Track spending, budgets, investments & net worth all in one beautifully designed place. The personal finance app powered by smart automation and built with privacy at the center. Available on Web, iPhone, Mac & iPad. Sta” The interface is light, built on **White (#FFFFFF)** with **Blue (#5A7086)** text, and **Vivid Blue (#437CEF)** as the main accent.

Type is set in **Matter**, with **JetBrains Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 16px.

Measured from [copilot.money](https://www.copilot.money/) on November 4, 2026 at 1440×900 and 390×844 from 406 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles, plus gradient stops #62C4FC, #3C80F7, #E1F4FF.

- **White (#FFFFFF):** Page background, seen 11 times. Token `background`, CSS `--inverted-primary`.
- **Blue (#5A7086):** Primary text and headings. Token `on-surface`.
- **Blue (#8B95AC):** Secondary text, seen 10 times. Token `on-surface-variant`.
- **White 90% (#FFFFFFE6):** Raised areas one step from the page, seen 8 times. Token `surface-container-low`.
- **Cool Snow (#F1F7FE):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--top-color`.
- **Deep Blue 70% (#143352B3):** Translucent fill for cards and controls, seen 30 times. Token `overlay`.
- **Deep Blue 8% (#14335214):** Stronger translucent fill, seen 30 times. Token `overlay-strong`.
- **White 90% (#FFFFFFE6):** Borders and dividers, seen 4 times. Token `outline`.
- **White 35% (#FFFFFF59):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Vivid Blue (#437CEF):** Primary buttons and calls to action, seen 8 times. Token `primary`, CSS `--blue-primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Blue (#143352):** Accent (CSS variable), seen 61 times. Token `secondary`, CSS `--primary`.
- **Blue (#5B7086):** Links and interactive text, seen 62 times. Token `tertiary`.
- **Vivid Red (#FF4334):** Errors and destructive states, seen 2 times. Token `error`.
- **Dark Green (#008A33):** Success and positive states, seen 1 time. Token `success`.

## Typography

**Matter** and **JetBrains Mono** (monospace) share the interface. Fallback stack: `Matter, ui-sans-serif, system-ui, sans-serif`. Other loaded fonts: Geist Mono.

- **headline-display:** Matter 64px at weight 600, line height 1.25, tracking -0.008em (40px on mobile). Page title (h1).
- **headline-lg:** Matter 48px at weight 600, line height 1.15, tracking -0.01em (30px on mobile). Section headings (h2).
- **headline-md:** Matter 33.5px at weight 600, line height 1.29. Sub-section headings.
- **headline-sm:** Matter 24px at weight 550, line height 1.25, tracking -0.012em. Card and feature titles.
- **body-md:** Matter 16px at weight 430. Body text.
- **body-lg:** Matter 20px at weight 500, line height 1.5. Lead paragraphs.
- **body-sm:** Matter 13px at weight 430, line height 1.38. Secondary and small text.
- **label-lg:** Matter 16px at weight 500, line height 1.38. Large buttons and tabs.
- **label-md:** Matter 14px at weight 550, line height 1.43, tracking 0.007em. Buttons, navigation and labels.
- **label-sm:** Matter 13px at weight 550, line height 1.23, tracking 0.08em. Small labels and badges.
- **code:** JetBrains Mono 11px at weight 430, line height 1.36, tracking 0.045em, uppercase. Code and technical values.

## Layout

Spacing does not follow a strict grid: 52% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 8px, md 14px, lg 24px, xl 64px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 18px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(67, 124, 239, 0.12) 0px 0px 0px 0.5px, rgba(67, 124, 239, 0.07) 0px 1px 3px 0px, rgba(67, 124, 239, 0.04) 0px 4px 12px 0px, rgba(67, 124, 239, 0.05) 0px 24px 80px 0px, rgba(255, 255, 255, 0.03) 1.5px 1.5px 8px 0px inset, rgba(0, 0, 0, 0.02) -1.5px -1.5px 6px 0px inset`
- `rgba(67, 124, 239, 0.06) 0px 1px 2px 0px, rgba(67, 124, 239, 0.09) 0px 4px 12px 0px`
- `rgba(65, 171, 255, 0.08) 0px 1px 4px 0px, rgba(65, 171, 255, 0.08) 0px 2px 8px 0px, rgba(65, 171, 255, 0.08) 0px 4px 24px 0px, rgba(65, 171, 255, 0.08) 0px 4px 40px 0px, rgba(255, 255, 255, 0.04) 1.5px 1.5px 2px 0px inset, rgba(0, 0, 0, 0.02) -1.5px -1.5px 2px 0px inset`

Hairline rings and inset highlights also appear: `rgba(10, 14, 20, 0.1) 0px 0px 0px 0.6px inset`.

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **sm (16px):** 124 elements.
- **full (9999px):** 88 elements.
- **md (24px):** 80 elements.
- **lg (32px):** 68 elements.
- **xl (40px):** 44 elements.
- **xs (8px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #437CEF fill, #FFFFFF text, 16px/500, 40px radius, padding 8px 20px, border 1px solid #FFFFFF59, shadow `rgba(65, 171, 255, 0.04) 0px 4px 4px 0px, rgba(65, 171, 255, 0.06) 0px 4px 12px 0px, rgba(65, 171, 255, 0.08) 0px 4px 16px 0px`.
- **button-secondary (“New Meet your money assistant”):** transparent fill, #FFFFFF text, 14px/500, 999px radius, padding 0px 11.5px 0px 3.5px, border 1px solid #FFFFFFE6, shadow `rgba(67, 124, 239, 0.06) 0px 1px 2px 0px, rgba(67, 124, 239, 0.09) 0px 4px 12px 0px`.
- **button-outline (“Log in”):** #FFFFFF fill, #143352B3 text, 16px/500, 40px radius, padding 8px 20px, border 1px solid #0A0E141A, shadow `rgba(10, 14, 20, 0.03) 0px 1px 4px 0px, rgba(10, 14, 20, 0.08) 0px 1px 1px -1px`.
- **button-ghost (“Product”):** transparent fill, #143352 text, 16px/500, 999px radius, padding 8px 14px, shadow `rgba(67, 124, 239, 0) 0px 0px 0px 0.5px inset`.
- **card:** #FFFFFFCC fill, #143352 text, 16px/430, 32px radius, padding 12.5px 22.5px 12.5px 16.5px, border 1px solid #FFFFFFB3, shadow `rgba(65, 171, 255, 0.08) 0px 1px 4px 0px, rgba(65, 171, 255, 0.08) 0px 2px 8px 0px, rgba(65, 171, 255, 0.08) 0px 4px 24px 0px, rgba(65, 171, 255, 0.08) 0px 4px 40px 0px, rgba(255, 255, 255, 0.04) 1.5px 1.5px 2px 0px inset, rgba(0, 0, 0, 0.02) -1.5px -1.5px 2px 0px inset`.
- **link:** transparent fill, #143352B3 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FFFFFFE6, #F1F7FE.
- Do keep text in 2 levels: #5A7086, #8B95AC.
- Do reserve #437CEF for primary actions and key highlights.
- Do set headlines in Matter with tight tracking (-0.008em).
- Do reuse the measured spacing steps (8px, 14px, 24px).
- Do use 16px corners on most elements; larger surfaces also use 24px, 32px and 40px.
- Don't use #8B95AC for body text; it reaches 3.00:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Matter and JetBrains Mono.
- Don't use #437CEF for large backgrounds or body text.
- Don't make interface transitions slower than 0.42s.

## Motion

Interface transitions are quick: 0.16s, 0.24s, 0.3s, 0.2s.

- **Easing:** `cubic-bezier(0.25, 1, 0.5, 1)`, `ease-out`, `cubic-bezier(0.16, 1, 0.3, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/copilot.money/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
