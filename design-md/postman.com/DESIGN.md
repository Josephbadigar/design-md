---
version: alpha
name: Postman
description: "Light interface measured from postman.com: gtStandard type with system-ui, vivid orange accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FF6C37"
  surface: "#FF6C37"
  on-surface: "#212121"
  on-background: "#212121"
  on-surface-variant: "#FFFFFF"
  on-surface-muted: "#FFF0DE"
  overlay: "#FFE0C424"
  overlay-strong: "#120A0666"
  outline: "#FFE0C424"
  outline-variant: "#FFE0C40F"
  primary: "#FF6C37"
  on-primary: "#000000"
  inverse-surface: "#0E0704"
  secondary: "#E0531F"
  tertiary: "#FF8A5C"
  warning: "#FFA90A"
typography:
  headline-display:
    fontFamily: gtStandard
    fontSize: 63.5px
    fontWeight: 500
    lineHeight: 1.02
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: gtStandard
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.22
    letterSpacing: -0.02em
  headline-md:
    fontFamily: system-ui
    fontSize: 21px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: -0.008em
  headline-sm:
    fontFamily: gtStandard
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.01em
  body-md:
    fontFamily: inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: -0.01em
  body-lg:
    fontFamily: inter
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: -0.008em
  body-sm:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.7
    letterSpacing: -0.011em
  caption:
    fontFamily: inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.63
    letterSpacing: -0.013em
  label-lg:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: -0.01em
  label-md:
    fontFamily: inter
    fontSize: 15px
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: -0.011em
  label-sm:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.63
    letterSpacing: -0.011em
  code:
    fontFamily: ibmPlexMono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.63
    letterSpacing: -0.013em
  headline-display-mobile:
    fontFamily: gtStandard
    fontSize: 58px
    fontWeight: 500
    lineHeight: 1.02
    letterSpacing: -0.02em
rounded:
  sm: 5px
  md: 8px
  lg: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 5px
  md: 10px
  lg: 22px
  xl: 40px
  gutter: 10px
  section: 96px
  margin: 24px
  container: 760px
components:
  button-primary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 4px 12px
    height: 33px
  button-primary-hover:
    backgroundColor: "{colors.background}"
  button-secondary:
    backgroundColor: "#0A0503"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 11px
    height: 44px
  button-tertiary:
    backgroundColor: "#120A06B8"
    textColor: "#FFE0C4D9"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 10px 14px 10px 18px
    height: 38px
  button-ghost:
    textColor: "#8A8178"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 0px 15px
  card:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Postman Design System

## Overview

Postman describes itself as: “Go faster from development to production with higher accuracy and fewer tokens.” The interface is light, built on **Vivid Orange (#FF6C37)** with **Charcoal (#212121)** text, and **Vivid Orange (#FF6C37)** as the main accent.

Type is set in **gtStandard** and **system-ui**, with **ibmPlexMono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [postman.com](https://www.postman.com/) on October 21, 2026 at 1440×900 and 390×844 from 391 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #230C15, #300F18, #FF6C379E.

- **Vivid Orange (#FF6C37):** Page background. Token `background`, CSS `--orange-50`.
- **Charcoal (#212121):** Primary text and headings. Token `on-surface`.
- **White (#FFFFFF):** Secondary text, seen 51 times. Token `on-surface-variant`, CSS `--color-white`.
- **Pale Orange (#FFF0DE):** Muted text and metadata, seen 24 times. Token `on-surface-muted`.
- **Pale Orange 14% (#FFE0C424):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Warm Charcoal 40% (#120A0666):** Stronger translucent fill, seen 4 times. Token `overlay-strong`.
- **Pale Orange 14% (#FFE0C424):** Borders and dividers, seen 8 times. Token `outline`.
- **Pale Orange 6% (#FFE0C40F):** Secondary dividers, seen 6 times. Token `outline-variant`.
- **Vivid Orange (#FF6C37):** Brand color on large areas, seen 1 time. Token `primary`, CSS `--orange-50`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Near Black (#0E0704):** High-contrast fills, seen 8 times. Token `inverse-surface`.
- **Orange (#E0531F):** Secondary buttons, seen 36 times. Token `secondary`.
- **Orange (#FF8A5C):** Most used accent color, seen 6 times. Token `tertiary`.
- **Vivid Orange (#FFA90A):** Warnings and highlights, seen 3 times. Token `warning`.

## Typography

**gtStandard**, **system-ui**, **inter** and **ibmPlexMono** (monospace) share the interface. Fallback stack: `gtStandard, gtStandard Fallback, inter, inter Fallback`. Other loaded fonts: inter Fallback, ibmPlexMono Fallback.

- **headline-display:** gtStandard 63.5px at weight 500, line height 1.02, tracking -0.02em (58px on mobile). Page title (h1).
- **headline-lg:** gtStandard 36px at weight 500, line height 1.22, tracking -0.02em. Section headings (h2).
- **headline-md:** system-ui 21px at weight 600, line height 1.5, tracking -0.008em. Sub-section headings.
- **headline-sm:** gtStandard 20px at weight 500, line height 1.2, tracking -0.01em. Card and feature titles.
- **body-md:** inter 16px at weight 400, line height 1.15, tracking -0.01em. Body text.
- **body-lg:** inter 19px at weight 400, line height 1.6, tracking -0.008em. Lead paragraphs.
- **body-sm:** inter 14px at weight 400, line height 1.7, tracking -0.011em. Secondary and small text.
- **caption:** inter 12px at weight 400, line height 1.63, tracking -0.013em. Captions and fine print.
- **label-lg:** system-ui 16px at weight 400, line height 1.15, tracking -0.01em. Large buttons and tabs.
- **label-md:** inter 15px at weight 600, line height 1.15, tracking -0.011em. Buttons, navigation and labels.
- **label-sm:** inter 14px at weight 600, line height 1.63, tracking -0.011em. Small labels and badges.
- **code:** ibmPlexMono 12px at weight 400, line height 1.63, tracking -0.013em, uppercase. Code and technical values.

## Layout

Spacing does not follow a strict grid: 33% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 5px, md 10px, lg 22px, xl 40px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 760px.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 480px, 500px, 576px, 640px, 768px, 1024px, 1140px, 1199px, 1200px, 1375px, 2160px, 2560px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(255, 180, 115, 0.22) 0px 0px 22px 0px, rgba(255, 180, 115, 0.14) 0px 0px 22px 0px inset`
- `rgba(14, 7, 4, 0.5) 0px 16px 40px 0px, rgba(255, 224, 196, 0.06) 0px 1px 0px 0px inset`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 68 elements.
- **lg (12px):** 20 elements.
- **sm (5px):** 16 elements.
- **md (8px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign Up for Free”):** #E0531F fill, #FFFFFF text, 14px/600, 5px radius, padding 4px 12px.
- **button-primary-hover:** background #FF6C37, text #FFFFFF on hover.
- **button-secondary (“Claude Code”):** #0A0503 fill, #FFF0DE text, 16px/400, 999px radius, padding 11px, border 1px solid #FFE0C424.
- **button-tertiary (“Claude Code”):** #120A06B8 fill, #FFE0C4D9 text, 14px/400, 999px radius, padding 10px 14px 10px 18px, border 1px solid #FFE0C429.
- **button-ghost (“Product”):** transparent fill, #8A8178 text, 14px/600, padding 0px 15px.
- **card:** transparent fill, #212121 text, 16px/400, 12px radius, padding 0px, border 1px solid #FFE0C424, shadow `rgba(14, 7, 4, 0.5) 0px 16px 40px 0px, rgba(255, 224, 196, 0.06) 0px 1px 0px 0px inset`.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FF6C37 for the page.
- Do keep text in 3 levels: #212121, #FFFFFF, #FFF0DE.
- Do use #FF6C37 as the brand accent: header, logo and key highlights.
- Do set headlines in gtStandard with tight tracking (-0.02em).
- Do reuse the measured spacing steps (5px, 10px, 22px).
- Do make buttons and chips fully rounded (9999px); most other elements use 12px corners.
- Don't use #FFFFFF for body text; it reaches 2.8:1 on #FF6C37. Keep it for large text or metadata.
- Don't use #FFF0DE for body text; it reaches 2.5:1 on #FF6C37. Keep it for large text or metadata.
- Don't introduce new font families beyond gtStandard, system-ui, inter and ibmPlexMono.
- Don't use #FF6C37 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.1s, 0.3s.

- **Easing:** `ease`, `cubic-bezier(0.2, 0.7, 0.2, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/postman.com/), the free DESIGN.md generator.
