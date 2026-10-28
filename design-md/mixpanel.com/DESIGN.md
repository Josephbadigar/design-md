---
version: alpha
name: Mixpanel
description: "Light monochrome interface measured from mixpanel.com: Garnett Medium type with Garnett Regular, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1F2023"
  on-background: "#1F2023"
  on-surface-variant: "#2A2A2F"
  on-surface-muted: "#626266"
  on-surface-subtle: "#8F8F91"
  surface-container-low: "#FAFAFA"
  surface-container: "#F6F6F6"
  surface-container-high: "#FBEBE7"
  overlay: "#00000012"
  overlay-strong: "#FFFFFF1A"
  outline: "#EAEAEA"
  outline-variant: "#E9E9E9"
  primary: "#1F2023"
  on-primary: "#0000EE"
  secondary: "#C6B7FF"
  tertiary: "#7856FF"
  error: "#E34F2F"
typography:
  headline-display:
    fontFamily: Garnett Medium
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Garnett Regular
    fontSize: 42px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0.02em
  headline-md:
    fontFamily: Garnett Medium
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Garnett Regular
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0.02em
  title-lg:
    fontFamily: Garnett Medium
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.2
  body-md:
    fontFamily: Garnett Regular
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.02em
  body-lg:
    fontFamily: Garnett Medium
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0.02em
  body-sm:
    fontFamily: sans-serif
    fontSize: 12px
    fontWeight: 400
  caption:
    fontFamily: Garnett Regular
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.68
    letterSpacing: 0.02em
  label-md:
    fontFamily: Garnett Medium
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1
  label-sm:
    fontFamily: Garnett Medium
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1
rounded:
  sm: 4px
  md: 100px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 32px
  xl: 40px
  gutter: 8px
  section: 160px
  margin: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 4px 6px 4px 14px
    height: 28px
  button-primary-hover:
    backgroundColor: "#1F2023CC"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "#000000"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 8px 16px 40px 16px
    height: 69px
  button-outline-hover:
    backgroundColor: "#F4F3FF"
    textColor: "{colors.on-surface}"
  button-ghost:
    backgroundColor: "{colors.surface-container}"
    textColor: "#000000"
    typography: "{typography.body-sm}"
    rounded: 10px
    padding: 10px 12px
    height: 39px
  link:
    textColor: "{colors.primary}"
---

# Mixpanel Design System

## Overview

Mixpanel describes itself as: “Mixpanel is the product intelligence platform for the AI era, combining analytics, session replay, experiments, feature flags, and AI-powered insights.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1F2023)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Garnett Medium** and **Garnett Regular**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 4px.

Measured from [mixpanel.com](https://mixpanel.com/home/) on October 21, 2026 at 1440×900 and 390×844 from 307 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles, plus gradient stops #C956FF, #DAD0FF, #A993FF, #FF834E.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`.
- **Charcoal (#1F2023):** Primary text and headings, seen 15 times. Token `on-surface`.
- **Graphite (#2A2A2F):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Slate (#626266):** Muted text and metadata, seen 6 times. Token `on-surface-muted`.
- **Gray (#8F8F91):** Subtle text and placeholders, seen 16 times. Token `on-surface-subtle`.
- **Snow (#FAFAFA):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **Snow (#F6F6F6):** Cards and panels, seen 2 times. Token `surface-container`.
- **Pale Red (#FBEBE7):** Hover and pressed fills, seen 2 times. Token `surface-container-high`.
- **Near Black 7% (#00000012):** Translucent fill for cards and controls, seen 5 times. Token `overlay`.
- **White 10% (#FFFFFF1A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Mist (#EAEAEA):** Borders and dividers, seen 9 times. Token `outline`.
- **Mist (#E9E9E9):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Charcoal (#1F2023):** Primary buttons and calls to action, seen 28 times. Token `primary`.
- **Vivid Indigo (#0000EE):** Text and icons on primary. Token `on-primary`.
- **Light Violet (#C6B7FF):** Brand color in logos and imagery, seen 7 times. Token `secondary`.
- **Violet (#7856FF):** Accent, seen 3 times. Token `tertiary`.
- **Red (#E34F2F):** Errors and destructive states, seen 3 times. Token `error`.

## Typography

**Garnett Medium**, **Garnett Regular** and **sans-serif** share the interface. Fallback stack: `Garnett Medium, Garnett Medium Placeholder, sans-serif`. Other loaded fonts: ABC Arizona Text Light Italic, Apercu Pro Medium, Garnett Regular Placeholder, Garnett Medium Placeholder.

- **headline-display:** Garnett Medium 48px at weight 400, line height 1.2, tracking -0.02em. Page title (h1).
- **headline-lg:** Garnett Regular 42px at weight 400, line height 1, tracking 0.02em. Section headings (h2).
- **headline-md:** Garnett Medium 28px at weight 400, line height 1.2, tracking -0.01em. Sub-section headings.
- **headline-sm:** Garnett Regular 24px at weight 400, line height 1, tracking 0.02em. Card and feature titles.
- **title-lg:** Garnett Medium 22px at weight 400, line height 1.2. Small titles.
- **body-md:** Garnett Regular 14px at weight 400, line height 1.5, tracking 0.02em. Body text.
- **body-lg:** Garnett Medium 16px at weight 400, line height 1.6, tracking 0.02em. Lead paragraphs.
- **body-sm:** sans-serif 12px at weight 400. Secondary and small text.
- **caption:** Garnett Regular 10px at weight 400, line height 1.68, tracking 0.02em. Captions and fine print.
- **label-md:** Garnett Medium 16px at weight 500, line height 1. Buttons, navigation and labels.
- **label-sm:** Garnett Medium 12px at weight 500, line height 1. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 43% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 10px, lg 32px, xl 40px.
- **Sections:** 160px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 767.98px, 807.98px, 808px, 1023.98px, 1199.98px, 1200px, 1439.98px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FAFAFA → #F6F6F6 → #FBEBE7) and #EAEAEA borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 248 elements.
- **md (100px):** 36 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started Free”):** #1F2023 fill, #0000EE text, 12px/400, 100px radius, padding 4px 6px 4px 14px.
- **button-primary-hover:** background #1F2023CC, text #0000EE on hover.
- **button-outline (“Mixpanel AI”):** #FFFFFF fill, #000000 text, 16px/500, padding 8px 16px 40px 16px.
- **button-outline-hover:** background #F4F3FF, text #1F2023 on hover.
- **button-ghost (“Want me to find the root cause?”):** #F6F6F6 fill, #000000 text, 12px/400, 10px radius, padding 10px 12px, border 1px solid #E9E9E9.
- **link:** transparent fill, #1F2023 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAFAFA, #F6F6F6, #FBEBE7.
- Do keep text in 4 levels: #1F2023, #2A2A2F, #626266, #8F8F91.
- Do let contrast carry emphasis; primary actions use #1F2023 on #FFFFFF.
- Do set headlines in Garnett Medium with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 10px, 32px).
- Do use 4px corners on most elements; larger surfaces also use 100px.
- Don't use #8F8F91 for body text; it reaches 3.2:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Garnett Medium, Garnett Regular and sans-serif.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.15s, 0.4s. Longer ambient animations run 2.2s, 0.7s, 1.1s.

- **Easing:** `ease`, `ease-out`, `linear`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mixpanel.com/), the free DESIGN.md generator.
