---
version: alpha
name: Ant Design
description: "Light interface measured from ant.design: AlibabaSans type with system-ui, vivid blue accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1F1F1F"
  on-background: "#1F1F1F"
  on-surface-variant: "#595959"
  surface-container-low: "#F0F3FA"
  surface-container: "#E8F4FD"
  surface-container-high: "#FCE9E9"
  overlay: "#0000000A"
  overlay-strong: "#FFFFFF4D"
  outline: "#D9D9D9"
  outline-variant: "#F0F0F0"
  primary: "#1677FF"
  on-primary: "#FFFFFF"
  secondary: "#91CAFF"
  tertiary: "#FADB14"
  error: "#FF4D4F"
  warning: "#FAAD14"
typography:
  headline-display:
    fontFamily: AlibabaSans
    fontSize: 38px
    fontWeight: 900
    lineHeight: 1.21
  body-md:
    fontFamily: AlibabaSans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.57
  body-lg:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: AlibabaSans
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.57
  headline-display-mobile:
    fontFamily: AlibabaSans
    fontSize: 30px
    fontWeight: 900
    lineHeight: 1.21
rounded:
  sm: 4px
  md: 6px
  lg: 8px
  xl: 100px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 80px
  margin: 32px
  container: 1208px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.lg}"
    padding: 0px 15px
    height: 40px
  button-primary-hover:
    backgroundColor: "#4096FF"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.lg}"
    padding: 0px 15px
    height: 40px
  button-outline-hover:
    textColor: "#4096FF"
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.error}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 15px
    height: 32px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 20px
    padding: 0px 12px 0px 32px
  card:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 16px
    padding: 32px
  link:
    textColor: "{colors.on-surface}"
---

# Ant Design Design System

## Overview

Ant Design describes itself as: “An enterprise-class UI design language and React UI library with a set of high-quality React components, one of best React UI library for enterprises” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1F1F1F)** text, and **Vivid Blue (#1677FF)** as the main accent.

Type is set in **AlibabaSans** and **system-ui**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [ant.design](https://ant.design/) on November 4, 2026 at 1440×900 and 390×844 from 393 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles.

- **White (#FFFFFF):** Page background, seen 39 times. Token `background`.
- **Charcoal (#1F1F1F):** Primary text and headings. Token `on-surface`.
- **Slate (#595959):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Cool Snow (#F0F3FA):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Pale Blue (#E8F4FD):** Cards and panels, seen 1 time. Token `surface-container`.
- **Pale Red (#FCE9E9):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Near Black 4% (#0000000A):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **White 30% (#FFFFFF4D):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Silver (#D9D9D9):** Borders and dividers, seen 19 times. Token `outline`.
- **Mist (#F0F0F0):** Secondary dividers, seen 13 times. Token `outline-variant`.
- **Vivid Blue (#1677FF):** Primary buttons and calls to action, seen 16 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Blue (#91CAFF):** Accent, seen 3 times. Token `secondary`.
- **Vivid Amber (#FADB14):** Accent, seen 3 times. Token `tertiary`.
- **Red (#FF4D4F):** Errors and destructive states, seen 3 times. Token `error`.
- **Vivid Orange (#FAAD14):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**AlibabaSans** and **system-ui** share the interface. Fallback stack: `AlibabaSans, -apple-system, BlinkMacSystemFont, Segoe UI`.

- **headline-display:** AlibabaSans 38px at weight 900, line height 1.21 (30px on mobile). Page title (h1).
- **body-md:** AlibabaSans 14px at weight 400, line height 1.57. Body text.
- **body-lg:** system-ui 16px at weight 400, line height 1.5. Lead paragraphs.
- **label-md:** AlibabaSans 16px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** system-ui 14px at weight 400, line height 1.57. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 70% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 48px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1208px.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 480px, 575px, 576px, 767px, 767.99px, 768px, 991px, 992px, 1199px, 1200px, 1600px, 1920px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.05) 0px 1px 2px 0px, rgba(0, 0, 0, 0.03) 0px 1px 6px -1px, rgba(0, 0, 0, 0.03) 0px 2px 4px 0px`
- `rgba(5, 145, 255, 0.1) 0px 2px 0px 0px`
- `rgba(0, 0, 0, 0.08) 0px 6px 16px 0px, rgba(0, 0, 0, 0.12) 0px 3px 6px -4px, rgba(0, 0, 0, 0.05) 0px 9px 28px 8px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0.14) 0px 106px 36px -116px inset`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **lg (8px):** 190 elements.
- **sm (4px):** 72 elements.
- **full (9999px):** 60 elements.
- **md (6px):** 40 elements.
- **xl (100px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Getting Started”):** #1677FF fill, #FFFFFF text, 16px/400, 8px radius, padding 0px 15px, shadow `rgba(5, 145, 255, 0.1) 0px 2px 0px 0px`.
- **button-primary-hover:** background #4096FF, text #FFFFFF on hover.
- **button-outline (“Design Language”):** #FFFFFF fill, #000000E0 text, 16px/400, 8px radius, padding 0px 15px, border 1px solid #D9D9D9, shadow `rgba(0, 0, 0, 0.02) 0px 2px 0px 0px`.
- **button-outline-hover:** background #FFFFFF, text #4096FF on hover.
- **button-ghost (“Danger button”):** #FFFFFF fill, #FF4D4F text, 14px/400, 6px radius, padding 0px 15px, border 1px solid #FF4D4F, shadow `rgba(255, 38, 5, 0.06) 0px 2px 0px 0px`.
- **input-field (“Type keywords...”):** transparent fill, #000000E0 text, 14px/400, 20px radius, padding 0px 12px 0px 32px.
- **card:** transparent fill, #000000E0 text, 14px/400, 16px radius, padding 32px, border 1px solid #F0F0F0, shadow `rgba(0, 0, 0, 0.08) 0px 4px 12px 0px, rgba(0, 0, 0, 0.08) 0px 12px 32px 0px`.
- **link:** transparent fill, #000000E0 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F0F3FA, #E8F4FD, #FCE9E9.
- Do keep text in 2 levels: #1F1F1F, #595959.
- Do reserve #1677FF for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 4px, 6px and 100px.
- Don't introduce new font families beyond AlibabaSans and system-ui.
- Don't use #1677FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.1s, 0.06s. Longer ambient animations run 1s, 1.2s.

- **Easing:** `ease`, `cubic-bezier(0.645, 0.045, 0.355, 1)`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/ant.design/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
