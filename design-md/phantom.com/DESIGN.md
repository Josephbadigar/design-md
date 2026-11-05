---
version: alpha
name: Phantom
description: "Light interface measured from phantom.com: Phantom type, light indigo accents, tonal surfaces and 24px corners."
colors:
  background: "#F5F2FF"
  surface: "#F5F2FF"
  on-surface: "#3C315B"
  on-background: "#3C315B"
  on-surface-strong: "#1C1C1C"
  on-surface-variant: "#86848D"
  surface-container-low: "#F4F2F4"
  surface-container: "#FDFCFE"
  surface-container-high: "#FFFDF8"
  surface-container-highest: "#E9E8EA"
  primary: "#AB9FF2"
  on-primary: "#3C315B"
  secondary: "#193A70"
  tertiary: "#785E19"
typography:
  display-hero:
    fontFamily: Phantom
    fontSize: 96px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.025em
  headline-display:
    fontFamily: Phantom
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.025em
  body-md:
    fontFamily: Phantom
    fontSize: 16px
    fontWeight: 400
  body-lg:
    fontFamily: Phantom
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.2
  headline-display-mobile:
    fontFamily: Phantom
    fontSize: 29px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.025em
  display-hero-mobile:
    fontFamily: Phantom
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.025em
rounded:
  xs: 4px
  sm: 24px
  md: 32px
  lg: 96px
  xl: 100px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 32px
  xl: 48px
  gutter: 10px
  section: 96px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 16px 32px
    height: 52px
  button-outline:
    backgroundColor: "#E2DFFE"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 32px
    height: 89px
  button-ghost:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 16px
    height: 56px
  input-field:
    textColor: "{colors.on-surface}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Phantom Design System

## Overview

Phantom describes itself as: “The self-custodial wallet for trading predictions, perps, and tokens across Solana, Ethereum, Bitcoin, Robinhood, HyperEVM, and more.” The interface is light, built on **Cool Snow (#F5F2FF)** with **Dark Violet (#3C315B)** text, and **Light Indigo (#AB9FF2)** as the main accent.

Type is set in **Phantom**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 24px.

Measured from [phantom.com](https://phantom.com/) on November 4, 2026 at 1440×900 and 390×844 from 219 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Cool Snow (#F5F2FF):** Page background, seen 1 time. Token `background`, CSS `--eofi4s0`.
- **Dark Violet (#3C315B):** Primary text and headings, seen 36 times. Token `on-surface`, CSS `--eofi4so`.
- **Charcoal (#1C1C1C):** Headings and emphasis, seen 6 times. Token `on-surface-strong`, CSS `--eofi4s6`.
- **Cool Gray (#86848D):** Secondary text, seen 4 times. Token `on-surface-variant`, CSS `--eofi4s5`.
- **Mist (#F4F2F4):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--eofi4s1`.
- **Snow (#FDFCFE):** Cards and panels, seen 3 times. Token `surface-container`, CSS `--eofi4se`.
- **Warm Snow (#FFFDF8):** Hover and pressed fills, seen 1 time. Token `surface-container-high`, CSS `--eofi4s8`.
- **Mist (#E9E8EA):** Highest raised elements, seen 2 times. Token `surface-container-highest`.
- **Light Indigo (#AB9FF2):** Primary buttons and calls to action, seen 2 times. Token `primary`, CSS `--eofi4s9`.
- **Dark Violet (#3C315B):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#193A70):** Accent in logos and imagery. Token `secondary`.
- **Dark Amber (#785E19):** Accent in logos and imagery. Token `tertiary`.

## Typography

**Phantom** carries the whole interface. Fallback stack: `Phantom`.

- **display-hero:** Phantom 96px at weight 400, line height 1.1, tracking -0.025em (32px on mobile). Oversized hero statements.
- **headline-display:** Phantom 80px at weight 400, line height 1.1, tracking -0.025em (29px on mobile). Page title (h1).
- **body-md:** Phantom 16px at weight 400. Body text.
- **body-lg:** Phantom 30px at weight 400, line height 1.2. Lead paragraphs.

## Layout

Spacing is mostly on a 4px grid (86% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 10px, lg 32px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Breakpoints:** 639px, 640px, 767px, 768px, 1023px, 1024px, 1279px, 1280px, 1535px, 1536px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgb(226, 223, 254) 0px 0px 4px 0px`

## Shapes

Most elements use 24px corners. Measured radii, most used first:

- **sm (24px):** 48 elements.
- **md (32px):** 28 elements.
- **full (9999px):** 12 elements.
- **lg (96px):** 8 elements.
- **xl (100px):** 8 elements.
- **xs (4px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Download”):** #AB9FF2 fill, #3C315B text, 16px/400, 32px radius, padding 16px 32px.
- **button-outline (“Download Phantom”):** #E2DFFE fill, #3C315B text, 13.3333px/400, 96px radius, padding 32px.
- **button-ghost (“Search”):** #FDFCFE fill, #3C315B text, 13.3333px/400, 32px radius, padding 16px.
- **input-field (“Enter your email”):** transparent fill, #3C315B text, 64px/400, padding 0px.
- **link:** transparent fill, #3C315B text, padding 0px.

## Do's and Don'ts

- Do use #F5F2FF for the page and lift surfaces in small steps: #F4F2F4, #FDFCFE, #FFFDF8, #E9E8EA.
- Do keep text in 3 levels: #3C315B, #1C1C1C, #86848D.
- Do reserve #AB9FF2 for primary actions and key highlights.
- Do set headlines in Phantom with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 10px, 32px).
- Do use 24px corners on most elements; larger surfaces also use 32px, 96px and 100px.
- Don't use #86848D for body text; it reaches 3.34:1 on #F5F2FF. Keep it for large text or metadata.
- Don't introduce new font families beyond Phantom.
- Don't use #AB9FF2 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.4s, 0.3s.

- **Easing:** `cubic-bezier(0.22, 1, 0.36, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/phantom.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
