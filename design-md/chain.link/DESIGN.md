---
version: alpha
name: Chainlink
description: "Dark interface measured from chain.link: TASA Orbiter VF type with Inter, vivid blue accents, flat surfaces and 2px corners."
colors:
  background: "#0E1119"
  surface: "#0E1119"
  on-surface: "#A6AEBC"
  on-background: "#A6AEBC"
  on-surface-strong: "#F5F7FA"
  overlay: "#16254121"
  overlay-strong: "#D9E2F221"
  outline: "#16254159"
  outline-variant: "#D9E2F240"
  primary: "#0D5DFF"
  on-primary: "#FFFFFF"
  secondary: "#0847F7"
  tertiary: "#2E7BFF"
typography:
  headline-display:
    fontFamily: TASA Orbiter VF
    fontSize: 64px
    fontWeight: 420
    lineHeight: 1
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: TASA Orbiter VF
    fontSize: 56px
    fontWeight: 430
    lineHeight: 1
    letterSpacing: -0.01em
  headline-md:
    fontFamily: TASA Orbiter VF
    fontSize: 40px
    fontWeight: 475
    lineHeight: 1.1
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: TASA Orbiter VF
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.13
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 450
    lineHeight: 1.5
    letterSpacing: -0.015em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 550
    lineHeight: 1.3
    letterSpacing: -0.025em
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 450
    lineHeight: 1
    letterSpacing: -0.01em
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 450
    lineHeight: 1
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.015em
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.14
  code:
    fontFamily: DM Mono
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: 0.05em
  headline-display-mobile:
    fontFamily: TASA Orbiter VF
    fontSize: 44px
    fontWeight: 462.5
    lineHeight: 1
    letterSpacing: -0.01em
  headline-md-mobile:
    fontFamily: TASA Orbiter VF
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.01em
rounded:
  md: 2px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 57.04px
  gutter: 8px
  section: 57.04px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 16px 24px
    height: 50px
  button-primary-hover:
    backgroundColor: "{colors.secondary}"
  button-outline:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 16px 24px
    height: 50px
  button-ghost:
    textColor: "{colors.background}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 42px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 12px 16px
  card:
    backgroundColor: "{colors.on-primary}"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 24px
  link:
    textColor: "{colors.on-surface}"
---

# Chainlink Design System

## Overview

Chainlink describes itself as: “Chainlink is the industry-standard oracle platform powering the majority of decentralized finance and bringing the capital markets onchain.” The interface is dark, built on **Cool Charcoal (#0E1119)** with **Blue (#A6AEBC)** text, and **Vivid Blue (#0D5DFF)** as the main accent.

Type is set in **TASA Orbiter VF** and **Inter**, with **DM Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 2px.

Measured from [chain.link](https://chain.link/) on November 4, 2026 at 1440×900 and 390×844 from 346 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Cool Charcoal (#0E1119):** Page background, seen 14 times. Token `background`.
- **Blue (#A6AEBC):** Primary text and headings. Token `on-surface`.
- **Snow (#F5F7FA):** Headings and emphasis, seen 15 times. Token `on-surface-strong`.
- **Deep Blue 13% (#16254121):** Translucent fill for cards and controls, seen 8 times. Token `overlay`.
- **Pale Blue 13% (#D9E2F221):** Stronger translucent fill, seen 5 times. Token `overlay-strong`.
- **Deep Blue 35% (#16254159):** Borders and dividers, seen 1 time. Token `outline`.
- **Pale Blue 25% (#D9E2F240):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Blue (#0D5DFF):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0847F7):** Accent (CSS variable), seen 19 times. Token `secondary`, CSS `--_backbone--theme---button-primary--background`.
- **Vivid Blue (#2E7BFF):** Accent in text, fills and borders, seen 35 times. Token `tertiary`.

## Typography

**TASA Orbiter VF**, **Inter** and **DM Mono** (monospace) share the interface. Fallback stack: `TASA Orbiter VF, sans-serif`. Other loaded fonts: argent-pixel-cf.

- **headline-display:** TASA Orbiter VF 64px at weight 420, line height 1, tracking -0.01em (44px on mobile). Page title (h1).
- **headline-lg:** TASA Orbiter VF 56px at weight 430, line height 1, tracking -0.01em. Section headings (h2).
- **headline-md:** TASA Orbiter VF 40px at weight 475, line height 1.1, tracking -0.01em (32px on mobile). Sub-section headings.
- **headline-sm:** TASA Orbiter VF 32px at weight 500, line height 1.13, tracking -0.01em. Card and feature titles.
- **body-md:** Inter 16px at weight 450, line height 1.5, tracking -0.015em. Body text.
- **body-lg:** Inter 18px at weight 550, line height 1.3, tracking -0.025em. Lead paragraphs.
- **body-sm:** Inter 14px at weight 450, line height 1, tracking -0.01em. Secondary and small text.
- **caption:** Inter 12px at weight 450, line height 1. Captions and fine print.
- **label-md:** Inter 16px at weight 500, line height 1.5, tracking -0.015em. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 600, line height 1.14. Small labels and badges.
- **code:** DM Mono 12px at weight 500, line height 1.25, tracking 0.05em. Code and technical values.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 57.04px.
- **Sections:** 57.04px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 767px, 768px, 991px, 1500px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgb(8, 71, 247) 0px 2px 0px 0px inset`

## Shapes

Most elements use 2px corners. Measured radii, most used first:

- **md (2px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Watch now”):** #0D5DFF fill, #FFFFFF text, 14px/600, 2px radius, padding 16px 24px.
- **button-primary-hover:** background #0847F7, text #FFFFFF on hover.
- **button-outline (“Learn more”):** transparent fill, #F5F7FA text, 14px/600, 2px radius, padding 16px 24px, border 1px solid #D9E2F266.
- **button-ghost (“Start building”):** transparent fill, #0E1119 text, 14px/600, 2px radius, padding 12px 16px, border 1px solid #16254159.
- **input-field (“Email address”):** #0E1119 fill, #F5F7FA text, 14px/400, 2px 0px 0px 2px radius, padding 12px 16px, border 1px solid #D9E2F240.
- **card:** #FFFFFF fill, #0E1119 text, 16px/450, padding 24px.
- **link:** transparent fill, #D9E2F2BF text, padding 0px.

## Do's and Don'ts

- Do use #0E1119 for the page.
- Do keep text in 2 levels: #A6AEBC, #F5F7FA.
- Do reserve #0D5DFF for primary actions and key highlights.
- Do set headlines in TASA Orbiter VF with tight tracking (-0.01em).
- Do keep spacing on the 4px grid.
- Do use 2px corners on most elements.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond TASA Orbiter VF, Inter and DM Mono.
- Don't use #0D5DFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s.

- **Easing:** `cubic-bezier(0.19, 1, 0.22, 1)`, `cubic-bezier(0.25, 0.46, 0.45, 0.94)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/chain.link/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
