---
version: alpha
name: Superhuman
description: "Light interface measured from superhuman.com: Super Sans VF type, violet accents, tonal surfaces and 12px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#292827"
  on-background: "#292827"
  on-surface-variant: "#666665"
  surface-container-low: "#F7F5F2"
  surface-container: "#F2F0EB"
  surface-container-high: "#E8E0FF"
  surface-container-highest: "#DEDBD5"
  outline: "#73716D33"
  outline-variant: "#FCFAF714"
  primary: "#714CB6"
  on-primary: "#FFFFFF"
  secondary: "#D4C7FF"
typography:
  headline-display:
    fontFamily: Super Sans VF
    fontSize: 49px
    fontWeight: 460
    lineHeight: 1.2
    letterSpacing: -0.027em
  headline-lg:
    fontFamily: Super Sans VF
    fontSize: 25px
    fontWeight: 460
    lineHeight: 1.2
    letterSpacing: -0.028em
  body-md:
    fontFamily: Super Sans VF
    fontSize: 18px
    fontWeight: 540
    lineHeight: 1.5
    letterSpacing: -0.008em
  body-lg:
    fontFamily: Super Sans VF
    fontSize: 19px
    fontWeight: 700
    lineHeight: 1.5
  label-md:
    fontFamily: Super Sans VF
    fontSize: 16px
    fontWeight: 460
    lineHeight: 1.5
  label-sm:
    fontFamily: Super Sans VF
    fontSize: 14px
    fontWeight: 540
    lineHeight: 1.2
  headline-display-mobile:
    fontFamily: Super Sans VF
    fontSize: 32px
    fontWeight: 460
    lineHeight: 1.2
    letterSpacing: -0.028em
  headline-lg-mobile:
    fontFamily: Super Sans VF
    fontSize: 20px
    fontWeight: 460
    lineHeight: 1.2
    letterSpacing: -0.028em
rounded:
  sm: 8px
  md: 12px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 6px 20px
    height: 52px
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 6px 16px
    height: 36px
  button-secondary-hover:
    backgroundColor: "#BEA1F5"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px 8px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 32px
  link:
    textColor: "{colors.on-primary}"
---

# Superhuman Design System

## Overview

Superhuman describes itself as: “Superhuman is the AI productivity suite that gives you superpowers everywhere you work. So you can be more creative, strategic, and impactful.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#292827)** text, and **Violet (#714CB6)** as the main accent.

Type is set in **Super Sans VF**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 12px.

Measured from [superhuman.com](https://superhuman.com/) on October 29, 2026 at 1440×900 and 390×844 from 286 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`.
- **Graphite (#292827):** Primary text and headings, seen 30 times. Token `on-surface`, CSS `--neutral-90`.
- **Slate (#666665):** Secondary text, seen 18 times. Token `on-surface-variant`.
- **Snow (#F7F5F2):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`.
- **Warm Mist (#F2F0EB):** Cards and panels, seen 3 times. Token `surface-container`, CSS `--neutral-10`.
- **Pale Violet (#E8E0FF):** Hover and pressed fills, seen 2 times. Token `surface-container-high`.
- **Warm Silver (#DEDBD5):** Highest raised elements, seen 1 time. Token `surface-container-highest`.
- **Warm Slate 20% (#73716D33):** Borders and dividers, seen 8 times. Token `outline`.
- **Snow 8% (#FCFAF714):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Violet (#714CB6):** Primary buttons and calls to action, seen 8 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Pale Violet (#D4C7FF):** Secondary buttons, seen 5 times. Token `secondary`.

## Typography

**Super Sans VF** carries the whole interface. Fallback stack: `Super Sans VF, system-ui, -apple-system, BlinkMacSystemFont`.

- **headline-display:** Super Sans VF 49px at weight 460, line height 1.2, tracking -0.027em (32px on mobile). Page title (h1).
- **headline-lg:** Super Sans VF 25px at weight 460, line height 1.2, tracking -0.028em (20px on mobile). Section headings (h2).
- **body-md:** Super Sans VF 18px at weight 540, line height 1.5, tracking -0.008em. Body text.
- **body-lg:** Super Sans VF 19px at weight 700, line height 1.5. Lead paragraphs.
- **label-md:** Super Sans VF 16px at weight 460, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Super Sans VF 14px at weight 540, line height 1.2. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (89% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 16px, lg 32px, xl 40px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `color(srgb 0.278431 0.270588 0.262745 / 0.04) 0px 0px 0px 1px, color(srgb 0.278431 0.270588 0.262745 / 0.06) 0px 4px 8px -2px, color(srgb 0.278431 0.270588 0.262745 / 0.04) 0px 2px 4px 0px, color(srgb 0.278431 0.270588 0.262745 / 0.04) 0px 1px 2px 0px, color(srgb 0.870588 0.858824 0.835294 / 0.2) 0px 0px 0px 1px`

Hairline rings and inset highlights also appear: `color(srgb 0.45098 0.443137 0.427451 / 0.2) 0px 0px 0px 1px inset`.

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **md (12px):** 60 elements.
- **sm (8px):** 32 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try Go”):** #714CB6 fill, #FFFFFF text, 16px/600, 12px radius, padding 6px 20px.
- **button-secondary (“Get Mail”):** #D4C7FF fill, #292827 text, 14px/600, 8px radius, padding 6px 16px.
- **button-secondary-hover:** background #BEA1F5, text #292827 on hover.
- **button-ghost (“Products”):** transparent fill, #292827 text, 16px/460, padding 0px 8px.
- **card:** #F2F0EB fill, #292827 text, 16px/460, 12px radius, padding 32px, shadow `color(srgb 0.278431 0.270588 0.262745 / 0.04) 0px 0px 0px 1px, color(srgb 0.278431 0.270588 0.262745 / 0.06) 0px 4px 8px -2px, color(srgb 0.278431 0.270588 0.262745 / 0.04) 0px 2px 4px 0px, color(srgb 0.278431 0.270588 0.262745 / 0.04) 0px 1px 2px 0px, color(srgb 0.870588 0.858824 0.835294 / 0.2) 0px 0px 0px 1px`.
- **link:** transparent fill, #FFFFFFCC text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F7F5F2, #F2F0EB, #E8E0FF, #DEDBD5.
- Do keep text in 2 levels: #292827, #666665.
- Do reserve #714CB6 for primary actions and key highlights.
- Do set headlines in Super Sans VF with tight tracking (-0.027em).
- Do reuse the measured spacing steps (6px, 16px, 32px).
- Do use 12px corners on most elements; larger surfaces also use 8px.
- Don't introduce new font families beyond Super Sans VF.
- Don't use #714CB6 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.5s.

- **Easing:** `ease`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/superhuman.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
