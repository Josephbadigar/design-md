---
version: alpha
name: Asana
description: "Light interface measured from asana.com: TWK Lausanne type, red accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0D0D0D"
  on-background: "#0D0D0D"
  on-surface-variant: "#3D3D3D"
  on-surface-muted: "#6E6E6E"
  surface-container-low: "#FAFAFA"
  surface-container: "#F3F3F3"
  outline: "#E7E7E7"
  outline-variant: "#CFCFCF"
  primary: "#FF584A"
  on-primary: "#000000"
  secondary: "#004232"
  tertiary: "#B5E9CA"
typography:
  headline-display:
    fontFamily: TWK Lausanne
    fontSize: 102px
    fontWeight: 300
    lineHeight: 0.9
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: TWK Lausanne
    fontSize: 54px
    fontWeight: 300
    lineHeight: 1
    letterSpacing: -0.02em
  headline-md:
    fontFamily: TWK Lausanne
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.2
  headline-sm:
    fontFamily: TWK Lausanne
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.2
  title-lg:
    fontFamily: TWK Lausanne
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.5
  body-md:
    fontFamily: TWK Lausanne
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.5
    letterSpacing: 0.02em
  body-sm:
    fontFamily: TWK Lausanne
    fontSize: 13px
    fontWeight: 300
    lineHeight: 1.5
    letterSpacing: 0.02em
  caption:
    fontFamily: TWK Lausanne
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.75
  label-lg:
    fontFamily: TWK Lausanne
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: TWK Lausanne
    fontSize: 14px
    fontWeight: 500
  label-sm:
    fontFamily: TWK Lausanne
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: TWK Lausanne
    fontSize: 48px
    fontWeight: 300
    lineHeight: 0.9
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: TWK Lausanne
    fontSize: 30px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
rounded:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 64px
  xl: 100px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 14px
  lg: 32px
  xl: 40px
  gutter: 8px
  section: 80px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 0px 16px
    height: 44px
  button-primary-hover:
    backgroundColor: "{colors.on-surface-muted}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 8px 24px
  input-field:
    textColor: "#646F79"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.surface-container}"
---

# Asana Design System

## Overview

Asana describes itself as: “Work management software for teams and AI agents. Plan, automate, and execute critical workflows together.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#0D0D0D)** text, and **Red (#FF584A)** as the main accent.

Type is set in **TWK Lausanne**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [asana.com](https://asana.com/) on October 29, 2026 at 1440×900 and 390×844 from 446 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #FF453E, #F481F4.

- **White (#FFFFFF):** Page background, seen 17 times. Token `background`, CSS `--lightmode-accent-white`.
- **Charcoal (#0D0D0D):** Primary text and headings, seen 66 times. Token `on-surface`, CSS `--black-1000`.
- **Graphite (#3D3D3D):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Slate (#6E6E6E):** Muted text and metadata, seen 11 times. Token `on-surface-muted`, CSS `--lightmode-link-text-weak-hover`.
- **Snow (#FAFAFA):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Mist (#F3F3F3):** Cards and panels, seen 21 times. Token `surface-container`, CSS `--lightmode-accent-gray-light`.
- **Mist (#E7E7E7):** Borders and dividers, seen 6 times. Token `outline`.
- **Silver (#CFCFCF):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Red (#FF584A):** Brand color in the logo, seen 1 time. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Deep Teal (#004232):** Accent (CSS variable). Token `secondary`.
- **Light Green (#B5E9CA):** Accent (CSS variable). Token `tertiary`.

## Typography

**TWK Lausanne** carries the whole interface. Fallback stack: `TWK Lausanne, Helvetica Neue, Helvetica, sans-serif`.

- **headline-display:** TWK Lausanne 102px at weight 300, line height 0.9, tracking -0.025em (48px on mobile). Page title (h1).
- **headline-lg:** TWK Lausanne 54px at weight 300, line height 1, tracking -0.02em (30px on mobile). Section headings (h2).
- **headline-md:** TWK Lausanne 30px at weight 400, line height 1.2. Sub-section headings.
- **headline-sm:** TWK Lausanne 24px at weight 500, line height 1.2. Card and feature titles.
- **title-lg:** TWK Lausanne 22px at weight 500, line height 1.5. Small titles.
- **body-md:** TWK Lausanne 16px at weight 300, line height 1.5, tracking 0.02em. Body text.
- **body-sm:** TWK Lausanne 13px at weight 300, line height 1.5, tracking 0.02em. Secondary and small text.
- **caption:** TWK Lausanne 12px at weight 400, line height 1.75. Captions and fine print.
- **label-lg:** TWK Lausanne 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** TWK Lausanne 14px at weight 500. Buttons, navigation and labels.
- **label-sm:** TWK Lausanne 13px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (79% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 14px, lg 32px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 1px, 200px, 300px, 350px, 400px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#FAFAFA → #F3F3F3) and hairline rings:

- `rgb(13, 13, 13) 0px 0px 0px 1px inset`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **xs (4px):** 84 elements.
- **xl (100px):** 48 elements.
- **sm (8px):** 40 elements.
- **lg (64px):** 20 elements.
- **full (9999px):** 16 elements.
- **md (10px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #0D0D0D fill, #FFFFFF text, 14px/500, 100px radius, padding 0px 16px.
- **button-primary-hover:** background #6E6E6E, text #FFFFFF on hover.
- **button-ghost (“Products”):** transparent fill, #0D0D0D text, 14px/500, 100px radius, padding 8px 24px.
- **input-field:** transparent fill, #646F79 text, 16px/400, padding 0px.
- **link:** transparent fill, #F3F3F3 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAFAFA, #F3F3F3.
- Do keep text in 3 levels: #0D0D0D, #3D3D3D, #6E6E6E.
- Do use #FF584A as the brand accent: header, logo and key highlights.
- Do set headlines in TWK Lausanne with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 14px, 32px).
- Do use 4px corners on most elements; larger surfaces also use 100px, 8px and 64px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond TWK Lausanne.
- Don't use #FF584A for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.15s, 0.25s.

- **Easing:** `ease`, `linear`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/asana.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
