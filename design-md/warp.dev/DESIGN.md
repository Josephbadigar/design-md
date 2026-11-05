---
version: alpha
name: Warp
description: "Light interface measured from warp.dev: sans-serif type with matter, vivid indigo accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FBF9FE"
  surface: "#FBF9FE"
  on-surface: "#1A1522"
  on-background: "#1A1522"
  on-surface-variant: "#5D5964"
  surface-container-low: "#FBFDFD"
  surface-container: "#F7F7F7"
  surface-container-high: "#EEF7FA"
  overlay: "#29233359"
  overlay-strong: "#322C3B8C"
  outline: "#1A15221F"
  outline-variant: "#1A152212"
  primary: "#2A1EFF"
  on-primary: "#FFFFFF"
  inverse-surface: "#211B2B"
  secondary: "#D2B5FF"
typography:
  headline-display:
    fontFamily: azeretSemiMono
    fontSize: 54px
    fontWeight: 400
    lineHeight: 1.18
  headline-lg:
    fontFamily: sans-serif
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1.4
  body-md:
    fontFamily: matter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: matter
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.35
    letterSpacing: -0.02em
  body-sm:
    fontFamily: matter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.55
  label-md:
    fontFamily: Matter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: Matter
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.54
  code:
    fontFamily: azeretSemiMono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1
  headline-display-mobile:
    fontFamily: azeretSemiMono
    fontSize: 34px
    fontWeight: 400
    lineHeight: 1.18
rounded:
  md: 4px
  full: 9999px
spacing:
  xs: 3px
  sm: 6px
  md: 10px
  lg: 32px
  xl: 56px
  gutter: 12px
  section: 56px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 7px 12px
    height: 34px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 6px 16px
    height: 32px
  button-secondary-hover:
    backgroundColor: "{colors.primary}"
  button-outline:
    backgroundColor: "{colors.on-primary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 6px 16px
    height: 32px
  button-outline-hover:
    textColor: "{colors.primary}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 6px 10px
  input-field:
    textColor: "#F0EBF7"
    rounded: 5px
    padding: 0px 10px 0px 32px
  link:
    textColor: "#1A1522B3"
---

# Warp Design System

## Overview

Warp describes itself as: “Build your software factory on Warp: factories as code, any model or harness, with evals, benchmarks, and self-improvement built in.” The interface is light, built on **Snow (#FBF9FE)** with **Cool Charcoal (#1A1522)** text, and **Vivid Indigo (#2A1EFF)** as the main accent.

Type is set in **sans-serif** and **matter**, with **azeretSemiMono** for code. Headlines run large; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [warp.dev](https://www.warp.dev/) on November 4, 2026 at 1440×900 and 390×844 from 461 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Snow (#FBF9FE):** Page background, seen 1 time. Token `background`.
- **Cool Charcoal (#1A1522):** Primary text and headings, seen 26 times. Token `on-surface`.
- **Cool Slate (#5D5964):** Secondary text, seen 9 times. Token `on-surface-variant`.
- **Snow (#FBFDFD):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`.
- **Snow (#F7F7F7):** Cards and panels, seen 1 time. Token `surface-container`.
- **Cool Snow (#EEF7FA):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Cool Graphite 35% (#29233359):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Cool Graphite 55% (#322C3B8C):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Cool Charcoal 12% (#1A15221F):** Borders and dividers, seen 25 times. Token `outline`.
- **Cool Charcoal 7% (#1A152212):** Secondary dividers, seen 7 times. Token `outline-variant`.
- **Vivid Indigo (#2A1EFF):** Primary buttons and calls to action, seen 11 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Cool Charcoal (#211B2B):** High-contrast fills, seen 7 times. Token `inverse-surface`.
- **Light Violet (#D2B5FF):** Accent in text, fills and borders, seen 4 times. Token `secondary`.

## Typography

**azeretSemiMono** (monospace), **sans-serif**, **matter** and **Matter** share the interface. Fallback stack: `azeretSemiMono, azeretSemiMono Fallback, Azeret SemiMono, ui-monospace`. Other loaded fonts: Hack, Agent CLI JetBrains Mono.

- **headline-display:** azeretSemiMono 54px at weight 400, line height 1.18 (34px on mobile). Page title (h1).
- **headline-lg:** sans-serif 21px at weight 400, line height 1.4. Section headings (h2).
- **body-md:** matter 16px at weight 400, line height 1.5. Body text.
- **body-lg:** matter 18px at weight 700, line height 1.35, tracking -0.02em. Lead paragraphs.
- **body-sm:** matter 14px at weight 400, line height 1.55. Secondary and small text.
- **label-md:** Matter 14px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Matter 13px at weight 500, line height 1.54. Small labels and badges.
- **code:** azeretSemiMono 14px at weight 400, line height 1. Code and technical values.

## Layout

Spacing does not follow a strict grid: 47% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 6px, md 10px, lg 32px, xl 56px.
- **Sections:** 56px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 620px, 720px, 900px, 980px, 1100px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FBFDFD → #F7F7F7 → #EEF7FA) and #1A15221F borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 44 elements.
- **md (4px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“factory.yaml”):** #2A1EFF fill, #FFFFFF text, 13px/400, padding 7px 12px.
- **button-secondary (“Get started”):** #1A1522 fill, #FFFFFF text, 13px/500, 4px radius, padding 6px 16px, border 1px solid #1A1522.
- **button-secondary-hover:** background #2A1EFF, text #FFFFFF on hover.
- **button-outline (“download warp terminal”):** #FFFFFF fill, #1A1522 text, 13px/500, 4px radius, padding 6px 16px, border 1px solid #1A15222E.
- **button-outline-hover:** background #FFFFFF, text #2A1EFF on hover.
- **button-ghost (“Products”):** transparent fill, #1A1522 text, 13px/500, padding 6px 10px.
- **input-field (“Search sessions...”):** transparent fill, #F0EBF7 text, 12px/400, 5px radius, padding 0px 10px 0px 32px.
- **link:** transparent fill, #1A1522B3 text, padding 0px.

## Do's and Don'ts

- Do use #FBF9FE for the page and lift surfaces in small steps: #FBFDFD, #F7F7F7, #EEF7FA.
- Do keep text in 2 levels: #1A1522, #5D5964.
- Do reserve #2A1EFF for primary actions and key highlights.
- Do reuse the measured spacing steps (6px, 10px, 32px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond azeretSemiMono, sans-serif, matter and Matter.
- Don't use #2A1EFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.12s, 0.2s. Longer ambient animations run 1.8s.

- **Easing:** `ease`, `ease-in-out`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/warp.dev/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
