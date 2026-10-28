---
version: alpha
name: Bun
description: "Dark monochrome interface measured from bun.sh: Archivo type with system-ui, tonal surfaces and pill-shaped controls."
colors:
  background: "#0D0A0C"
  surface: "#0D0A0C"
  on-surface: "#EAEAE8"
  on-background: "#EAEAE8"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#A8A8A5"
  on-surface-muted: "#80807E"
  surface-container-low: "#0E0E0E"
  surface-container: "#000000"
  surface-container-high: "#171316"
  surface-container-highest: "#1E1E21"
  overlay: "#EAEAE899"
  overlay-strong: "#FFFFFF26"
  outline: "#28282B"
  outline-variant: "#3E3E42"
  primary: "#EAEAE8"
  on-primary: "#0D0A0C"
  secondary: "#FF2E97"
  success: "#28DC82"
  warning: "#FCD34D"
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
    rounded: 0px
    padding: 0px 14px
    height: 36px
  button-primary-hover:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface-strong}"
  button-outline:
    backgroundColor: "{colors.surface-container-highest}"
    textColor: "#F0F0EE"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 3px 10px
    height: 24px
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-muted}"
    rounded: 0px
    padding: 0px 12px
    height: 36px
  link:
    textColor: "{colors.primary}"
---

# Bun Design System

## Overview

Bun describes itself as: “Bundle, install, and run JavaScript & TypeScript — all in Bun. Bun is a fast JavaScript runtime & toolkit with a bundler, test runner, and npm-compatible package manager built in.” The interface is dark, built on **Charcoal (#0D0A0C)** with **Mist (#EAEAE8)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Archivo** and **system-ui**, with **Martian Mono** for code. Headlines run large with tight negative tracking; body text is 14.5px. The surface language is flat. Controls are pill-shaped.

Measured from [bun.sh](https://bun.sh/) on October 21, 2026 at 1440×900 and 390×844 from 423 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 18 roles.

- **Charcoal (#0D0A0C):** Page background, seen 19 times. Token `background`.
- **Mist (#EAEAE8):** Primary text and headings, seen 41 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 2 times. Token `on-surface-strong`, CSS `--tw-ring-offset-color`.
- **Gray (#A8A8A5):** Secondary text, seen 22 times. Token `on-surface-variant`.
- **Slate (#80807E):** Muted text and metadata, seen 37 times. Token `on-surface-muted`.
- **Charcoal (#0E0E0E):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Near Black (#000000):** Cards and panels, seen 5 times. Token `surface-container`.
- **Charcoal (#171316):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Charcoal (#1E1E21):** Highest raised elements, seen 2 times. Token `surface-container-highest`.
- **Mist 60% (#EAEAE899):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **White 15% (#FFFFFF26):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Graphite (#28282B):** Borders and dividers, seen 23 times. Token `outline`.
- **Graphite (#3E3E42):** Secondary dividers, seen 11 times. Token `outline-variant`.
- **Mist (#EAEAE8):** Primary buttons and calls to action, seen 66 times. Token `primary`.
- **Charcoal (#0D0A0C):** Text and icons on primary. Token `on-primary`.
- **Vivid Pink (#FF2E97):** Most used accent color, seen 15 times. Token `secondary`.
- **Teal (#28DC82):** Success and positive states, seen 10 times. Token `success`.
- **Amber (#FCD34D):** Warnings and highlights, seen 1 time. Token `warning`.

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

Spacing does not follow a strict grid: 69% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 12px, lg 24px, xl 40px.
- **Sections:** 112px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 580px, 640px, 767px, 768px, 1024px, 1280px, 1536px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#0E0E0E → #000000 → #171316 → #1E1E21) and #28282B borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (3px):** 188 elements.
- **full (9999px):** 52 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Install”):** #EAEAE8 fill, #0D0A0C text, 13.5px/600, padding 0px 14px.
- **button-primary-hover:** background #FF2E97, text #FFFFFF on hover.
- **button-outline (“Windows”):** #1E1E21 fill, #F0F0EE text, 12px/400, padding 3px 10px.
- **button-ghost (“Search docs, APIs, guides… /”):** #0D0A0C fill, #80807E text, 13.5px/400, padding 0px 12px, border 1px solid #28282B.
- **link:** transparent fill, #EAEAE8 text, padding 0px.

## Do's and Don'ts

- Do use #0D0A0C for the page and lift surfaces in small steps: #0E0E0E, #000000, #171316, #1E1E21.
- Do keep text in 4 levels: #EAEAE8, #FFFFFF, #A8A8A5, #80807E.
- Do let contrast carry emphasis; primary actions use #EAEAE8 on #0D0A0C.
- Do set headlines in Archivo with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 3px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Archivo, system-ui and Martian Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 1e-06s, 0.15s, 0.2s, 0.3s.

- **Easing:** `ease`, `cubic-bezier(0.22, 1, 0.36, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/bun.sh/), the free DESIGN.md generator.
