---
version: alpha
name: Retool
description: "Dark interface measured from retool.com: saansFont type with pxGroteskFont, vivid orange accents, tonal surfaces and 12px corners."
colors:
  background: "#151515"
  surface: "#151515"
  on-surface: "#E9EBDF"
  on-background: "#E9EBDF"
  on-surface-strong: "#F7F8F4"
  on-surface-variant: "#CBCCC4"
  surface-container-low: "#242424"
  overlay: "#15151510"
  overlay-strong: "#000000CC"
  outline: "#433E38"
  outline-variant: "#1515151F"
  primary: "#ECA438"
  on-primary: "#000000"
  secondary: "#EF4444"
  tertiary: "#518DD2"
typography:
  headline-display:
    fontFamily: saansFont
    fontSize: 72px
    fontWeight: 300
    lineHeight: 1.05
    letterSpacing: -0.022em
  headline-lg:
    fontFamily: saansFont
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.05
    letterSpacing: -0.01em
  headline-md:
    fontFamily: saansFont
    fontSize: 24px
    fontWeight: 380
    lineHeight: 1.2
    letterSpacing: -0.01em
  body-md:
    fontFamily: pxGroteskFont
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.2
  body-lg:
    fontFamily: saansFont
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.5
    letterSpacing: 0.01em
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: pxGroteskFont
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0.01em
  headline-display-mobile:
    fontFamily: saansFont
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.05
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: saansFont
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.05
    letterSpacing: -0.01em
  headline-md-mobile:
    fontFamily: saansFont
    fontSize: 20px
    fontWeight: 380
    lineHeight: 1.2
    letterSpacing: -0.01em
rounded:
  sm: 8px
  md: 12px
  lg: 16px
  xl: 36px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 24px
  section: 80px
  container: 1440px
components:
  button-primary:
    backgroundColor: "#D9D9D9"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 38px
  button-outline:
    backgroundColor: "{colors.overlay-strong}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    padding: 0px
    height: 40px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    padding: 0px 20px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Retool Design System

## Overview

Retool describes itself as: “Build, deploy, and manage internal tools with Retool's unified engine. Connect to any database, API, or LLM. Leverage AI throughout your business.” The interface is dark, built on **Charcoal (#151515)** with **Mist (#E9EBDF)** text, and **Vivid Orange (#ECA438)** as the main accent.

Type is set in **saansFont** and **pxGroteskFont**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 12px.

Measured from [retool.com](https://retool.com/) on October 29, 2026 at 1440×900 and 390×844 from 363 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Charcoal (#151515):** Page background, seen 5 times. Token `background`, CSS `--color-surface-background-base`.
- **Mist (#E9EBDF):** Primary text and headings, seen 40 times. Token `on-surface`, CSS `--btn-secondary-red-hover-text`.
- **Snow (#F7F8F4):** Headings and emphasis, seen 2 times. Token `on-surface-strong`.
- **Warm Silver (#CBCCC4):** Secondary text, seen 7 times. Token `on-surface-variant`.
- **Graphite (#242424):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **Charcoal 6% (#15151510):** Translucent fill for cards and controls, seen 2 times. Token `overlay`, CSS `--raw-dark-black-2-alpha-6`.
- **Near Black 80% (#000000CC):** Stronger translucent fill, seen 1 time. Token `overlay-strong`, CSS `--nav-scrolled-background`.
- **Warm Graphite (#433E38):** Borders and dividers, seen 52 times. Token `outline`.
- **Charcoal 12% (#1515151F):** Secondary dividers, seen 8 times. Token `outline-variant`.
- **Vivid Orange (#ECA438):** Brand accent (CSS variable). Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Red (#EF4444):** Accent (CSS variable). Token `secondary`.
- **Blue (#518DD2):** Accent in text, fills and borders, seen 2 times. Token `tertiary`, CSS `--nav-items-active-selected`.

## Typography

**saansFont**, **pxGroteskFont** and **system-ui** share the interface. Fallback stack: `saansFont, saansFont Fallback, sans-serif`.

- **headline-display:** saansFont 72px at weight 300, line height 1.05, tracking -0.022em (40px on mobile). Page title (h1).
- **headline-lg:** saansFont 48px at weight 300, line height 1.05, tracking -0.01em (40px on mobile). Section headings (h2).
- **headline-md:** saansFont 24px at weight 380, line height 1.2, tracking -0.01em (20px on mobile). Sub-section headings.
- **body-md:** pxGroteskFont 14px at weight 400, line height 1.2. Body text.
- **body-lg:** saansFont 16px at weight 300, line height 1.5, tracking 0.01em. Lead paragraphs.
- **label-md:** system-ui 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** pxGroteskFont 12px at weight 400, line height 1.2, tracking 0.01em, uppercase. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (86% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Breakpoints:** 400px, 544px, 640px, 767px, 768px, 1024px, 1200px, 1280px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#242424) and #433E38 borders.

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **md (12px):** 20 elements.
- **lg (16px):** 20 elements.
- **xl (36px):** 16 elements.
- **sm (8px):** 8 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Import code”):** #D9D9D9 fill, #15151599 text, 14px/400, 12px radius, padding 8px 12px, border 1px solid #1515151F.
- **button-outline (“See what's new. Watch the film”):** #000000CC fill, #E9EBDF text, 16px/400, 3.35544e+07px radius, padding 0px, border 1px solid #E9EBDF1F.
- **button-secondary (“Start for free”):** #E9EBDF fill, #151515 text, 14px/400, 3.35544e+07px radius, padding 0px 20px.
- **button-ghost (“Solution”):** transparent fill, #E9EBDF text, 16px/400, padding 0px.
- **link:** transparent fill, #CBCCC4 text, padding 0px.

## Do's and Don'ts

- Do use #151515 for the page and lift surfaces in small steps: #242424.
- Do keep text in 3 levels: #E9EBDF, #F7F8F4, #CBCCC4.
- Do use #ECA438 as the brand accent: header, logo and key highlights.
- Do set headlines in saansFont with tight tracking (-0.022em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 12px corners on most elements; larger surfaces also use 16px, 36px and 8px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond saansFont, pxGroteskFont and system-ui.
- Don't use #ECA438 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.6s, 0.2s, 0.4s, 0.3s.

- **Easing:** `cubic-bezier(0.72, 0, 0.12, 1)`, `cubic-bezier(0.24, 0.01, 0.36, 1)`, `cubic-bezier(0.12, 1, 0.72, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/retool.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
