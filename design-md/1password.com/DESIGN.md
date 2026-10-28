---
version: alpha
name: 1Password
description: "Dark interface measured from 1password.com: agileSans type, amber accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#1D1D21"
  surface: "#1D1D21"
  on-surface: "#D2D2D3"
  on-background: "#D2D2D3"
  on-surface-strong: "#FFFFFF"
  surface-container-low: "#303136"
  primary: "#CBB88E"
  on-primary: "#000000"
  secondary: "#145FE4"
typography:
  headline-display:
    fontFamily: agileSans
    fontSize: 88px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: agileSans
    fontSize: 64px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  body-md:
    fontFamily: agileSans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: agileSans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-sm:
    fontFamily: agileSans
    fontSize: 14px
    fontWeight: 300
    lineHeight: 1.5
    letterSpacing: -0.02em
  label-md:
    fontFamily: agileSans
    fontSize: 16px
    fontWeight: 350
    lineHeight: 1.6
    letterSpacing: -0.02em
  headline-display-mobile:
    fontFamily: agileSans
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: agileSans
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
rounded:
  md: 2px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 24px
  gutter: 16px
  section: 224px
  margin: 24px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.secondary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 10px 24px
    height: 46px
  button-primary-hover:
    textColor: "{colors.on-surface-strong}"
  button-secondary:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 10px 24px
    height: 46px
  button-secondary-hover:
    textColor: "{colors.background}"
  button-tertiary:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 2px 0px
    height: 28px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 2px 0px
  link:
    textColor: "{colors.on-surface}"
---

# 1Password Design System

## Overview

1Password describes itself as: “Protect passwords and secrets, manage app access, and secure AI tools with 1Password. Easy to adopt from growing teams to enterprise.” The interface is dark, built on **Charcoal (#1D1D21)** with **Silver (#D2D2D3)** text, and **Amber (#CBB88E)** as the main accent.

Type is set in **agileSans**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [1password.com](https://1password.com/) on October 21, 2026 at 1440×900 and 390×844 from 301 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **Charcoal (#1D1D21):** Page background, seen 3 times. Token `background`.
- **Silver (#D2D2D3):** Primary text and headings. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 39 times. Token `on-surface-strong`, CSS `--tw-ring-offset-color`.
- **Cool Graphite (#303136):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Amber (#CBB88E):** Brand color in the header. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#145FE4):** Most used accent color, seen 10 times. Token `secondary`.

## Typography

**agileSans** carries the whole interface. Fallback stack: `agileSans, agileSans Fallback, sans-serif`.

- **headline-display:** agileSans 88px at weight 300, line height 1.1, tracking -0.02em (48px on mobile). Page title (h1).
- **headline-lg:** agileSans 64px at weight 300, line height 1.1, tracking -0.02em (40px on mobile). Section headings (h2).
- **body-md:** agileSans 16px at weight 400, line height 1.5. Body text.
- **body-lg:** agileSans 18px at weight 400, line height 1.2, tracking -0.02em. Lead paragraphs.
- **body-sm:** agileSans 14px at weight 300, line height 1.5, tracking -0.02em. Secondary and small text.
- **label-md:** agileSans 16px at weight 350, line height 1.6, tracking -0.02em. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (72% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 8px, md 12px, lg 24px.
- **Sections:** 224px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 375px, 415px, 563px, 568px, 662px, 768px, 1023px, 1024px, 1025px, 1180px, 1200px, 1261px, 1440px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#303136).

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 32 elements.
- **md (2px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Talk to sales”):** #FFFFFF fill, #145FE4 text, 16px/400, 9999px radius, padding 10px 24px.
- **button-primary-hover:** background #FFFFFF, text #FFFFFF on hover.
- **button-secondary (“View plans”):** #FFFFFF fill, #FFFFFF text, 16px/400, 9999px radius, padding 10px 24px.
- **button-secondary-hover:** background #FFFFFF, text #1D1D21 on hover.
- **button-tertiary (“Business”):** transparent fill, #000000 text, 16px/350, padding 2px 0px.
- **button-ghost (“Business”):** transparent fill, #000000 text, 16px/350, padding 2px 0px.
- **link:** transparent fill, #FFFFFFCC text, padding 0px.

## Do's and Don'ts

- Do use #1D1D21 for the page and lift surfaces in small steps: #303136.
- Do keep text in 2 levels: #D2D2D3, #FFFFFF.
- Do use #CBB88E as the brand accent: header, logo and key highlights.
- Do set headlines in agileSans with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 2px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond agileSans.
- Don't use #CBB88E for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/1password.com/), the free DESIGN.md generator.
