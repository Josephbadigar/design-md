---
version: alpha
name: daisyUI
description: "Light monochrome interface measured from daisyui.com: Outfit type with system-ui, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#18181B"
  on-background: "#18181B"
  on-surface-variant: "#5D5D5F"
  on-surface-muted: "#71717B"
  surface-container-low: "#F8F8F8"
  overlay: "#18181B80"
  outline: "#18181B33"
  outline-variant: "#E8E8E8"
  primary: "#09090B"
  on-primary: "#E4E4E7"
  secondary: "#EC003F"
  tertiary: "#F43098"
  success: "#00D390"
  error: "#FF637D"
typography:
  display-hero:
    fontFamily: Outfit
    fontSize: 72px
    fontWeight: 900
    lineHeight: 1
  headline-display:
    fontFamily: Outfit
    fontSize: 50.5px
    fontWeight: 400
    lineHeight: 1.1
  headline-lg:
    fontFamily: Outfit
    fontSize: 36px
    fontWeight: 300
    lineHeight: 1.11
  headline-md:
    fontFamily: Outfit
    fontSize: 30px
    fontWeight: 300
    lineHeight: 1.2
  headline-sm:
    fontFamily: Outfit
    fontSize: 24px
    fontWeight: 300
    lineHeight: 1.33
  body-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 300
    lineHeight: 1.43
  body-lg:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: system-ui
    fontSize: 10px
    fontWeight: 400
    lineHeight: 2
    letterSpacing: 0.025em
  label-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.75
  headline-display-mobile:
    fontFamily: Outfit
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.1
  display-hero-mobile:
    fontFamily: Outfit
    fontSize: 32px
    fontWeight: 900
    lineHeight: 1
rounded:
  sm: 4px
  md: 8px
  lg: 11px
  xl: 40px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 16px
  section: 80px
  margin: 16px
  container: 1280px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    padding: 0px 20px
    height: 48px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    padding: 0px 12px
    height: 32px
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 11px 1px 11px
    height: 51px
  card:
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# daisyUI Design System

## Overview

daisyUI describes itself as: “Tailwind CSS component library by daisyUI. Build faster with semantic components, built-in themes, and reusable UI blocks.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#18181B)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Outfit** and **system-ui**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [daisyui.com](https://daisyui.com/) on November 4, 2026 at 1440×900 and 390×844 from 443 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #F43098, #FD4B89, #422AD5, #0093DF.

- **White (#FFFFFF):** Page background, seen 14 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Charcoal (#18181B):** Primary text and headings, seen 60 times. Token `on-surface`.
- **Slate (#5D5D5F):** Secondary text, seen 28 times. Token `on-surface-variant`.
- **Cool Slate (#71717B):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Snow (#F8F8F8):** Raised areas one step from the page, seen 43 times. Token `surface-container-low`.
- **Charcoal 50% (#18181B80):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Charcoal 20% (#18181B33):** Borders and dividers, seen 11 times. Token `outline`.
- **Mist (#E8E8E8):** Secondary dividers, seen 5 times. Token `outline-variant`.
- **Near Black (#09090B):** Primary buttons and calls to action, seen 8 times. Token `primary`.
- **Mist (#E4E4E7):** Text and icons on primary. Token `on-primary`.
- **Vivid Pink (#EC003F):** Accent in text, fills and borders, seen 12 times. Token `secondary`.
- **Vivid Pink (#F43098):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.
- **Teal (#00D390):** Success and positive states, seen 5 times. Token `success`.
- **Red (#FF637D):** Errors and destructive states, seen 2 times. Token `error`.

## Typography

**Outfit** and **system-ui** share the interface. Fallback stack: `Outfit, Noto Sans JP, Noto Sans, Vazirmatn`.

- **display-hero:** Outfit 72px at weight 900, line height 1 (32px on mobile). Oversized hero statements.
- **headline-display:** Outfit 50.5px at weight 400, line height 1.1 (24px on mobile). Page title (h1).
- **headline-lg:** Outfit 36px at weight 300, line height 1.11. Section headings (h2).
- **headline-md:** Outfit 30px at weight 300, line height 1.2. Sub-section headings.
- **headline-sm:** Outfit 24px at weight 300, line height 1.33. Card and feature titles.
- **body-md:** system-ui 14px at weight 300, line height 1.43. Body text.
- **body-lg:** system-ui 16px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** system-ui 10px at weight 400, line height 2, tracking 0.025em. Secondary and small text.
- **label-md:** system-ui 14px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** system-ui 12px at weight 400, line height 1.75. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (82% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1280px.
- **Page margin:** 16px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `oklch(1 0 0 / 0.06) 0px 0.5px 0px 0.5px inset, oklab(0.98 0 0 / 0.3) 0px 3px 2px -2px, oklab(0.98 0 0 / 0.3) 0px 4px 3px -2px`
- `oklch(1 0 0 / 0) 0px 0.5px 0px 0.5px inset, oklab(0 0 0 / 0) 0px 3px 2px -2px, oklab(0 0 0 / 0) 0px 4px 3px -2px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px inset, oklch(1 0 0 / 0.1) 0px 8px 0px -4px inset, oklch(0 0 0 / 0.1) 0px 1px 0px 0px`

Hairline rings and inset highlights also appear: `oklch(0 0 0 / 0) 0px 0px 0px 0px inset, oklch(0 0 0 / 0) 0px 0px 0px 0px`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 159 elements.
- **sm (4px):** 90 elements.
- **xl (40px):** 37 elements.
- **lg (11px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“How to use?”):** #09090B fill, #E4E4E7 text, 18px/600, 3.35544e+07px radius, padding 0px 20px, border 1px solid #08080A, shadow `oklch(1 0 0 / 0.06) 0px 0.5px 0px 0.5px inset, oklab(0.14 0.00136333 -0.00481054 / 0.3) 0px 3px 2px -2px, oklab(0.14 0.00136333 -0.00481054 / 0.3) 0px 4px 3px -2px`.
- **button-outline (“npx skills add saadeghi/daisyui”):** #F8F8F8 fill, #18181B text, 12px/300, 3.35544e+07px radius, padding 0px 12px, border 1px solid #E8E8E8, shadow `oklch(1 0 0 / 0.06) 0px 0.5px 0px 0.5px inset, oklab(0.98 0 0 / 0.3) 0px 3px 2px -2px, oklab(0.98 0 0 / 0.3) 0px 4px 3px -2px`.
- **button-ghost (“Features”):** #FFFFFF fill, #18181B text, 12px/400, 4px 4px 0px 0px radius, padding 0px 11px 1px 11px.
- **card:** transparent fill, 16px/400, 8px radius, padding 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px, rgba(0, 0, 0, 0.07) 0px 0px 0px 0px`.
- **link:** transparent fill, #18181BB3 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8F8F8.
- Do keep text in 3 levels: #18181B, #5D5D5F, #71717B.
- Do let contrast carry emphasis; primary actions use #09090B on #FFFFFF.
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do use 8px corners on most elements; larger surfaces also use 4px, 40px and 11px.
- Don't introduce new font families beyond Outfit and system-ui.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.5s, 0.15s.

- **Easing:** `ease-in-out`, `ease`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/daisyui.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
