---
version: alpha
name: Amplitude
description: "Light interface measured from amplitude.com: Gellix type with IBM Plex Sans, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#50565B"
  on-surface-muted: "#565656"
  on-surface-subtle: "#868D95"
  surface-container-low: "#F5F7FA"
  overlay: "#F5F7FACC"
  overlay-strong: "#00000033"
  outline: "#E2E4E9"
  outline-variant: "#00000033"
  primary: "#1E61F0"
  on-primary: "#FFFFFF"
  secondary: "#0052F2"
typography:
  headline-display:
    fontFamily: Gellix
    fontSize: 72px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.014em
  headline-lg:
    fontFamily: Gellix
    fontSize: 44px
    fontWeight: 600
    lineHeight: 1.09
    letterSpacing: -0.011em
  headline-md:
    fontFamily: Gellix
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.11
    letterSpacing: -0.018em
  headline-sm:
    fontFamily: Gellix
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.005em
  title-lg:
    fontFamily: Gellix
    fontSize: 22px
    fontWeight: 600
    lineHeight: 1.09
    letterSpacing: -0.023em
  body-md:
    fontFamily: IBM Plex Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-sm:
    fontFamily: Gellix
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  caption:
    fontFamily: Gellix
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.23
  label-lg:
    fontFamily: Gellix
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  label-md:
    fontFamily: Gellix
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.35
  label-sm:
    fontFamily: Gellix
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.35
    letterSpacing: -0.003em
  headline-lg-mobile:
    fontFamily: Gellix
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.13
    letterSpacing: -0.008em
rounded:
  sm: 1px
  md: 4px
  lg: 8px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 30px
    padding: 12px 30px
    height: 46px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px 12px
    height: 48px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.primary}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-primary}"
---

# Amplitude Design System

## Overview

Amplitude describes itself as: “From analytics to feedback to code, Amplitude brings AI into every step of building self-improving products. Start free with 2M events per month.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Blue (#1E61F0)** as the main accent.

Type is set in **Gellix** and **IBM Plex Sans**. Headlines run large with tight negative tracking; body text is 18px. The surface language is flat. Controls are pill-shaped.

Measured from [amplitude.com](https://amplitude.com/) on October 21, 2026 at 1440×900 and 390×844 from 400 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 6 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Near Black (#000000):** Primary text and headings, seen 75 times. Token `on-surface`.
- **Cool Slate (#50565B):** Secondary text, seen 24 times. Token `on-surface-variant`.
- **Slate (#565656):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Cool Gray (#868D95):** Subtle text and placeholders, seen 5 times. Token `on-surface-subtle`.
- **Snow (#F5F7FA):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **Snow 80% (#F5F7FACC):** Translucent fill for cards and controls, seen 11 times. Token `overlay`.
- **Near Black 20% (#00000033):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Cool Mist (#E2E4E9):** Borders and dividers, seen 5 times. Token `outline`.
- **Near Black 20% (#00000033):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Vivid Blue (#1E61F0):** Primary buttons and calls to action, seen 27 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0052F2):** Most used accent color, seen 10 times. Token `secondary`.

## Typography

**Gellix** and **IBM Plex Sans** share the interface. Fallback stack: `Twemoji Country Flags, Gellix, Arial, ui-sans-serif`.

- **headline-display:** Gellix 72px at weight 600, line height 1, tracking -0.014em. Page title (h1).
- **headline-lg:** Gellix 44px at weight 600, line height 1.09, tracking -0.011em (32px on mobile). Section headings (h2).
- **headline-md:** Gellix 28px at weight 600, line height 1.11, tracking -0.018em. Sub-section headings.
- **headline-sm:** Gellix 24px at weight 600, line height 1.25, tracking -0.005em. Card and feature titles.
- **title-lg:** Gellix 22px at weight 600, line height 1.09, tracking -0.023em. Small titles.
- **body-md:** IBM Plex Sans 18px at weight 400, line height 1.56. Body text.
- **body-sm:** Gellix 14px at weight 400, line height 1.43. Secondary and small text.
- **caption:** Gellix 13px at weight 400, line height 1.23. Captions and fine print.
- **label-lg:** Gellix 18px at weight 400, line height 1.56. Large buttons and tabs.
- **label-md:** Gellix 16px at weight 600, line height 1.35. Buttons, navigation and labels.
- **label-sm:** Gellix 14px at weight 600, line height 1.35, tracking -0.003em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 64% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 16px, lg 24px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 380px, 480px, 500px, 600px, 620px, 640px, 650px, 680px, 700px, 768px, 769px, 992px, 1000px, 1130px, 1200px, 1342px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F5F7FA) and #E2E4E9 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (4px):** 76 elements.
- **full (9999px):** 60 elements.
- **sm (1px):** 16 elements.
- **lg (8px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Accept”):** #1E61F0 fill, #FFFFFF text, 16px/600, 30px radius, padding 12px 30px.
- **button-outline (“Agent Analytics”):** #F5F7FA fill, #000000 text, 16px/600, padding 0px 12px.
- **button-secondary (“Get started”):** #000000 fill, #FFFFFF text, 16px/600, 9999px radius, padding 0px 16px, border 1px solid #000000.
- **button-ghost (“Manage Settings”):** transparent fill, #1E61F0 text, 14px/400, padding 0px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5F7FA.
- Do keep text in 4 levels: #000000, #50565B, #565656, #868D95.
- Do reserve #1E61F0 for primary actions and key highlights.
- Do set headlines in Gellix with tight tracking (-0.014em).
- Do reuse the measured spacing steps (6px, 16px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't use #868D95 for body text; it reaches 3.4:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Gellix and IBM Plex Sans.
- Don't use #1E61F0 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.2s, 0.25s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/amplitude.com/), the free DESIGN.md generator.
