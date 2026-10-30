---
version: alpha
name: Dub
description: "Light monochrome interface measured from dub.co: satoshi type with Inter, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#737373"
  on-background: "#737373"
  on-surface-strong: "#171717"
  on-surface-variant: "#262626"
  on-surface-muted: "#525252"
  surface-container-low: "#FAFAFA"
  surface-container: "#F5F5F5"
  surface-container-high: "#E5E5E5"
  overlay: "#FFFFFF33"
  outline: "#E5E5E5"
  outline-variant: "#0000000D"
  primary: "#737373"
  on-primary: "#FFFFFF"
  inverse-surface: "#000000"
  secondary: "#C084FC"
  tertiary: "#4ADE80"
typography:
  headline-display:
    fontFamily: satoshi
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
  headline-lg:
    fontFamily: satoshi
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.11
  headline-md:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.38
  headline-sm:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.33
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
  code:
    fontFamily: GeistMono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: satoshi
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
rounded:
  sm: 4px
  md: 6px
  lg: 8px
  xl: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 48px
  gutter: 8px
components:
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "#0A0A0A"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 0px
    height: 80px
  button-ghost:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 0px
    height: 80px
  link:
    textColor: "{colors.primary}"
---

# Dub Design System

## Overview

Dub describes itself as: “Dub is the modern link attribution platform for short links, conversion tracking, and affiliate programs.” The interface is light, built on **White (#FFFFFF)** with **Slate (#737373)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **satoshi** and **Inter**, with **GeistMono** for code. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [dub.co](https://dub.co/) on October 29, 2026 at 1440×900 and 390×844 from 416 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #F97316.

- **White (#FFFFFF):** Page background, seen 17 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Slate (#737373):** Primary text and headings, seen 51 times. Token `on-surface`.
- **Charcoal (#171717):** Headings and emphasis, seen 38 times. Token `on-surface-strong`.
- **Graphite (#262626):** Secondary text, seen 18 times. Token `on-surface-variant`.
- **Slate (#525252):** Muted text and metadata, seen 8 times. Token `on-surface-muted`.
- **Snow (#FAFAFA):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`.
- **Snow (#F5F5F5):** Cards and panels, seen 15 times. Token `surface-container`.
- **Mist (#E5E5E5):** Hover and pressed fills, seen 2 times. Token `surface-container-high`.
- **White 20% (#FFFFFF33):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Mist (#E5E5E5):** Borders and dividers, seen 49 times. Token `outline`.
- **Near Black 5% (#0000000D):** Secondary dividers, seen 9 times. Token `outline-variant`.
- **Slate (#737373):** Primary actions (the main text color; the palette is monochrome), seen 53 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000000):** High-contrast fills, seen 2 times. Token `inverse-surface`.
- **Light Violet (#C084FC):** Accent in text, fills and borders, seen 3 times. Token `secondary`.
- **Green (#4ADE80):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.

## Typography

**satoshi**, **Inter** and **GeistMono** (monospace) share the interface. Fallback stack: `satoshi, satoshi Fallback, system-ui, sans-serif`.

- **headline-display:** satoshi 48px at weight 500, line height 1 (30px on mobile). Page title (h1).
- **headline-lg:** satoshi 36px at weight 500, line height 1.11. Section headings (h2).
- **headline-md:** Inter 30px at weight 400, line height 1.38. Sub-section headings.
- **headline-sm:** Inter 24px at weight 400, line height 1.33. Card and feature titles.
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Inter 18px at weight 400, line height 1.56. Lead paragraphs.
- **body-sm:** Inter 14px at weight 400, line height 1.43. Secondary and small text.
- **caption:** Inter 12px at weight 400, line height 1.33. Captions and fine print.
- **label-md:** Inter 14px at weight 500, line height 1.43. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 500, line height 1.33. Small labels and badges.
- **code:** GeistMono 14px at weight 400, line height 1.43. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (86% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 280px, 281px, 360px, 420px, 450px, 640px, 768px, 900px, 1024px, 1280px, 1400px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **lg (8px):** 132 elements.
- **xl (12px):** 32 elements.
- **sm (4px):** 28 elements.
- **full (9999px):** 20 elements.
- **md (6px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“View all customers”):** #F5F5F5 fill, #0A0A0A text, 16px/400, 12px radius, padding 0px.
- **button-ghost (“CASE STUDY”):** #F5F5F5 fill, #737373 text, 16px/400, 12px radius, padding 0px.
- **link:** transparent fill, #737373 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAFAFA, #F5F5F5, #E5E5E5.
- Do keep text in 4 levels: #737373, #171717, #262626, #525252.
- Do let contrast carry emphasis; primary actions use #737373 on #FFFFFF.
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do use 8px corners on most elements; larger surfaces also use 12px, 4px and 6px.
- Don't introduce new font families beyond satoshi, Inter and GeistMono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.5s, 0.075s, 0.1s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.16, 1, 0.3, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/dub.co/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
