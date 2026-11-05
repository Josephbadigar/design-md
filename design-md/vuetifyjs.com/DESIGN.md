---
version: alpha
name: Vuetify
description: "Light interface measured from vuetifyjs.com: Roboto type, blue accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#666666"
  on-background: "#666666"
  on-surface-strong: "#000000"
  on-surface-variant: "#212121"
  surface-container-low: "#EEEEEE"
  outline: "#0000001F"
  outline-variant: "#1867C01F"
  primary: "#2373C4"
  on-primary: "#FFFFFF"
  inverse-surface: "#121212"
  secondary: "#E2777A"
  tertiary: "#2196F3"
typography:
  headline-display:
    fontFamily: Roboto
    fontSize: 57px
    fontWeight: 700
    lineHeight: 1.12
    letterSpacing: -0.004em
  headline-lg:
    fontFamily: Roboto
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.25
  headline-md:
    fontFamily: Roboto
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.27
  body-md:
    fontFamily: Roboto
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Roboto
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.018em
  label-lg:
    fontFamily: Roboto
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.007em
  label-md:
    fontFamily: Roboto
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Roboto
    fontSize: 12px
    fontWeight: 500
    letterSpacing: 0.007em
  code:
    fontFamily: monospace
    fontSize: 14px
    fontWeight: 500
  headline-display-mobile:
    fontFamily: Roboto
    fontSize: 45px
    fontWeight: 700
    lineHeight: 1.16
rounded:
  sm: 4px
  md: 8px
  lg: 24px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 34px
  gutter: 8px
  section: 152px
  margin: 16px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 8px
    height: 72px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
    height: 36px
  button-tertiary:
    backgroundColor: "#1867C0"
    textColor: "#1867C0"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 0px 12px
    height: 36px
  button-ghost:
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 8px
  card:
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 8px
---

# Vuetify Design System

## Overview

Vuetify describes itself as: “Vuetify is a no-design-skills-required Open Source UI component framework for Vue with everything you need to build ...” The interface is light, built on **White (#FFFFFF)** with **Slate (#666666)** text, and **Blue (#2373C4)** as the main accent.

Type is set in **Roboto**, with **monospace** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [vuetifyjs.com/en](https://vuetifyjs.com/en/) (the site sent our reader to its /en version; vuetifyjs.com was asked for) on November 4, 2026 at 1440×900 and 390×844 from 398 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 27 times. Token `background`.
- **Slate (#666666):** Primary text and headings. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 3 times. Token `on-surface-strong`, CSS `--prism-keyword`.
- **Charcoal (#212121):** Secondary text, seen 24 times. Token `on-surface-variant`.
- **Mist (#EEEEEE):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Near Black 12% (#0000001F):** Borders and dividers, seen 8 times. Token `outline`.
- **Blue 12% (#1867C01F):** Secondary dividers, seen 6 times. Token `outline-variant`.
- **Blue (#2373C4):** Brand color in the header, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#121212):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Red (#E2777A):** Accent in text, fills and borders, seen 5 times. Token `secondary`.
- **Vivid Blue (#2196F3):** Accent, seen 3 times. Token `tertiary`.

## Typography

**Roboto** and **monospace** (monospace) share the interface. Fallback stack: `Roboto, sans-serif`.

- **headline-display:** Roboto 57px at weight 700, line height 1.12, tracking -0.004em (45px on mobile). Page title (h1).
- **headline-lg:** Roboto 32px at weight 700, line height 1.25. Section headings (h2).
- **headline-md:** Roboto 22px at weight 400, line height 1.27. Sub-section headings.
- **body-md:** Roboto 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Roboto 14px at weight 400, line height 1.5, tracking 0.018em. Secondary and small text.
- **label-lg:** Roboto 16px at weight 500, line height 1.5, tracking 0.007em. Large buttons and tabs.
- **label-md:** Roboto 14px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Roboto 12px at weight 500, tracking 0.007em. Small labels and badges.
- **code:** monospace 14px at weight 500. Code and technical values.

## Layout

Spacing follows a 4px grid: 95% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 34px.
- **Sections:** 152px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 16px on each side of full-width sections.
- **Breakpoints:** 599.98px, 600px, 839.98px, 840px, 1144.98px, 1145px, 1544.98px, 1545px, 2137.98px, 2138px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#EEEEEE):

- `rgba(0, 0, 0, 0.3) 0px 0px 0px 0px, rgba(0, 0, 0, 0.15) 0px 0px 0px 0px`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0.3) 0px 1px 2px 0px, rgba(0, 0, 0, 0.15) 0px 2px 6px 2px`.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 152 elements.
- **md (8px):** 92 elements.
- **full (9999px):** 40 elements.
- **lg (24px):** 32 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“DeepCloud AG”):** #000000DE fill, #000000DE text, 16px/400, 4px radius, padding 8px, shadow `rgba(0, 0, 0, 0.3) 0px 0px 0px 0px, rgba(0, 0, 0, 0.15) 0px 0px 0px 0px`.
- **button-secondary (“SearchCtrl+K”):** #00000099 fill, #00000099 text, 14px/400, 4px radius, padding 0px 12px.
- **button-tertiary (“One”):** #1867C0 fill, #1867C0 text, 14px/400, 8px radius, padding 0px 12px, border 1px solid #1867C0.
- **button-ghost (“v4.3.2”):** transparent fill, 14px/500, 4px radius, padding 0px 8px.
- **card:** transparent fill, 16px/400, 4px radius, padding 8px, shadow `rgba(0, 0, 0, 0.3) 0px 0px 0px 0px, rgba(0, 0, 0, 0.15) 0px 0px 0px 0px`.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #EEEEEE.
- Do keep text in 3 levels: #666666, #000000, #212121.
- Do use #2373C4 as the brand accent: header, logo and key highlights.
- Do set headlines in Roboto with tight tracking (-0.004em).
- Do keep spacing on the 4px grid.
- Do use 4px corners on most elements; larger surfaces also use 8px and 24px.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Roboto and monospace.
- Don't use #2373C4 for large backgrounds or body text.
- Don't make interface transitions slower than 0.28s.

## Motion

Interface transitions are quick: 0.28s, 0.2s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/vuetifyjs.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
