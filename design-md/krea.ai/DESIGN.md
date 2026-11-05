---
version: alpha
name: Krea
description: "Dark monochrome interface measured from krea.ai: Suisse Intl type, tonal surfaces and 8px corners."
colors:
  background: "#0B0F15"
  surface: "#0B0F15"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#A3A3A3"
  on-surface-muted: "#737373"
  on-surface-subtle: "#404040"
  surface-container-low: "#0D1530"
  surface-container: "#000000"
  surface-container-high: "#262626"
  overlay: "#FFFFFF1A"
  overlay-strong: "#FFFFFF0B"
  outline: "#FFFFFF26"
  outline-variant: "#00000033"
  primary: "#262626"
  on-primary: "#FFFFFF"
  secondary: "#006EFF"
typography:
  display-hero:
    fontFamily: Suisse Intl
    fontSize: 72px
    fontWeight: 600
    lineHeight: 1.05
    letterSpacing: -0.025em
  headline-display:
    fontFamily: Suisse Intl
    fontSize: 60px
    fontWeight: 400
    lineHeight: 1.05
  headline-lg:
    fontFamily: Suisse Intl
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.015em
  headline-md:
    fontFamily: Suisse Intl
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
  headline-sm:
    fontFamily: Suisse Intl
    fontSize: 20px
    fontWeight: 450
    lineHeight: 1.25
  body-md:
    fontFamily: Suisse Intl
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Suisse Intl
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.01em
  body-sm:
    fontFamily: Suisse Intl
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1
  caption:
    fontFamily: Suisse Intl
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-lg:
    fontFamily: Suisse Intl
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Suisse Intl
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.33
  label-sm:
    fontFamily: Suisse Intl
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Suisse Intl
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.05
  headline-lg-mobile:
    fontFamily: Suisse Intl
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.015em
rounded:
  sm: 8px
  md: 14px
  lg: 16px
  xl: 24px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 64px
  gutter: 8px
  section: 160px
  margin: 64px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    padding: 8px 16px
    height: 36px
  button-primary-hover:
    backgroundColor: "#202020"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.surface-container}"
    typography: "{typography.label-lg}"
    padding: 24px 40px
    height: 48px
  button-secondary-hover:
    backgroundColor: "#FFFFFFE6"
  button-outline:
    backgroundColor: "{colors.overlay-strong}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    padding: 24px 40px
    height: 50px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 12px
  card:
    textColor: "#0A0A0A"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 24px 32px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Krea Design System

## Overview

Krea describes itself as: “Generate, edit, and enhance images, videos, and 3D with Krea's AI creative suite. Start free with real-time tools and the best generative models.” The interface is dark, built on **Cool Charcoal (#0B0F15)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Suisse Intl**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [krea.ai](https://www.krea.ai/) on November 4, 2026 at 1440×900 and 390×844 from 449 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles, plus gradient stops #4C9EFF, #155DFC, #2E6CF6, #1A3FB8.

- **Cool Charcoal (#0B0F15):** Page background, seen 1 time. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 43 times. Token `on-surface`, CSS `--color-white`.
- **Gray (#A3A3A3):** Secondary text, seen 12 times. Token `on-surface-variant`, CSS `--color-primary-400`.
- **Slate (#737373):** Muted text and metadata, seen 15 times. Token `on-surface-muted`, CSS `--color-primary-500`.
- **Graphite (#404040):** Subtle text and placeholders, seen 46 times. Token `on-surface-subtle`, CSS `--color-primary-700`.
- **Deep Blue (#0D1530):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Near Black (#000000):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--color-primary-1000`.
- **Graphite (#262626):** Hover and pressed fills, seen 10 times. Token `surface-container-high`, CSS `--color-primary-800`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White 4% (#FFFFFF0B):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White 15% (#FFFFFF26):** Borders and dividers, seen 3 times. Token `outline`.
- **Near Black 20% (#00000033):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Graphite (#262626):** Primary buttons and calls to action, seen 10 times. Token `primary`, CSS `--color-primary-800`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#006EFF):** Accent in text, fills and borders, seen 6 times. Token `secondary`.

## Typography

**Suisse Intl** carries the whole interface. Fallback stack: `Suisse Intl, ui-sans-serif, system-ui, sans-serif`.

- **display-hero:** Suisse Intl 72px at weight 600, line height 1.05, tracking -0.025em. Oversized hero statements.
- **headline-display:** Suisse Intl 60px at weight 400, line height 1.05 (36px on mobile). Page title (h1).
- **headline-lg:** Suisse Intl 30px at weight 600, line height 1.2, tracking -0.015em (24px on mobile). Section headings (h2).
- **headline-md:** Suisse Intl 24px at weight 600, line height 1.33. Sub-section headings.
- **headline-sm:** Suisse Intl 20px at weight 450, line height 1.25. Card and feature titles.
- **body-md:** Suisse Intl 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Suisse Intl 15px at weight 400, line height 1.5, tracking 0.01em. Lead paragraphs.
- **body-sm:** Suisse Intl 13px at weight 400, line height 1. Secondary and small text.
- **caption:** Suisse Intl 12px at weight 400, line height 1.33. Captions and fine print.
- **label-lg:** Suisse Intl 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** Suisse Intl 15px at weight 500, line height 1.33. Buttons, navigation and labels.
- **label-sm:** Suisse Intl 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (81% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 64px.
- **Sections:** 160px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 64px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 6px 0px`
- `rgba(255, 255, 255, 0.9) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px, rgba(0, 0, 0, 0.28) 0px 18px 40px -28px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 124 elements.
- **md (14px):** 32 elements.
- **xl (24px):** 30 elements.
- **lg (16px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Log in”):** #262626 fill, #FFFFFF text, 14px/450, 3.35544e+07px radius, padding 8px 16px.
- **button-primary-hover:** background #202020, text #FFFFFF on hover.
- **button-secondary (“Open Krea”):** #FFFFFF fill, #000000 text, 16px/450, 3.35544e+07px radius, padding 24px 40px.
- **button-secondary-hover:** background #FFFFFFE6, text #000000 on hover.
- **button-outline (“Krea Agent”):** #FFFFFF0B fill, #FFFFFF text, 16px/450, 3.35544e+07px radius, padding 24px 40px, border 1px solid #FFFFFF26, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.999994 0.0000455678 0.0000200868 / 0.1) 0px 0px 0px 0.5px inset, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`.
- **button-ghost (“Features”):** transparent fill, #FFFFFF text, 15px/400, 8px radius, padding 12px.
- **card:** transparent fill, #0A0A0A text, 16px/400, 16px radius, padding 24px 32px, shadow `rgba(255, 255, 255, 0.9) 0px 1px 0px 0px inset, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px, rgba(0, 0, 0, 0.28) 0px 18px 40px -28px`.
- **link:** transparent fill, #737373 text, padding 0px.

## Do's and Don'ts

- Do use #0B0F15 for the page and lift surfaces in small steps: #0D1530, #000000, #262626.
- Do keep text in 4 levels: #FFFFFF, #A3A3A3, #737373, #404040.
- Do let contrast carry emphasis; primary actions use #262626 on #0B0F15.
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 8px corners on most elements; larger surfaces also use 14px, 24px and 16px.
- Don't use #737373 for body text; it reaches 4.05:1 on #0B0F15. Keep it for large text or metadata.
- Don't use #404040 for body text; it reaches 1.85:1 on #0B0F15. Keep it for large text or metadata.
- Don't introduce new font families beyond Suisse Intl.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.4s, 0.15s. Longer ambient animations run 0.7s.

- **Easing:** `cubic-bezier(0, 0, 0.2, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/krea.ai/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
