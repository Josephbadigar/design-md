---
version: alpha
name: Typefully
description: "Light interface measured from typefully.com: Inter type with inter-arrows-subset, vivid blue accents, flat surfaces and 6px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#354450"
  on-surface-muted: "#5C6D7A"
  on-surface-subtle: "#8D9AA5"
  overlay: "#C7CDD133"
  overlay-strong: "#8D9AA51A"
  outline: "#E6E8EA"
  outline-variant: "#C7CDD1"
  primary: "#199AF5"
  on-primary: "#FFFFFF"
  secondary: "#FF4D4D"
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
  button-ghost:
    textColor: "{colors.on-surface-muted}"
    rounded: "{rounded.md}"
    padding: 0px 10px
  link:
    textColor: "{colors.primary}"
---

# Typefully Design System

## Overview

Typefully describes itself as: “Create, schedule, and publish social media posts on X (Twitter), LinkedIn, Threads, Bluesky, and more. Grow faster with analytics, tools and automations.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Blue (#199AF5)** as the main accent.

Type is set in **Inter** and **inter-arrows-subset**, with **ui-monospace** for code. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 6px.

Measured from [typefully.com](https://typefully.com/) on October 29, 2026 at 1440×900 and 390×844 from 382 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #7B63F2, #8B5CF6.

- **White (#FFFFFF):** Page background, seen 27 times. Token `background`, CSS `--bg0`.
- **Near Black (#000000):** Primary text and headings, seen 38 times. Token `on-surface`, CSS `--tw-mask-bottom-from-color`.
- **Dark Blue (#354450):** Secondary text, seen 52 times. Token `on-surface-variant`.
- **Blue (#5C6D7A):** Muted text and metadata, seen 25 times. Token `on-surface-muted`, CSS `--c3`.
- **Blue (#8D9AA5):** Subtle text and placeholders, seen 8 times. Token `on-surface-subtle`.
- **Cool Silver 20% (#C7CDD133):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Blue 10% (#8D9AA51A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Mist (#E6E8EA):** Borders and dividers, seen 25 times. Token `outline`.
- **Cool Silver (#C7CDD1):** Secondary dividers, seen 25 times. Token `outline-variant`.
- **Vivid Blue (#199AF5):** Primary buttons and calls to action, seen 13 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Red (#FF4D4D):** Accent, seen 2 times. Token `secondary`.

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
- **button-ghost (“Log in”):** transparent fill, #5C6D7A text, 13.5px/500, 9.6px radius, padding 0px 10px.
- **link:** transparent fill, #199AF5 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 4 levels: #000000, #354450, #5C6D7A, #8D9AA5.
- Do reserve #199AF5 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 18px).
- Do use 6px corners on most elements; larger surfaces also use 9.6px and 12px.
- Don't use #8D9AA5 for body text; it reaches 2.88:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Inter, inter-arrows-subset and ui-monospace.
- Don't use #199AF5 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/typefully.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
