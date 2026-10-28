---
version: alpha
name: Motion
description: "Dark interface measured from motion.dev: TASA Orbiter type with system-ui, vivid amber accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#080808"
  surface: "#080808"
  on-surface: "#EDEBE5"
  on-background: "#EDEBE5"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#979D97"
  on-surface-muted: "#6E6A64"
  surface-container-low: "#000000"
  surface-container: "#0E1312"
  surface-container-high: "#141214"
  overlay: "#EDEBE524"
  overlay-strong: "#EDEBE529"
  outline: "#343034"
  outline-variant: "#EDEBE529"
  primary: "#FBD509"
  on-primary: "#080808"
  inverse-surface: "#636361"
  secondary: "#26210C"
  tertiary: "#FFDB2A"
  error: "#F43F5E"
  success: "#52CD86"
typography:
  display-hero:
    fontFamily: TASA Orbiter
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.035em
  headline-display:
    fontFamily: TASA Orbiter
    fontSize: 34.5px
    fontWeight: 700
    lineHeight: 1.08
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: TASA Orbiter
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-md:
    fontFamily: TASA Orbiter
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-md:
    fontFamily: TASA Orbiter
    fontSize: 16px
    fontWeight: 400
  body-sm:
    fontFamily: TASA Orbiter
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.35
  caption:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
  code:
    fontFamily: Geist Mono
    fontSize: 11px
    fontWeight: 400
    letterSpacing: 0.1em
  headline-display-mobile:
    fontFamily: TASA Orbiter
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: -0.035em
  display-hero-mobile:
    fontFamily: TASA Orbiter
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.035em
rounded:
  md: 3px
  full: 9999px
spacing:
  xs: 3px
  sm: 8px
  md: 12px
  lg: 18px
  xl: 48px
  gutter: 12px
  section: 96px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.code}"
    rounded: 0px
    padding: 12px 18px
    height: 48px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.code}"
    rounded: 0px
    padding: 12px 18px
    height: 48px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.code}"
    rounded: 0px
    padding: 5px 9px
  input-field:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.caption}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 96px 0px
  link:
    textColor: "{colors.on-surface}"
---

# Motion Design System

## Overview

Motion describes itself as: “Motion (prev Framer Motion) is a fast, production-grade animation library for React, JavaScript and Vue. Build smooth UI animations at a tiny footprint.” The interface is dark, built on **Near Black (#080808)** with **Warm Mist (#EDEBE5)** text, and **Vivid Amber (#FBD509)** as the main accent.

Type is set in **TASA Orbiter** and **system-ui**, with **Geist Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [motion.dev](https://motion.dev/) on October 21, 2026 at 1440×900 and 390×844 from 462 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 19 roles.

- **Near Black (#080808):** Page background, seen 29 times. Token `background`.
- **Warm Mist (#EDEBE5):** Primary text and headings, seen 72 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 3 times. Token `on-surface-strong`.
- **Gray (#979D97):** Secondary text, seen 17 times. Token `on-surface-variant`.
- **Warm Slate (#6E6A64):** Muted text and metadata, seen 5 times. Token `on-surface-muted`.
- **Near Black (#000000):** Raised areas one step from the page, seen 13 times. Token `surface-container-low`.
- **Charcoal (#0E1312):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--background`.
- **Charcoal (#141214):** Hover and pressed fills, seen 12 times. Token `surface-container-high`.
- **Warm Mist 14% (#EDEBE524):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Warm Mist 16% (#EDEBE529):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Graphite (#343034):** Borders and dividers, seen 28 times. Token `outline`.
- **Warm Mist 16% (#EDEBE529):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Amber (#FBD509):** Primary buttons and calls to action, seen 5 times. Token `primary`.
- **Near Black (#080808):** Text and icons on primary. Token `on-primary`.
- **Slate (#636361):** High-contrast fills, seen 8 times. Token `inverse-surface`.
- **Deep Amber (#26210C):** Brand accent (CSS variable), seen 12 times. Token `secondary`.
- **Vivid Amber (#FFDB2A):** Brand accent (CSS variable), seen 12 times. Token `tertiary`.
- **Vivid Red (#F43F5E):** Errors and destructive states, seen 6 times. Token `error`.
- **Green (#52CD86):** Success and positive states, seen 4 times. Token `success`.

## Typography

**TASA Orbiter**, **system-ui** and **Geist Mono** (monospace) share the interface. Fallback stack: `TASA Orbiter, sans-serif`.

- **display-hero:** TASA Orbiter 40px at weight 700, line height 1.1, tracking -0.035em (28px on mobile). Oversized hero statements.
- **headline-display:** TASA Orbiter 34.5px at weight 700, line height 1.08, tracking -0.035em (30px on mobile). Page title (h1).
- **headline-lg:** TASA Orbiter 30px at weight 700, line height 1.1, tracking -0.03em. Section headings (h2).
- **headline-md:** TASA Orbiter 20px at weight 700, line height 1.2, tracking -0.02em. Sub-section headings.
- **body-md:** TASA Orbiter 16px at weight 400. Body text.
- **body-sm:** TASA Orbiter 15px at weight 400, line height 1.35. Secondary and small text.
- **caption:** system-ui 12px at weight 400, line height 1.4. Captions and fine print.
- **code:** Geist Mono 11px at weight 400, tracking 0.1em, uppercase. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (75% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 3px, sm 8px, md 12px, lg 18px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 360px, 400px, 480px, 600px, 620px, 700px, 760px, 768px, 780px, 800px, 900px, 1000px, 1001px, 1080px, 1100px, 1199px, 1200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.2) 0px 1px 0px 0px, rgba(0, 0, 0, 0.6) 0px 18px 40px -16px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 16 elements.
- **md (3px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“GET STARTED GET STARTED”):** #FBD509 fill, #080808 text, 11px/400, padding 12px 18px, border 1px solid #FBD509.
- **button-outline (“MOTION+ MOTION+”):** #080808 fill, #979D97 text, 11px/400, padding 12px 18px, border 1px solid #EDEBE529.
- **button-ghost (“RUNWAY”):** transparent fill, #080808 text, 11px/400, padding 5px 9px.
- **input-field:** transparent fill, #FFFFFF text, 12px/400, padding 0px.
- **card:** #080808 fill, 16px/400, padding 96px 0px.
- **link:** transparent fill, #EDEBE5 text, padding 0px.

## Do's and Don'ts

- Do use #080808 for the page and lift surfaces in small steps: #000000, #0E1312, #141214.
- Do keep text in 4 levels: #EDEBE5, #FFFFFF, #979D97, #6E6A64.
- Do reserve #FBD509 for primary actions and key highlights.
- Do set headlines in TASA Orbiter with tight tracking (-0.035em).
- Do reuse the measured spacing steps (8px, 12px, 18px).
- Do make buttons and chips fully rounded (9999px); most other elements use 3px corners.
- Don't use #6E6A64 for body text; it reaches 3.7:1 on #080808. Keep it for large text or metadata.
- Don't introduce new font families beyond TASA Orbiter, system-ui and Geist Mono.
- Don't use #FBD509 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/motion.dev/), the free DESIGN.md generator.
