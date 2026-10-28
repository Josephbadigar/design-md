---
version: alpha
name: Typefully
description: "Dark interface measured from typefully.com: Inter type with inter-arrows-subset, vivid blue accents, tonal surfaces and 6px corners."
colors:
  background: "#111418"
  surface: "#111418"
  on-surface: "#C4C9D4"
  on-background: "#C4C9D4"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#8B94A7"
  on-surface-muted: "#5A6272"
  surface-container-low: "#282B31"
  overlay: "#32363E4D"
  overlay-strong: "#5A62724D"
  outline: "#5A627280"
  outline-variant: "#5A62724D"
  primary: "#199AF5"
  on-primary: "#FFFFFF"
  secondary: "#00E5CC"
  error: "#FF4D4D"
  success: "#34A853"
  warning: "#FBBC05"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 44px
    fontWeight: 700
    lineHeight: 1.14
  headline-lg:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.16
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.45
  body-lg:
    fontFamily: inter-arrows-subset
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: -0.019em
  body-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-md:
    fontFamily: Inter
    fontSize: 15.5px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.3
  code:
    fontFamily: ui-monospace
    fontSize: 14.5px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.14
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 26px
    fontWeight: 700
    lineHeight: 1.16
rounded:
  sm: 6px
  md: 9.6px
  lg: 12px
spacing:
  xs: 3px
  sm: 8px
  md: 12px
  lg: 18px
  xl: 64px
  gutter: 12px
  section: 64px
  container: 1292px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: 0px 10px
    height: 26px
  button-secondary:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    padding: 0px 18px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    rounded: "{rounded.md}"
    padding: 0px 10px
  link:
    textColor: "{colors.primary}"
---

# Typefully Design System

## Overview

Typefully describes itself as: “Create, schedule, and publish social media posts on X (Twitter), LinkedIn, Threads, Bluesky, and more. Grow faster with analytics, tools and automations.” The interface is dark, built on **Cool Charcoal (#111418)** with **Cool Silver (#C4C9D4)** text, and **Vivid Blue (#199AF5)** as the main accent.

Type is set in **Inter** and **inter-arrows-subset**, with **ui-monospace** for code. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 6px.

Measured from [typefully.com](https://typefully.com/) on October 21, 2026 at 1440×900 and 390×844 from 382 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #7B63F2, #8B5CF6.

- **Cool Charcoal (#111418):** Page background, seen 1 time. Token `background`, CSS `--bg0`.
- **Cool Silver (#C4C9D4):** Primary text and headings, seen 52 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 37 times. Token `on-surface-strong`, CSS `--color-typ-verified-badge`.
- **Blue (#8B94A7):** Secondary text, seen 25 times. Token `on-surface-variant`, CSS `--c3`.
- **Blue (#5A6272):** Muted text and metadata, seen 8 times. Token `on-surface-muted`.
- **Cool Graphite (#282B31):** Raised areas one step from the page, seen 25 times. Token `surface-container-low`.
- **Cool Graphite 30% (#32363E4D):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Blue 30% (#5A62724D):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Blue 50% (#5A627280):** Borders and dividers, seen 25 times. Token `outline`.
- **Blue 30% (#5A62724D):** Secondary dividers, seen 25 times. Token `outline-variant`.
- **Vivid Blue (#199AF5):** Primary buttons and calls to action, seen 13 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Teal (#00E5CC):** Accent, seen 2 times. Token `secondary`.
- **Red (#FF4D4D):** Errors and destructive states, seen 2 times. Token `error`.
- **Green (#34A853):** Success and positive states, seen 1 time. Token `success`.
- **Vivid Amber (#FBBC05):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**Inter**, **inter-arrows-subset** and **ui-monospace** (monospace) share the interface. Fallback stack: `Inter, -apple-system, system-ui, Helvetica Neue`. Other loaded fonts: Roboto, GT America.

- **headline-display:** Inter 44px at weight 700, line height 1.14 (28px on mobile). Page title (h1).
- **headline-lg:** Inter 36px at weight 700, line height 1.16 (26px on mobile). Section headings (h2).
- **body-md:** Inter 14px at weight 400, line height 1.45. Body text.
- **body-lg:** inter-arrows-subset 16px at weight 400, line height 1.25, tracking -0.019em. Lead paragraphs.
- **body-sm:** Inter 11px at weight 400, line height 1. Secondary and small text.
- **label-lg:** Inter 16px at weight 600, line height 1.5. Large buttons and tabs.
- **label-md:** Inter 15.5px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Inter 15px at weight 500, line height 1.3. Small labels and badges.
- **code:** ui-monospace 14.5px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing does not follow a strict grid: 54% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 8px, md 12px, lg 18px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1292px.
- **Breakpoints:** 375px, 420px, 520px, 600px, 640px, 680px, 720px, 800px, 840px, 1024px, 1280px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.666339 -0.0653025 -0.156603 / 0.2) 0px 0px 0px 1px, rgba(0, 0, 0, 0.04) 0px 1px 3px -1px, rgba(0, 0, 0, 0.04) 0px 1px 4px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(255, 255, 255, 0.6) 0px 0px 6px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.04) 0px 1px 3px -1px, rgba(0, 0, 0, 0.04) 0px 1px 4px -1px`

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **sm (6px):** 24 elements.
- **md (9.6px):** 8 elements.
- **lg (12px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #199AF5 fill, #FFFFFF text, 13.5px/600, 9.6px radius, padding 0px 10px.
- **button-secondary (“Google”):** #282B31 fill, #C4C9D4 text, 15px/500, 3.22639e+07px radius, padding 0px 18px, border 0.96px solid #5A627280, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.666339 -0.0653025 -0.156603 / 0.2) 0px 0px 0px 1px, rgba(0, 0, 0, 0.04) 0px 1px 3px -1px, rgba(0, 0, 0, 0.04) 0px 1px 4px -1px`.
- **button-ghost (“Log in”):** transparent fill, #8B94A7 text, 13.5px/500, 9.6px radius, padding 0px 10px.
- **link:** transparent fill, #199AF5 text, padding 0px.

## Do's and Don'ts

- Do use #111418 for the page and lift surfaces in small steps: #282B31.
- Do keep text in 4 levels: #C4C9D4, #FFFFFF, #8B94A7, #5A6272.
- Do reserve #199AF5 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 18px).
- Do use 6px corners on most elements; larger surfaces also use 9.6px and 12px.
- Don't use #5A6272 for body text; it reaches 3.0:1 on #111418. Keep it for large text or metadata.
- Don't introduce new font families beyond Inter, inter-arrows-subset and ui-monospace.
- Don't use #199AF5 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/typefully.com/), the free DESIGN.md generator.
