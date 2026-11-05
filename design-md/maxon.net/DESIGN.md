---
version: alpha
name: Maxon
description: "Light interface measured from maxon.net: Rajdhani type with Roboto, red accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1C232B"
  on-background: "#1C232B"
  on-surface-strong: "#000000"
  overlay: "#00000080"
  primary: "#D32328"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: Rajdhani
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
  body-md:
    fontFamily: Rajdhani
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Rajdhani
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Roboto
    fontSize: 8px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Rajdhani
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Roboto
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Rajdhani
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: 0.1em
  headline-display-mobile:
    fontFamily: Rajdhani
    fontSize: 35px
    fontWeight: 400
    lineHeight: 1
rounded:
  full: 9999px
spacing:
  sm: 8px
  md: 12px
  lg: 24px
components:
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 12px 24px
    height: 47px
  button-outline-hover:
    backgroundColor: "#8D9196"
    textColor: "{colors.on-primary}"
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 12px 16px
  link:
    textColor: "{colors.on-surface-strong}"
---

# Maxon Design System

## Overview

Maxon describes itself as: “Maxon tools include the award-winning Cinema 4D suite of 3D modeling, simulation and animation technology, the Red Giant lineup of revolutionary editing,…” The interface is light, built on **White (#FFFFFF)** with **Cool Charcoal (#1C232B)** text, and **Red (#D32328)** as the main accent.

Type is set in **Rajdhani** and **Roboto**. Headlines run large; body text is 14px. The surface language is flat. Controls are pill-shaped.

Measured from [maxon.net/en](https://www.maxon.net/en/) (the site sent our reader to its /en version; maxon.net was asked for) on November 4, 2026 at 1440×900 and 390×844 from 152 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 6 roles.

- **White (#FFFFFF):** Page background, seen 19 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Cool Charcoal (#1C232B):** Primary text and headings, seen 8 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 12 times. Token `on-surface-strong`.
- **Near Black 50% (#00000080):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Red (#D32328):** Brand color in the logo, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**Rajdhani** and **Roboto** share the interface. Fallback stack: `Rajdhani, Helvetica, Arial, sans-serif`. Other loaded fonts: Inter.

- **headline-display:** Rajdhani 80px at weight 400, line height 1, uppercase (35px on mobile). Page title (h1).
- **body-md:** Rajdhani 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Rajdhani 16px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** Roboto 8px at weight 400, line height 1.5. Secondary and small text.
- **label-lg:** Rajdhani 20px at weight 400, line height 1.5, uppercase. Large buttons and tabs.
- **label-md:** Roboto 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Rajdhani 14px at weight 600, line height 1.5, tracking 0.1em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (89% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** sm 8px, md 12px, lg 24px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 76 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“LEARN MORE”):** #FFFFFF fill, #000000 text, 14px/600, 9999px radius, padding 12px 24px, border 1px solid #8D9196.
- **button-outline-hover:** background #8D9196, text #FFFFFF on hover.
- **button-ghost (“PRODUCTS”):** transparent fill, #FFFFFF text, 16px/700, padding 12px 16px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #1C232B, #000000.
- Do use #D32328 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px).
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Rajdhani and Roboto.
- Don't use #D32328 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s. Longer ambient animations run 0.7s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/maxon.net/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
