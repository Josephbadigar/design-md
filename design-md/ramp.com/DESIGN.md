---
version: alpha
name: Ramp
description: "Light monochrome interface measured from ramp.com: Lausanne type, tonal surfaces and 16px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0C0A08"
  on-background: "#0C0A08"
  on-surface-variant: "#6D6C6B"
  surface-container-low: "#F4F2F0"
  overlay: "#2121210D"
  overlay-strong: "#1A19190D"
  outline: "#E5E7EB"
  outline-variant: "#2121211A"
  primary: "#1A1919"
  on-primary: "#FFFFFF"
  secondary: "#E4F222"
typography:
  headline-display:
    fontFamily: Lausanne
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1
  headline-lg:
    fontFamily: Lausanne
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.04
  headline-md:
    fontFamily: Lausanne
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.05
  headline-sm:
    fontFamily: Lausanne
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.14
  title-lg:
    fontFamily: Lausanne
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.17
  body-md:
    fontFamily: Lausanne
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Lausanne
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.46
  label-md:
    fontFamily: Lausanne
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Lausanne
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.05
  headline-sm-mobile:
    fontFamily: Lausanne
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.18
  title-lg-mobile:
    fontFamily: Lausanne
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.2
rounded:
  xs: 4px
  sm: 6px
  md: 10px
  lg: 12px
  xl: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 64px
  gutter: 8px
  section: 128px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
    height: 34px
  button-outline:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
    height: 34px
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 16px
    height: 43px
  link:
    textColor: "{colors.on-surface}"
---

# Ramp Design System

## Overview

Ramp describes itself as: “Make expense management easy with Ramp's spend management platform. Combine global corporate cards, travel, expenses and accounts payable to automate finance operations and improve efficiency.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#0C0A08)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Lausanne**. Headlines run large; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 16px.

Measured from [ramp.com](https://ramp.com/) on October 29, 2026 at 1440×900 and 390×844 from 412 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 26 times. Token `background`, CSS `--fides-overlay-primary-button-text-color`.
- **Near Black (#0C0A08):** Primary text and headings, seen 56 times. Token `on-surface`.
- **Slate (#6D6C6B):** Secondary text, seen 49 times. Token `on-surface-variant`.
- **Mist (#F4F2F0):** Raised areas one step from the page, seen 10 times. Token `surface-container-low`.
- **Charcoal 5% (#2121210D):** Translucent fill for cards and controls, seen 8 times. Token `overlay`.
- **Charcoal 5% (#1A19190D):** Stronger translucent fill, seen 4 times. Token `overlay-strong`.
- **Cool Mist (#E5E7EB):** Borders and dividers, seen 22 times. Token `outline`.
- **Charcoal 10% (#2121211A):** Secondary dividers, seen 5 times. Token `outline-variant`.
- **Charcoal (#1A1919):** Primary buttons and calls to action, seen 2 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Yellow (#E4F222):** Accent in text, fills and borders, seen 5 times. Token `secondary`.

## Typography

**Lausanne** carries the whole interface. Fallback stack: `Lausanne, Arial, sans-serif`. Other loaded fonts: Material Icons, Material Icons Outlined.

- **headline-display:** Lausanne 64px at weight 400, line height 1 (40px on mobile). Page title (h1).
- **headline-lg:** Lausanne 48px at weight 400, line height 1.04. Section headings (h2).
- **headline-md:** Lausanne 40px at weight 400, line height 1.05. Sub-section headings.
- **headline-sm:** Lausanne 28px at weight 400, line height 1.14 (22px on mobile). Card and feature titles.
- **title-lg:** Lausanne 24px at weight 400, line height 1.17 (20px on mobile). Small titles.
- **body-md:** Lausanne 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Lausanne 13px at weight 400, line height 1.46. Secondary and small text.
- **label-md:** Lausanne 14px at weight 400, line height 1.43. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (88% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 64px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 380px, 480px, 600px, 601px, 701px, 768px, 992px, 1024px, 1100px, 1280px, 1360px, 1440px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F4F2F0) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(255, 255, 255, 0.6) 0px 0px 2px 0px inset`

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **xl (16px):** 96 elements.
- **lg (12px):** 64 elements.
- **sm (6px):** 56 elements.
- **xs (4px):** 40 elements.
- **md (10px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #1A1919 fill, #FFFFFF text, 14px/400, 6px radius, padding 12px 16px.
- **button-outline (“See a demo”):** #E4F222 fill, #0C0A08 text, 14px/400, 6px radius, padding 12px 16px.
- **button-ghost (“View Demo”):** #F4F2F0 fill, #0C0A08 text, 16px/400, 6px radius, padding 16px.
- **link:** transparent fill, #0C0A08 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F4F2F0.
- Do keep text in 2 levels: #0C0A08, #6D6C6B.
- Do let contrast carry emphasis; primary actions use #1A1919 on #FFFFFF.
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do use 16px corners on most elements; larger surfaces also use 12px, 6px and 4px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Lausanne.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.4s, 0.3s, 0.24s, 0.25s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.45, 0.05, 0.55, 0.95)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/ramp.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
