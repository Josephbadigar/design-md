---
version: alpha
name: Spline
description: "Dark monochrome interface measured from spline.design: Geist type with Spline Sans, tonal surfaces and pill-shaped controls."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#8A8A8A"
  on-background: "#8A8A8A"
  on-surface-strong: "#E6E6E6"
  on-surface-variant: "#BDBDBD"
  on-surface-muted: "#999999"
  surface-container-low: "#101010"
  surface-container: "#181818"
  surface-container-high: "#242424"
  overlay: "#FFFFFF0F"
  overlay-strong: "#FFFFFF1A"
  outline: "#2E2E2E"
  outline-variant: "#1E1E1E"
  primary: "#EEEEEE"
  on-primary: "#000000"
  inverse-surface: "#3E3E3E"
  secondary: "#8EB2F2"
  tertiary: "#F2C879"
typography:
  display-hero:
    fontFamily: Geist
    fontSize: 56px
    fontWeight: 450
    lineHeight: 1.14
    letterSpacing: -0.06em
  headline-display:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: 450
    lineHeight: 1.17
    letterSpacing: -0.06em
  headline-lg:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: 450
    lineHeight: 1.25
    letterSpacing: -0.05em
  body-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.55
  body-lg:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.55
  body-sm:
    fontFamily: Spline Sans
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.45
  label-lg:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.55
  label-md:
    fontFamily: Geist
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.55
  label-sm:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.55
  code:
    fontFamily: Geist Mono
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: 0.08em
  headline-display-mobile:
    fontFamily: Geist
    fontSize: 36px
    fontWeight: 450
    lineHeight: 1.22
    letterSpacing: -0.06em
  display-hero-mobile:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: 450
    lineHeight: 1.25
    letterSpacing: -0.05em
rounded:
  sm: 6px
  md: 8px
  lg: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 20px
  xl: 40px
  gutter: 8px
  section: 256px
  margin: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 0px 14px
    height: 34px
  button-primary-hover:
    backgroundColor: "#FFFFFF"
  button-secondary:
    backgroundColor: "#1F1F1F"
    textColor: "{colors.primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 0px 10px
    height: 24px
  button-outline:
    textColor: "{colors.primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 0px 14px
    height: 34px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 10px
  input-field:
    textColor: "#FFFFFF"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 2px 8px 0px 8px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Spline Design System

## Overview

Spline describes itself as: “Spline is a free 3D design tool in the browser. Your team and its agents model, animate and ship interactive 3D together, in real time.” The interface is dark, built on **Near Black (#000000)** with **Gray (#8A8A8A)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Geist** and **Spline Sans**, with **Geist Mono** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [spline.design](https://spline.design/) on October 29, 2026 at 1440×900 and 390×844 from 393 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles.

- **Near Black (#000000):** Page background, seen 1 time. Token `background`, CSS `--color-bg`.
- **Gray (#8A8A8A):** Primary text and headings, seen 63 times. Token `on-surface`.
- **Mist (#E6E6E6):** Headings and emphasis, seen 19 times. Token `on-surface-strong`, CSS `--color-white-090`.
- **Silver (#BDBDBD):** Secondary text, seen 30 times. Token `on-surface-variant`.
- **Gray (#999999):** Muted text and metadata, seen 13 times. Token `on-surface-muted`, CSS `--color-text-paragraph`.
- **Charcoal (#101010):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Charcoal (#181818):** Cards and panels, seen 6 times. Token `surface-container`.
- **Graphite (#242424):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **White 6% (#FFFFFF0F):** Translucent fill for cards and controls, seen 25 times. Token `overlay`, CSS `--color-btn-bg-highlight`.
- **White 10% (#FFFFFF1A):** Stronger translucent fill, seen 8 times. Token `overlay-strong`, CSS `--color-white-010`.
- **Graphite (#2E2E2E):** Borders and dividers, seen 4 times. Token `outline`.
- **Charcoal (#1E1E1E):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Mist (#EEEEEE):** Primary buttons and calls to action, seen 17 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Graphite (#3E3E3E):** High-contrast fills, seen 2 times. Token `inverse-surface`.
- **Light Blue (#8EB2F2):** Accent in text, fills and borders, seen 5 times. Token `secondary`.
- **Light Orange (#F2C879):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.

## Typography

**Geist**, **Spline Sans** and **Geist Mono** (monospace) share the interface. Fallback stack: `Geist, Geist Fallback, Helvetica Neue, Arial`.

- **display-hero:** Geist 56px at weight 450, line height 1.14, tracking -0.06em (32px on mobile). Oversized hero statements.
- **headline-display:** Geist 48px at weight 450, line height 1.17, tracking -0.06em (36px on mobile). Page title (h1).
- **headline-lg:** Geist 24px at weight 450, line height 1.25, tracking -0.05em. Section headings (h2).
- **body-md:** Geist 14px at weight 400, line height 1.55. Body text.
- **body-lg:** Geist 16px at weight 400, line height 1.55. Lead paragraphs.
- **body-sm:** Spline Sans 11px at weight 400, line height 1.45. Secondary and small text.
- **label-lg:** Geist 16px at weight 500, line height 1.55. Large buttons and tabs.
- **label-md:** Geist 15px at weight 400, line height 1.55. Buttons, navigation and labels.
- **label-sm:** Geist 14px at weight 500, line height 1.55. Small labels and badges.
- **code:** Geist Mono 11px at weight 400, line height 1.55, tracking 0.08em. Code and technical values.

## Layout

Spacing does not follow a strict grid: 58% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 10px, lg 20px, xl 40px.
- **Sections:** 256px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 48px on each side of full-width sections.
- **Breakpoints:** 400px, 560px, 625px, 640px, 720px, 780px, 820px, 821px, 1000px, 1080px, 1160px, 1200px, 1280px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#101010 → #181818 → #242424) and hairline rings:

- `rgb(29, 29, 29) 0px 0px 0px 2px`
- `rgb(16, 16, 16) 0px 0px 0px 2px`
- `rgba(255, 255, 255, 0.06) 0px 0px 0px 1px inset`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 228 elements.
- **sm (6px):** 116 elements.
- **md (8px):** 60 elements.
- **lg (16px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start building”):** #EEEEEE fill, #000000 text, 14px/500, 999px radius, padding 0px 14px, border 1px solid #EEEEEE.
- **button-primary-hover:** background #FFFFFF, text #000000 on hover.
- **button-secondary (“Web”):** #1F1F1F fill, #EEEEEE text, 11px/400, 999px radius, padding 0px 10px.
- **button-outline (“Talk to sales”):** transparent fill, #EEEEEE text, 14px/500, 999px radius, padding 0px 14px, border 1px solid #2E2E2E.
- **button-ghost (“Products”):** transparent fill, #8A8A8A text, 14px/400, 8px radius, padding 0px 10px.
- **input-field (“Ask Spline to build a low-poly c”):** transparent fill, #FFFFFF text, 16px/400, padding 2px 8px 0px 8px.
- **card:** #101010 fill, #EEEEEE text, 16px/400, 16px radius, padding 0px.
- **link:** transparent fill, #BDBDBD text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #101010, #181818, #242424.
- Do keep text in 4 levels: #8A8A8A, #E6E6E6, #BDBDBD, #999999.
- Do let contrast carry emphasis; primary actions use #EEEEEE on #000000.
- Do set headlines in Geist with tight tracking (-0.06em).
- Do reuse the measured spacing steps (8px, 10px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 6px corners.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Geist, Spline Sans and Geist Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.2s, 0.35s, 0.15s, 0.5s. Longer ambient animations run 1.2s.

- **Easing:** `ease`, `cubic-bezier(0.2, 0.8, 0.2, 1)`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/spline.design/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
