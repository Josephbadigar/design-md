---
version: alpha
name: HeroUI
description: "Light interface measured from heroui.com: Inter type, vivid blue accents, tonal surfaces and 24px corners."
colors:
  background: "#F5F5F5"
  surface: "#F5F5F5"
  on-surface: "#18181B"
  on-background: "#18181B"
  on-surface-variant: "#71717A"
  surface-container-low: "#F9F9F9"
  surface-container: "#FCFCFC"
  surface-container-high: "#FFFFFF"
  surface-container-highest: "#EBEBEC"
  overlay: "#00BCFF26"
  overlay-strong: "#F5A52426"
  outline: "#DDDEE0"
  primary: "#0485F7"
  on-primary: "#FCFCFC"
  inverse-surface: "#000000"
  secondary: "#1E63AE"
  error: "#FF383C"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.07
    letterSpacing: -0.03em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
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
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
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
    fontFamily: monospace
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.5em
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.025em
rounded:
  sm: 8px
  md: 12px
  lg: 16px
  xl: 24px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 48px
  gutter: 8px
  section: 48px
  margin: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 0px 16px 0px 20px
    height: 40px
  button-outline:
    backgroundColor: "{colors.surface-container-highest}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 0px 12px
    height: 32px
  button-ghost:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 8px 28px 8px 12px
    height: 36px
  card:
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 16px
  link:
    textColor: "{colors.on-surface-variant}"
---

# HeroUI Design System

## Overview

HeroUI describes itself as: “Beautiful, accessible React UI components built on React Aria and Tailwind CSS v4. The modern alternative to MUI, Chakra UI, and shadcn/ui for building production-ready applications.” The interface is light, built on **Snow (#F5F5F5)** with **Charcoal (#18181B)** text, and **Vivid Blue (#0485F7)** as the main accent.

Type is set in **Inter**, with **monospace** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 24px.

Measured from [heroui.com](https://heroui.com/) on November 4, 2026 at 1440×900 and 390×844 from 301 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **Snow (#F5F5F5):** Page background, seen 2 times. Token `background`.
- **Charcoal (#18181B):** Primary text and headings, seen 43 times. Token `on-surface`.
- **Cool Slate (#71717A):** Secondary text, seen 38 times. Token `on-surface-variant`.
- **Snow (#F9F9F9):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--color-fd-secondary`.
- **Snow (#FCFCFC):** Cards and panels, seen 3 times. Token `surface-container`.
- **White (#FFFFFF):** Hover and pressed fills, seen 12 times. Token `surface-container-high`.
- **Mist (#EBEBEC):** Highest raised elements, seen 26 times. Token `surface-container-highest`.
- **Vivid Cyan 15% (#00BCFF26):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Vivid Orange 15% (#F5A52426):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Silver (#DDDEE0):** Borders and dividers, seen 2 times. Token `outline`.
- **Vivid Blue (#0485F7):** Primary buttons and calls to action, seen 8 times. Token `primary`.
- **Snow (#FCFCFC):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000000):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Blue (#1E63AE):** Accent, seen 1 time. Token `secondary`.
- **Vivid Red (#FF383C):** Errors and destructive states, seen 4 times. Token `error`.

## Typography

**Inter** and **monospace** (monospace) share the interface. Fallback stack: `Inter, Inter Fallback, ui-sans-serif, system-ui`.

- **headline-display:** Inter 56px at weight 700, line height 1.07, tracking -0.03em (30px on mobile). Page title (h1).
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Inter 14px at weight 400, line height 1.43. Secondary and small text.
- **caption:** Inter 12px at weight 400, line height 1.33. Captions and fine print.
- **label-lg:** Inter 16px at weight 600, line height 1.5. Large buttons and tabs.
- **label-md:** Inter 14px at weight 500, line height 1.43. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 500, line height 1.33. Small labels and badges.
- **code:** monospace 40px at weight 400, line height 1, tracking -0.5em. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (88% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 16px on each side of full-width sections.
- **Breakpoints:** 600px, 1200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.04) 0px 2px 4px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px, rgba(0, 0, 0, 0.06) 0px 0px 1px 0px`
- `rgba(0, 0, 0, 0.02) 0px 0px 5px 0px, rgba(0, 0, 0, 0.06) 0px 2px 10px 0px, rgba(0, 0, 0, 0.3) 0px 0px 1px 0px`

## Shapes

Most elements use 24px corners. Measured radii, most used first:

- **xl (24px):** 148 elements.
- **md (12px):** 40 elements.
- **sm (8px):** 16 elements.
- **lg (16px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #0485F7 fill, #FCFCFC text, 14px/500, 24px radius, padding 0px 16px 0px 20px.
- **button-outline (“Click me”):** #EBEBEC fill, #18181B text, 14px/500, 24px radius, padding 0px 12px.
- **button-ghost (“Select one”):** #FFFFFF fill, #71717A text, 14px/400, 12px radius, padding 8px 28px 8px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.04) 0px 2px 4px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px, rgba(0, 0, 0, 0.06) 0px 0px 1px 0px`.
- **card:** transparent fill, 16px/400, 24px radius, padding 16px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.04) 0px 2px 4px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px, rgba(0, 0, 0, 0.06) 0px 0px 1px 0px`.
- **link:** transparent fill, #71717A text, padding 0px.

## Do's and Don'ts

- Do use #F5F5F5 for the page and lift surfaces in small steps: #F9F9F9, #FCFCFC, #FFFFFF, #EBEBEC.
- Do keep text in 2 levels: #18181B, #71717A.
- Do reserve #0485F7 for primary actions and key highlights.
- Do set headlines in Inter with tight tracking (-0.03em).
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 24px corners on most elements; larger surfaces also use 12px, 8px and 16px.
- Don't use #71717A for body text; it reaches 4.43:1 on #F5F5F5. Keep it for large text or metadata.
- Don't introduce new font families beyond Inter and monospace.
- Don't use #0485F7 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.1s, 0.15s, 0.25s, 0.2s. Longer ambient animations run 0.75s.

- **Easing:** `cubic-bezier(0, 0, 0.2, 1)`, `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/heroui.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
