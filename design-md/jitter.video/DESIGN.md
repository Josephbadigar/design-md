---
version: alpha
name: Jitter
description: "Light interface measured from jitter.video: TWK Lausanne type with Inter, light violet accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#19171C"
  on-background: "#19171C"
  on-surface-variant: "#6E6E73"
  surface-container-low: "#F2F1F3"
  surface-container: "#E5E4E7"
  outline: "#FFFFFF1A"
  primary: "#B593FF"
  on-primary: "#19171C"
  secondary: "#7A40ED"
typography:
  headline-display:
    fontFamily: TWK Lausanne
    fontSize: 80px
    fontWeight: 800
    lineHeight: 0.9
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: TWK Lausanne
    fontSize: 72px
    fontWeight: 800
    lineHeight: 0.95
    letterSpacing: -0.044em
  headline-md:
    fontFamily: TWK Lausanne
    fontSize: 48px
    fontWeight: 800
    lineHeight: 1
    letterSpacing: -0.04em
  headline-sm:
    fontFamily: TWK Lausanne
    fontSize: 36px
    fontWeight: 800
    lineHeight: 1
    letterSpacing: -0.044em
  title-lg:
    fontFamily: TWK Lausanne
    fontSize: 21px
    fontWeight: 800
    lineHeight: 0.95
    letterSpacing: -0.02em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.14
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.02em
  label-md:
    fontFamily: TWK Lausanne
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: -0.02em
  headline-display-mobile:
    fontFamily: TWK Lausanne
    fontSize: 64px
    fontWeight: 800
    lineHeight: 0.84
    letterSpacing: -0.037em
  headline-lg-mobile:
    fontFamily: TWK Lausanne
    fontSize: 40px
    fontWeight: 800
    lineHeight: 1
    letterSpacing: -0.04em
rounded:
  sm: 40px
  md: 50px
  full: 9999px
spacing:
  xs: 4px
  sm: 5px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 12px
  section: 60px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: 0px
    height: 60px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px
    height: 52px
  button-ghost:
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  input-field:
    backgroundColor: "#2D2933"
    textColor: "{colors.background}"
    rounded: 0px
    padding: 13px 210px 13px 24px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
    padding: 0px 0px 44px 0px
  link:
    textColor: "{colors.on-surface}"
---

# Jitter Design System

## Overview

Jitter describes itself as: “Jitter is a collaborative motion design tool that lets you create professional animations in minutes, no matter your experience with motion.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#19171C)** text, and **Light Violet (#B593FF)** as the main accent.

Type is set in **TWK Lausanne** and **Inter**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [jitter.video](https://jitter.video/) on November 4, 2026 at 1440×900 and 390×844 from 445 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **White (#FFFFFF):** Page background, seen 10 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Charcoal (#19171C):** Primary text and headings, seen 133 times. Token `on-surface`.
- **Slate (#6E6E73):** Secondary text, seen 48 times. Token `on-surface-variant`.
- **Mist (#F2F1F3):** Raised areas one step from the page, seen 9 times. Token `surface-container-low`.
- **Mist (#E5E4E7):** Cards and panels, seen 8 times. Token `surface-container`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 1 time. Token `outline`.
- **Light Violet (#B593FF):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **Charcoal (#19171C):** Text and icons on primary. Token `on-primary`.
- **Vivid Violet (#7A40ED):** Accent, seen 1 time. Token `secondary`, CSS `--gradient-start-plain`.

## Typography

**TWK Lausanne** and **Inter** share the interface. Fallback stack: `TWK Lausanne, sans-serif`.

- **headline-display:** TWK Lausanne 80px at weight 800, line height 0.9, tracking -0.03em (64px on mobile). Page title (h1).
- **headline-lg:** TWK Lausanne 72px at weight 800, line height 0.95, tracking -0.044em (40px on mobile). Section headings (h2).
- **headline-md:** TWK Lausanne 48px at weight 800, line height 1, tracking -0.04em. Sub-section headings.
- **headline-sm:** TWK Lausanne 36px at weight 800, line height 1, tracking -0.044em. Card and feature titles.
- **title-lg:** TWK Lausanne 21px at weight 800, line height 0.95, tracking -0.02em. Small titles.
- **body-md:** Inter 14px at weight 400, line height 1.14. Body text.
- **body-lg:** Inter 16px at weight 400, line height 1.5, tracking -0.02em. Lead paragraphs.
- **label-md:** TWK Lausanne 18px at weight 600, line height 1.5, tracking -0.02em. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 66% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 5px, md 12px, lg 20px, xl 40px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(25, 23, 28, 0) 0px 237px 66px 0px, rgba(25, 23, 28, 0.01) 0px 152px 61px 0px, rgba(25, 23, 28, 0.05) 0px 85px 51px 0px, rgba(25, 23, 28, 0.09) 0px 38px 38px 0px, rgba(25, 23, 28, 0.1) 0px 9px 21px 0px`
- `rgb(255, 255, 255) 1px 0px 0px 0px, rgb(255, 255, 255) -1px 0px 0px 0px`
- `rgb(25, 23, 28) 1px 0px 0px 0px, rgb(25, 23, 28) -1px 0px 0px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (40px):** 36 elements.
- **full (9999px):** 32 elements.
- **md (50px):** 10 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try Jitter for free”):** #B593FF fill, #19171C text, 20px/600, 50px radius, padding 0px.
- **button-secondary (“Sign up”):** #19171C fill, #FFFFFF text, 18px/600, 50px radius, padding 0px.
- **button-ghost (“Sign up”):** transparent fill, #FFFFFF text, 18px/600, padding 0px.
- **input-field (“Your email”):** #2D2933 fill, #FFFFFF text, 17px/600, 0px 50px 50px 0px radius, padding 13px 210px 13px 24px, border 1px solid #FFFFFF1A.
- **card:** #F2F1F3 fill, #19171C text, 12px/400, 40px radius, padding 0px 0px 44px 0px.
- **link:** transparent fill, #19171C text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F2F1F3, #E5E4E7.
- Do keep text in 2 levels: #19171C, #6E6E73.
- Do reserve #B593FF for primary actions and key highlights.
- Do set headlines in TWK Lausanne with tight tracking (-0.03em).
- Do reuse the measured spacing steps (5px, 12px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 40px corners.
- Don't introduce new font families beyond TWK Lausanne and Inter.
- Don't use #B593FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.35s.

## Motion

Interface transitions are quick: 0.3s, 0.35s, 0.2s. Longer ambient animations run 0.8s, 1.2s.

- **Easing:** `cubic-bezier(0.25, 0.46, 0.45, 0.94)`, `cubic-bezier(0.33, 1.42, 0.05, 0.96)`, `linear(0 0%, 0.255 1%, 0.4449 2%, 0.6018 3%, 0.7355 4%, 0.8513 5%, 0.9525 6%, 1.0413 7%, 1.1195 8%, 1.1881 9%, 1.2484 10%, 1.3011 11%, 1.3468 12%, 1.3862 13%, 1.4198 14%, 1.4479 15%, 1.4709 16%, 1.4892 17%, 1.503 18%, 1.5126 19%, 1.5182 20%, 1.52 21%, 1.5189 22%, 1.5156 23%, 1.5101 24%, 1.5025 25%, 1.4929 26%, 1.4817 27%, 1.469 28%, 1.4552 29%, 1.4406 30%, 1.4254 31%, 1.4099 32%, 1.3943 33%, 1.3787 34%, 1.3633 35%, 1.3481 36%, 1.3333 37%, 1.3188 38%, 1.3048 39%, 1.2912 40%, 1.278 41%, 1.2653 42%, 1.253 43%, 1.2412 44%, 1.2298 45%, 1.2188 46%, 1.2083 47%, 1.1981 48%, 1.1883 49%, 1.1789 50%, 1.1698 51%, 1.1611 52%, 1.1528 53%, 1.1447 54%, 1.137 55%, 1.1296 56%, 1.1225 57%, 1.1156 58%, 1.1091 59%, 1.1028 60%, 1.0967 61%, 1.0909 62%, 1.0854 63%, 1.0801 64%, 1.075 65%, 1.0701 66%, 1.0654 67%, 1.061 68%, 1.0567 69%, 1.0526 70%, 1.0488 71%, 1.0451 72%, 1.0415 73%, 1.0382 74%, 1.035 75%, 1.032 76%, 1.0292 77%, 1.0265 78%, 1.0239 79%, 1.0215 80%, 1.0193 81%, 1.0172 82%, 1.0152 83%, 1.0134 84%, 1.0117 85%, 1.0101 86%, 1.0086 87%, 1.0073 88%, 1.0061 89%, 1.005 90%, 1.004 91%, 1.0032 92%, 1.0024 93%, 1.0018 94%, 1.0012 95%, 1.0008 96%, 1.0004 97%, 1.0002 98%, 1 99%, 1 100%)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/jitter.video/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
