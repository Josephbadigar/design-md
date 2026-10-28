---
version: alpha
name: Neon
description: "Dark interface measured from neon.tech: Inter type, teal accents, tonal surfaces and 4px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#C9CBCF"
  on-surface-muted: "#AFB1B6"
  on-surface-subtle: "#797D86"
  surface-container-low: "#111315"
  surface-container: "#151617"
  surface-container-high: "#18191B"
  surface-container-highest: "#0D221A"
  overlay: "#FFFFFF05"
  outline: "#494B50"
  outline-variant: "#303236"
  primary: "#34D59A"
  on-primary: "#000000"
  inverse-surface: "#E4E5E7"
  error: "#FF3621"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Inter
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.04em
  headline-md:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.04em
  headline-sm:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.02em
  body-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.02em
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.02em
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  code:
    fontFamily: GeistMono
    fontSize: 52px
    fontWeight: 400
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.04em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.04em
  headline-sm-mobile:
    fontFamily: Inter
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.02em
rounded:
  md: 4px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "#1A1A1A"
    typography: "{typography.label-md}"
    padding: 0px 28px
    height: 44px
  button-primary-hover:
    backgroundColor: "{colors.on-surface-variant}"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    padding: 0px 18px
    height: 36px
  button-secondary-hover:
    backgroundColor: "{colors.on-surface-variant}"
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    padding: 0px 18px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 14px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Neon Design System

## Overview

Neon describes itself as: “The backend for apps and agents. Build with Lakebase Postgres, Auth, Functions, Storage, and an AI Gateway: instant, branchable, serverless.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Teal (#34D59A)** as the main accent.

Type is set in **Inter**, with **GeistMono** for code. Headlines run large with tight negative tracking; body text is 15px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [neon.tech](https://neon.com/) on October 21, 2026 at 1440×900 and 390×844 from 411 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles.

- **Near Black (#000000):** Page background, seen 8 times. Token `background`, CSS `--error-tooltip-bg`.
- **White (#FFFFFF):** Primary text and headings, seen 28 times. Token `on-surface`, CSS `--shiki-token-embed`.
- **Cool Silver (#C9CBCF):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Cool Gray (#AFB1B6):** Muted text and metadata, seen 29 times. Token `on-surface-muted`.
- **Cool Slate (#797D86):** Subtle text and placeholders, seen 10 times. Token `on-surface-subtle`, CSS `--shiki-token-comment`.
- **Charcoal (#111315):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **Charcoal (#151617):** Cards and panels, seen 1 time. Token `surface-container`.
- **Charcoal (#18191B):** Hover and pressed fills, seen 4 times. Token `surface-container-high`.
- **Deep Teal (#0D221A):** Highest raised elements, seen 2 times. Token `surface-container-highest`.
- **White 2% (#FFFFFF05):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Cool Graphite (#494B50):** Borders and dividers, seen 5 times. Token `outline`.
- **Cool Graphite (#303236):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Teal (#34D59A):** Brand color in the logo, seen 2 times. Token `primary`, CSS `--shiki-token-keyword`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Mist (#E4E5E7):** High-contrast fills, seen 15 times. Token `inverse-surface`.
- **Vivid Red (#FF3621):** Errors and destructive states, seen 4 times. Token `error`.

## Typography

**Inter** and **GeistMono** (monospace) share the interface. Fallback stack: `Inter, Inter Fallback, ui-sans-serif, system-ui`. Other loaded fonts: Inter Fallback.

- **headline-display:** Inter 56px at weight 400, line height 1.13, tracking -0.04em (32px on mobile). Page title (h1).
- **headline-lg:** Inter 44px at weight 400, line height 1.13, tracking -0.04em (28px on mobile). Section headings (h2).
- **headline-md:** Inter 36px at weight 400, line height 1.13, tracking -0.04em. Sub-section headings.
- **headline-sm:** Inter 28px at weight 400, line height 1.25, tracking -0.02em (22px on mobile). Card and feature titles.
- **body-md:** Inter 15px at weight 400, line height 1, tracking -0.02em. Body text.
- **body-lg:** Inter 18px at weight 400, line height 1.25, tracking -0.02em. Lead paragraphs.
- **body-sm:** Inter 13px at weight 400, line height 1.25, tracking -0.02em. Secondary and small text.
- **label-md:** Inter 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1, tracking -0.02em. Small labels and badges.
- **code:** GeistMono 52px at weight 400, line height 1. Code and technical values.

## Layout

Spacing does not follow a strict grid: 66% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 16px, lg 32px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 640px, 1024px, 1280px, 1366px, 1407px, 1919px, 1921px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#111315 → #151617 → #18191B → #0D221A) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, lab(100 -0.0000298023 0.0000119209 / 0.05) 0px 0px 0px 1px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 140 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #FFFFFF fill, #1A1A1A text, 16px/500, 3.35544e+07px radius, padding 0px 28px.
- **button-primary-hover:** background #C9CBCF, text #1A1A1A on hover.
- **button-secondary (“Sign up”):** #FFFFFF fill, #000000 text, 14px/500, 3.35544e+07px radius, padding 0px 18px.
- **button-secondary-hover:** background #C9CBCF, text #000000 on hover.
- **button-outline (“Log in”):** transparent fill, #FFFFFF text, 14px/500, 3.35544e+07px radius, padding 0px 18px, border 1px solid #61646B.
- **button-ghost (“Product”):** transparent fill, #FFFFFF text, 15px/400, 4px radius, padding 0px 14px.
- **link:** transparent fill, #AFB1B6 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #111315, #151617, #18191B, #0D221A.
- Do keep text in 4 levels: #FFFFFF, #C9CBCF, #AFB1B6, #797D86.
- Do use #34D59A as the brand accent: header, logo and key highlights.
- Do set headlines in Inter with tight tracking (-0.04em).
- Do reuse the measured spacing steps (6px, 16px, 32px).
- Do use 4px corners on most elements.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Inter and GeistMono.
- Don't use #34D59A for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/neon.tech/), the free DESIGN.md generator.
