---
version: alpha
name: FlutterFlow
description: "Light interface measured from flutterflow.io: Inter type, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FCFCFB"
  surface: "#FCFCFB"
  on-surface: "#1A1A1A"
  on-background: "#1A1A1A"
  on-surface-variant: "#3D3D3D"
  on-surface-muted: "#555555"
  on-surface-subtle: "#6B6B6B"
  surface-container-low: "#FFFFFF"
  surface-container: "#F5F5F5"
  surface-container-high: "#EFEFEF"
  surface-container-highest: "#EBEBEB"
  overlay: "#1A1A1A14"
  overlay-strong: "#FFFFFF99"
  outline: "#00000014"
  outline-variant: "#1A1A1A1F"
  primary: "#0A68E0"
  on-primary: "#FFFFFF"
  secondary: "#1B519F"
  tertiary: "#177245"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 66px
    fontWeight: 600
    lineHeight: 1.03
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: 510
    lineHeight: 1.08
    letterSpacing: -0.022em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.45
    letterSpacing: -0.012em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: -0.011em
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.55
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.55
  label-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 510
    lineHeight: 1.6
    letterSpacing: -0.011em
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 42px
    fontWeight: 600
    lineHeight: 1.05
    letterSpacing: -0.035em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 26px
    fontWeight: 510
    lineHeight: 1.2
    letterSpacing: -0.018em
rounded:
  xs: 6px
  sm: 8px
  md: 13px
  lg: 16px
  xl: 20px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 36px
  gutter: 8px
  section: 128px
  container: 1120px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 0px 14px
    height: 32px
  button-ghost:
    textColor: "{colors.on-surface-subtle}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 8px 10px 8px 12px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 16px 18px 56px 18px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 22px
    padding: 0px
  link:
    textColor: "{colors.on-surface-subtle}"
---

# FlutterFlow Design System

## Overview

FlutterFlow describes itself as: “Build an iPhone and Android app by describing it. Start with a first version in about five minutes, ask the agent for any change, and send it to the App Store and Google Play.” The interface is light, built on **Snow (#FCFCFB)** with **Charcoal (#1A1A1A)** text, and **Vivid Blue (#0A68E0)** as the main accent.

Type is set in **Inter**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [flutterflow.io](https://flutterflow.io/) on November 4, 2026 at 1440×900 and 390×844 from 346 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles.

- **Snow (#FCFCFB):** Page background, seen 3 times. Token `background`, CSS `--page`.
- **Charcoal (#1A1A1A):** Primary text and headings, seen 42 times. Token `on-surface`, CSS `--ink`.
- **Graphite (#3D3D3D):** Secondary text, seen 9 times. Token `on-surface-variant`, CSS `--ink-2`.
- **Slate (#555555):** Muted text and metadata, seen 3 times. Token `on-surface-muted`.
- **Slate (#6B6B6B):** Subtle text and placeholders, seen 57 times. Token `on-surface-subtle`, CSS `--muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`, CSS `--card`.
- **Snow (#F5F5F5):** Cards and panels, seen 6 times. Token `surface-container`, CSS `--app`.
- **Mist (#EFEFEF):** Hover and pressed fills, seen 2 times. Token `surface-container-high`, CSS `--p-widget`.
- **Mist (#EBEBEB):** Highest raised elements, seen 6 times. Token `surface-container-highest`, CSS `--p-fill`.
- **Charcoal 8% (#1A1A1A14):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **White 60% (#FFFFFF99):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Near Black 8% (#00000014):** Borders and dividers, seen 12 times. Token `outline`, CSS `--line-1`.
- **Charcoal 12% (#1A1A1A1F):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Vivid Blue (#0A68E0):** Brand accent (CSS variable), seen 3 times. Token `primary`, CSS `--accent`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#1B519F):** Accent (CSS variable). Token `secondary`.
- **Dark Teal (#177245):** Accent, seen 4 times. Token `tertiary`, CSS `--success`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, -apple-system, BlinkMacSystemFont, Segoe UI`.

- **headline-display:** Inter 66px at weight 600, line height 1.03, tracking -0.035em (42px on mobile). Page title (h1).
- **headline-lg:** Inter 48px at weight 510, line height 1.08, tracking -0.022em (26px on mobile). Section headings (h2).
- **headline-md:** Inter 20px at weight 400, line height 1.45, tracking -0.012em. Sub-section headings.
- **body-md:** Inter 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Inter 15px at weight 400, line height 1.6, tracking -0.011em. Lead paragraphs.
- **body-sm:** Inter 13px at weight 400, line height 1.55. Secondary and small text.
- **label-lg:** Inter 16px at weight 400, line height 1.55. Large buttons and tabs.
- **label-md:** Inter 15px at weight 510, line height 1.6, tracking -0.011em. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (79% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 36px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1120px.
- **Breakpoints:** 420px, 640px, 759.98px, 760px, 820px, 821px, 899.98px, 900px, 980px, 1023.98px, 1199.98px, 1279.98px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.08) 0px 0px 0px 1px, rgba(0, 0, 0, 0.22) 0px 18px 40px -22px`
- `rgba(0, 0, 0, 0.04) 0px 1px 2px 0px, rgba(0, 0, 0, 0.14) 0px 8px 24px -14px`
- `rgba(0, 0, 0, 0.08) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.04) 0px 1px 2px 0px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0.08) 0px 0px 0px 1px inset`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 84 elements.
- **xl (20px):** 26 elements.
- **sm (8px):** 24 elements.
- **md (13px):** 12 elements.
- **lg (16px):** 12 elements.
- **xs (6px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start building”):** #1A1A1A fill, #FFFFFF text, 13px/510, 999px radius, padding 0px 14px.
- **button-ghost (“Product”):** transparent fill, #6B6B6B text, 14px/400, 999px radius, padding 8px 10px 8px 12px.
- **input-field (“What should your app do?”):** transparent fill, #1A1A1A text, 16px/400, padding 16px 18px 56px 18px.
- **card:** #FFFFFF fill, #1A1A1A text, 16px/400, 22px radius, padding 0px, shadow `rgba(0, 0, 0, 0.04) 0px 1px 2px 0px, rgba(0, 0, 0, 0.14) 0px 8px 24px -14px`.
- **link:** transparent fill, #6B6B6B text, padding 0px.

## Do's and Don'ts

- Do use #FCFCFB for the page and lift surfaces in small steps: #FFFFFF, #F5F5F5, #EFEFEF, #EBEBEB.
- Do keep text in 4 levels: #1A1A1A, #3D3D3D, #555555, #6B6B6B.
- Do use #0A68E0 as the brand accent: header, logo and key highlights.
- Do set headlines in Inter with tight tracking (-0.035em).
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do make buttons and chips fully rounded (9999px); most other elements use 20px corners.
- Don't introduce new font families beyond Inter.
- Don't use #0A68E0 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.12s, 0.15s, 0.32s, 0.24s. Longer ambient animations run 1s, 1.05s.

- **Easing:** `cubic-bezier(0.25, 0.46, 0.45, 0.94)`, `ease`, `cubic-bezier(0.2, 0.8, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/flutterflow.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
