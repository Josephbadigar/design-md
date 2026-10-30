---
version: alpha
name: Shopify
description: "Dark monochrome interface measured from shopify.com: Shopify-Inter type, tonal surfaces and 8px corners."
colors:
  background: "#02090A"
  surface: "#02090A"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#9DABAD"
  on-surface-muted: "#A1A1AA"
  on-surface-subtle: "#9797A2"
  surface-container-low: "#000A1E"
  surface-container: "#000000"
  surface-container-high: "#051517"
  surface-container-highest: "#061A1C"
  overlay: "#FFFFFF33"
  overlay-strong: "#FFFFFF1A"
  outline: "#FFFFFF1A"
  outline-variant: "#11352D"
  primary: "#FFFFFF"
  on-primary: "#000000"
  secondary: "#7126FF"
typography:
  headline-display:
    fontFamily: Shopify-Inter
    fontSize: 96px
    fontWeight: 300
    lineHeight: 1.08
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Shopify-Inter
    fontSize: 64px
    fontWeight: 330
    lineHeight: 1.08
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Shopify-Inter
    fontSize: 56px
    fontWeight: 330
    lineHeight: 1.08
    letterSpacing: -0.03em
  headline-sm:
    fontFamily: Shopify-Inter
    fontSize: 44px
    fontWeight: 330
    lineHeight: 1.1
    letterSpacing: -0.01em
  title-lg:
    fontFamily: Shopify-Inter
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.01em
  body-md:
    fontFamily: Shopify-Inter
    fontSize: 14px
    fontWeight: 420
    lineHeight: 1.43
  body-lg:
    fontFamily: Shopify-Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: Shopify-Inter
    fontSize: 12px
    fontWeight: 420
    lineHeight: 1.2
    letterSpacing: 0.06em
  label-md:
    fontFamily: Shopify-Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  code:
    fontFamily: ui-monospace
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  headline-display-mobile:
    fontFamily: Shopify-Inter
    fontSize: 56px
    fontWeight: 330
    lineHeight: 1.08
    letterSpacing: -0.02em
  headline-md-mobile:
    fontFamily: Shopify-Inter
    fontSize: 36px
    fontWeight: 330
    lineHeight: 1.12
    letterSpacing: -0.02em
rounded:
  sm: 4px
  md: 8px
  lg: 12px
  xl: 48px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 64px
  gutter: 64px
  section: 64px
  margin: 90px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 8px 20px
    height: 44px
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 8px 13px
    height: 44px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 8px 13px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 72px 0px 0px 0px
  link:
    textColor: "{colors.primary}"
---

# Shopify Design System

## Overview

Shopify describes itself as: “Try Shopify free. Build or grow your business fast with AI. Get more than ecommerce software with tools to manage every part of your business.” The interface is dark, built on **Near Black (#02090A)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Shopify-Inter**, with **ui-monospace** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [shopify.com](https://www.shopify.com/) on October 29, 2026 at 1440×900 and 390×844 from 303 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #D6FFF0F2, #244749, #182E2F, #30DEEE.

- **Near Black (#02090A):** Page background, seen 12 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 48 times. Token `on-surface`, CSS `--tw-ring-offset-color`.
- **Cool Gray (#9DABAD):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Cool Gray (#A1A1AA):** Muted text and metadata, seen 24 times. Token `on-surface-muted`, CSS `--color-link-dark-active`.
- **Cool Gray (#9797A2):** Subtle text and placeholders, seen 14 times. Token `on-surface-subtle`.
- **Deep Blue (#000A1E):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Near Black (#000000):** Cards and panels, seen 2 times. Token `surface-container`.
- **Deep Cyan (#051517):** Hover and pressed fills, seen 2 times. Token `surface-container-high`.
- **Deep Cyan (#061A1C):** Highest raised elements, seen 4 times. Token `surface-container-highest`.
- **White 20% (#FFFFFF33):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **White 10% (#FFFFFF1A):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 3 times. Token `outline`.
- **Deep Teal (#11352D):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 65 times. Token `primary`, CSS `--tw-ring-offset-color`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Violet (#7126FF):** Accent, seen 1 time. Token `secondary`.

## Typography

**Shopify-Inter** and **ui-monospace** (monospace) share the interface. Fallback stack: `Shopify-Inter, Helvetica, Arial, sans-serif`.

- **headline-display:** Shopify-Inter 96px at weight 300, line height 1.08, tracking -0.02em (56px on mobile). Page title (h1).
- **headline-lg:** Shopify-Inter 64px at weight 330, line height 1.08, tracking -0.02em. Section headings (h2).
- **headline-md:** Shopify-Inter 56px at weight 330, line height 1.08, tracking -0.03em (36px on mobile). Sub-section headings.
- **headline-sm:** Shopify-Inter 44px at weight 330, line height 1.1, tracking -0.01em. Card and feature titles.
- **title-lg:** Shopify-Inter 24px at weight 400, line height 1.3, tracking -0.01em. Small titles.
- **body-md:** Shopify-Inter 14px at weight 420, line height 1.43. Body text.
- **body-lg:** Shopify-Inter 18px at weight 400, line height 1.4. Lead paragraphs.
- **body-sm:** Shopify-Inter 12px at weight 420, line height 1.2, tracking 0.06em. Secondary and small text.
- **label-md:** Shopify-Inter 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **code:** ui-monospace 12px at weight 400, line height 1.33, uppercase. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (77% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 64px is the most common gap in flex and grid layouts.
- **Page margin:** 90px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(255, 255, 255, 0.05) 0px 1px 2px 0px, rgba(255, 255, 255, 0.04) 0px 1px 0px 0px inset`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 8px 8px 0px, rgba(0, 0, 0, 0.1) 0px 4px 4px 0px, rgba(0, 0, 0, 0.1) 0px 2px 2px 0px, rgba(0, 0, 0, 0.1) 0px 0px 0px 1px, rgba(255, 255, 255, 0.03) 0px 1px 0px 0px inset`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(255, 255, 255, 0.03) 0px 0.929px 0px 0px inset, rgba(0, 0, 0, 0.1) 0px 0px 0px 0.929px, rgba(0, 0, 0, 0.1) 0px 1.858px 1.858px 0px, rgba(0, 0, 0, 0.1) 0px 3.717px 3.717px 0px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(255, 255, 255) 0px 0px 0px 0px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 92 elements.
- **full (9999px):** 28 elements.
- **sm (4px):** 24 elements.
- **lg (12px):** 24 elements.
- **xl (48px):** 6 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for free”):** #FFFFFF fill, #000000 text, 16px/550, 9999px radius, padding 8px 20px.
- **button-outline (“Fall '26 Edition”):** transparent fill, #FFFFFF text, 16px/550, 9999px radius, padding 8px 13px, border 2px solid #FFFFFF, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(255, 255, 255) 0px 0px 0px 0px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-ghost (“Fall '26 Edition”):** transparent fill, #FFFFFF text, 16px/550, 9999px radius, padding 8px 13px, border 2px solid #FFFFFF, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(255, 255, 255) 0px 0px 0px 0px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **card:** #02090A fill, #FFFFFF text, 16px/400, padding 72px 0px 0px 0px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #02090A for the page and lift surfaces in small steps: #000A1E, #000000, #051517, #061A1C.
- Do keep text in 4 levels: #FFFFFF, #9DABAD, #A1A1AA, #9797A2.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #02090A.
- Do set headlines in Shopify-Inter with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 4px, 12px and 48px.
- Don't introduce new font families beyond Shopify-Inter and ui-monospace.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.15s, 0.5s. Longer ambient animations run 80s, 8s, 0.7s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `linear`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/shopify.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
