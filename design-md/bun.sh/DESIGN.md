---
version: alpha
name: Bun
description: "Light monochrome interface measured from bun.sh: Archivo type with system-ui, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0A0A0A"
  on-background: "#0A0A0A"
  on-surface-variant: "#525252"
  on-surface-muted: "#707070"
  surface-container-low: "#F6F6F6"
  overlay: "#0A0A0A99"
  overlay-strong: "#FFFFFF26"
  outline: "#E2E2E2"
  outline-variant: "#FFFFFF33"
  primary: "#0C0C0C"
  on-primary: "#FFFFFF"
  secondary: "#D60066"
  tertiary: "#FF1F8F"
typography:
  display-hero:
    fontFamily: Archivo
    fontSize: 76px
    fontWeight: 800
    lineHeight: 0.92
    letterSpacing: -0.02em
  headline-display:
    fontFamily: Archivo
    fontSize: 68px
    fontWeight: 800
    lineHeight: 0.92
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: system-ui
    fontSize: 20.5px
    fontWeight: 600
    lineHeight: 1.38
    letterSpacing: -0.015em
  body-md:
    fontFamily: system-ui
    fontSize: 14.5px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: system-ui
    fontSize: 17px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: -0.02em
  body-sm:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: system-ui
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: system-ui
    fontSize: 14.5px
    fontWeight: 500
    lineHeight: 1.5
  code:
    fontFamily: Martian Mono
    fontSize: 11px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.04em
  headline-display-mobile:
    fontFamily: Archivo
    fontSize: 40px
    fontWeight: 800
    lineHeight: 0.92
    letterSpacing: -0.02em
  display-hero-mobile:
    fontFamily: Archivo
    fontSize: 41.5px
    fontWeight: 800
    lineHeight: 0.92
    letterSpacing: -0.02em
rounded:
  md: 3px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 12px
  section: 112px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 3px 10px
    height: 24px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    rounded: 0px
    padding: 0px 14px
    height: 36px
  button-secondary-hover:
    backgroundColor: "{colors.tertiary}"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-muted}"
    rounded: 0px
    padding: 0px 12px
    height: 36px
  link:
    textColor: "{colors.secondary}"
---

# Bun Design System

## Overview

Bun describes itself as: “Bundle, install, and run JavaScript & TypeScript — all in Bun. Bun is a fast JavaScript runtime & toolkit with a bundler, test runner, and npm-compatible package manager built in.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#0A0A0A)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Archivo** and **system-ui**, with **Martian Mono** for code. Headlines run large with tight negative tracking; body text is 14.5px. The surface language is flat. Controls are pill-shaped.

Measured from [bun.sh](https://bun.sh/) on October 29, 2026 at 1440×900 and 390×844 from 421 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 18 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Near Black (#0A0A0A):** Primary text and headings, seen 40 times. Token `on-surface`.
- **Slate (#525252):** Secondary text, seen 22 times. Token `on-surface-variant`.
- **Slate (#707070):** Muted text and metadata, seen 37 times. Token `on-surface-muted`.
- **Snow (#F6F6F6):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Near Black 60% (#0A0A0A99):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **White 15% (#FFFFFF26):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Mist (#E2E2E2):** Borders and dividers, seen 22 times. Token `outline`.
- **White 20% (#FFFFFF33):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Charcoal (#0C0C0C):** Primary buttons and calls to action, seen 69 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Pink (#D60066):** Links and interactive text, seen 1 time. Token `secondary`, CSS `--link-hover-color`.
- **Vivid Pink (#FF1F8F):** Accent in text, fills and borders, seen 9 times. Token `tertiary`.

## Typography

**Archivo**, **system-ui** and **Martian Mono** (monospace) share the interface. Fallback stack: `Archivo, ui-sans-serif, system-ui, sans-serif`.

- **display-hero:** Archivo 76px at weight 800, line height 0.92, tracking -0.02em (41.5px on mobile). Oversized hero statements.
- **headline-display:** Archivo 68px at weight 800, line height 0.92, tracking -0.02em (40px on mobile). Page title (h1).
- **headline-lg:** system-ui 20.5px at weight 600, line height 1.38, tracking -0.015em. Section headings (h2).
- **body-md:** system-ui 14.5px at weight 400, line height 1.5. Body text.
- **body-lg:** system-ui 17px at weight 600, line height 1.5, tracking -0.02em. Lead paragraphs.
- **body-sm:** system-ui 12px at weight 400, line height 1.5. Secondary and small text.
- **label-lg:** system-ui 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** system-ui 15px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** system-ui 14.5px at weight 500, line height 1.5. Small labels and badges.
- **code:** Martian Mono 11px at weight 500, line height 1.5, tracking 0.04em, uppercase. Code and technical values.

## Layout

Spacing does not follow a strict grid: 68% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 12px, lg 24px, xl 40px.
- **Sections:** 112px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 580px, 640px, 767px, 768px, 1024px, 1280px, 1536px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F6F6F6) and #E2E2E2 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (3px):** 180 elements.
- **full (9999px):** 52 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“macOS & Linux”):** #0C0C0C fill, #FFFFFF text, 12px/400, padding 3px 10px.
- **button-secondary (“Install”):** #0A0A0A fill, #FFFFFF text, 13.5px/600, padding 0px 14px.
- **button-secondary-hover:** background #FF1F8F, text #FFFFFF on hover.
- **button-outline (“Search docs, APIs, guides… /”):** #FFFFFF fill, #707070 text, 13.5px/400, padding 0px 12px, border 1px solid #E2E2E2.
- **link:** transparent fill, #D60066 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F6F6F6.
- Do keep text in 3 levels: #0A0A0A, #525252, #707070.
- Do let contrast carry emphasis; primary actions use #0C0C0C on #FFFFFF.
- Do set headlines in Archivo with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 3px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Archivo, system-ui and Martian Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.15s, 0.6s, 0.2s, 0.3s. Longer ambient animations run 4.494s.

- **Easing:** `cubic-bezier(0.22, 1, 0.36, 1)`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/bun.sh/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
