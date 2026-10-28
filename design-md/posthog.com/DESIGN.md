---
version: alpha
name: PostHog
description: "Light interface measured from posthog.com: RoundHog type, vivid orange accents, tonal surfaces and 4px corners."
colors:
  background: "#EEEFE9"
  surface: "#EEEFE9"
  on-surface: "#374151"
  on-background: "#374151"
  on-surface-strong: "#111111"
  on-surface-variant: "#111827"
  on-surface-muted: "#23251D"
  surface-container-low: "#FFFFFF"
  overlay: "#2F80FA1A"
  overlay-strong: "#FFFFFF40"
  outline: "#BFC1B7"
  outline-variant: "#D2D3CC"
  primary: "#F54E00"
  on-primary: "#FFFFFF"
  secondary: "#EB9D2A"
  tertiary: "#CD8407"
  warning: "#B17816"
typography:
  headline-display:
    fontFamily: RoundHog
    fontSize: 36px
    fontWeight: 800
    lineHeight: 1.11
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: RoundHog
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.33
    letterSpacing: -0.025em
  body-md:
    fontFamily: RoundHog
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.78
  body-sm:
    fontFamily: RoundHog
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: RoundHog
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-lg:
    fontFamily: RoundHog
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: RoundHog
    fontSize: 15px
    fontWeight: 600
    lineHeight: 1.78
  label-sm:
    fontFamily: RoundHog
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: RoundHog
    fontSize: 30px
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: -0.025em
rounded:
  sm: 2px
  md: 4px
  lg: 6px
  xl: 8px
  full: 9999px
spacing:
  xs: 2px
  sm: 6px
  md: 12px
  lg: 32px
  xl: 56px
  gutter: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 10px 12px
    height: 40px
  button-primary-hover:
    textColor: "#65675E"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 0px
    height: 47px
  button-tertiary:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 0px
    height: 47px
  button-ghost:
    textColor: "{colors.on-surface-muted}"
    rounded: "{rounded.md}"
    padding: 2px 8px
  link:
    textColor: "{colors.on-surface}"
---

# PostHog Design System

## Overview

PostHog describes itself as: “PostHog automatically diagnoses problems, fixes bugs, and generates pull requests – all without you having to prompt it.” The interface is light, built on **Warm Mist (#EEEFE9)** with **Dark Blue (#374151)** text, and **Vivid Orange (#F54E00)** as the main accent.

Type is set in **RoundHog**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [posthog.com](https://posthog.com/) on October 21, 2026 at 1440×900 and 390×844 from 396 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **Warm Mist (#EEEFE9):** Page background, seen 1 time. Token `background`.
- **Dark Blue (#374151):** Primary text and headings, seen 48 times. Token `on-surface`.
- **Charcoal (#111111):** Headings and emphasis, seen 12 times. Token `on-surface-strong`.
- **Deep Blue (#111827):** Secondary text, seen 10 times. Token `on-surface-variant`.
- **Charcoal (#23251D):** Muted text and metadata, seen 6 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`, CSS `--tw-ring-offset-color`.
- **Vivid Blue 10% (#2F80FA1A):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White 25% (#FFFFFF40):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Silver (#BFC1B7):** Borders and dividers, seen 3 times. Token `outline`.
- **Warm Silver (#D2D3CC):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Orange (#F54E00):** Brand color on large areas, seen 1 time. Token `primary`, CSS `--swiper-pagination-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Orange (#EB9D2A):** Secondary buttons, seen 44 times. Token `secondary`.
- **Orange (#CD8407):** Secondary buttons, seen 29 times. Token `tertiary`.
- **Orange (#B17816):** Warnings and highlights, seen 8 times. Token `warning`.

## Typography

**RoundHog** carries the whole interface. Fallback stack: `RoundHog, sans-serif`. Other loaded fonts: Source Code Pro.

- **headline-display:** RoundHog 36px at weight 800, line height 1.11, tracking -0.025em (30px on mobile). Page title (h1).
- **headline-lg:** RoundHog 30px at weight 700, line height 1.33, tracking -0.025em. Section headings (h2).
- **body-md:** RoundHog 18px at weight 500, line height 1.78. Body text.
- **body-sm:** RoundHog 16px at weight 400, line height 1.5. Secondary and small text.
- **caption:** RoundHog 14px at weight 400, line height 1.43. Captions and fine print.
- **label-lg:** RoundHog 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** RoundHog 15px at weight 600, line height 1.78. Buttons, navigation and labels.
- **label-sm:** RoundHog 14px at weight 600, line height 1.43. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 43% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 12px, lg 32px, xl 56px.
- **Gaps:** 32px is the most common gap in flex and grid layouts.
- **Breakpoints:** 1px, 425px, 482px, 520px, 600px, 640px, 767px, 768px, 800px, 900px, 1024px, 1160px, 1280px, 1536px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.25) 0px 25px 50px -12px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(14, 18, 22, 0.35) 0px 10px 38px -10px, rgba(14, 18, 22, 0.2) 0px 10px 20px -15px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 124 elements.
- **sm (2px):** 52 elements.
- **lg (6px):** 34 elements.
- **xl (8px):** 16 elements.
- **full (9999px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Give agents product context”):** #F54E00 fill, #FFFFFF text, 14px/600, 6px 6px 0px 0px radius, padding 10px 12px.
- **button-primary-hover:** background #00000000, text #65675E on hover.
- **button-secondary (“Install with AI”):** #EB9D2A fill, #111111 text, 18px/500, 8px radius, padding 0px, border 1px solid #B17816.
- **button-tertiary (“Get started”):** #CD8407 fill, #111111 text, 18px/500, 8px radius, padding 0px, border 1px solid #B17816.
- **button-ghost (“Products”):** transparent fill, #23251D text, 13px/500, 4px radius, padding 2px 8px.
- **link:** transparent fill, #374151 text, padding 0px.

## Do's and Don'ts

- Do use #EEEFE9 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 4 levels: #374151, #111111, #111827, #23251D.
- Do use #F54E00 as the brand accent: header, logo and key highlights.
- Do set headlines in RoundHog with tight tracking (-0.025em).
- Do reuse the measured spacing steps (6px, 12px, 32px).
- Do use 4px corners on most elements; larger surfaces also use 2px, 6px and 8px.
- Don't introduce new font families beyond RoundHog.
- Don't use #F54E00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`, `cubic-bezier(0.16, 1, 0.3, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/posthog.com/), the free DESIGN.md generator.
