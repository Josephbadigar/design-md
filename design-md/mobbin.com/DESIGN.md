---
version: alpha
name: Mobbin
description: "Light monochrome interface measured from mobbin.com: saans type, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#141414"
  on-background: "#141414"
  on-surface-variant: "#707070"
  on-surface-muted: "#ADADAD"
  surface-container-low: "#FFFFFFF5"
  surface-container: "#FFFFFFE6"
  overlay: "#40404014"
  overlay-strong: "#4040400F"
  primary: "#141414"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: saans
    fontSize: 80px
    fontWeight: 652
    lineHeight: 1
    letterSpacing: -0.007em
  headline-lg:
    fontFamily: saans
    fontSize: 44px
    fontWeight: 652
    lineHeight: 1.09
    letterSpacing: -0.009em
  headline-md:
    fontFamily: saans
    fontSize: 24px
    fontWeight: 652
    lineHeight: 1.25
  headline-sm:
    fontFamily: saans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.3
  body-md:
    fontFamily: saans
    fontSize: 16px
    fontWeight: 456
    lineHeight: 1.38
    letterSpacing: 0.013em
  body-sm:
    fontFamily: saans
    fontSize: 14px
    fontWeight: 456
    lineHeight: 1.43
    letterSpacing: 0.014em
  caption:
    fontFamily: saans
    fontSize: 12px
    fontWeight: 456
    lineHeight: 1.33
    letterSpacing: 0.017em
  label-md:
    fontFamily: saans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: saans
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
    letterSpacing: 0.014em
  headline-display-mobile:
    fontFamily: saans
    fontSize: 40px
    fontWeight: 652
    lineHeight: 1
    letterSpacing: -0.015em
  headline-lg-mobile:
    fontFamily: saans
    fontSize: 12px
    fontWeight: 456
    lineHeight: 1.33
    letterSpacing: 0.017em
rounded:
  sm: 3.33px
  md: 24px
  lg: 32px
  full: 9999px
spacing:
  base: 4px
  xs: 2px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 8px
  section: 80px
  margin: 20px
  container: 1728px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 0px 16px
    height: 44px
  button-primary-hover:
    backgroundColor: "#262626"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 0px 12px
    height: 36px
  button-outline-hover:
    backgroundColor: "{colors.background}"
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 0px 12px
  link:
    textColor: "{colors.on-primary}"
---

# Mobbin Design System

## Overview

Mobbin describes itself as: “Save hours of UI & UX research with our library of 621,500+ fully searchable mobile & web app screenshots.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#141414)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **saans**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [mobbin.com](https://mobbin.com/) on October 21, 2026 at 1440×900 and 390×844 from 299 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 12 times. Token `background`, CSS `--color-overscroll-canvas`.
- **Charcoal (#141414):** Primary text and headings, seen 40 times. Token `on-surface`.
- **Slate (#707070):** Secondary text, seen 10 times. Token `on-surface-variant`, CSS `--color-text-secondary`.
- **Gray (#ADADAD):** Muted text and metadata, seen 10 times. Token `on-surface-muted`.
- **White 96% (#FFFFFFF5):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **White 90% (#FFFFFFE6):** Cards and panels, seen 1 time. Token `surface-container`.
- **Graphite 8% (#40404014):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **Graphite 6% (#4040400F):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Charcoal (#141414):** Primary buttons and calls to action, seen 83 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**saans** carries the whole interface. Fallback stack: `saans, saans Fallback`. Other loaded fonts: saans Fallback.

- **headline-display:** saans 80px at weight 652, line height 1, tracking -0.007em (40px on mobile). Page title (h1).
- **headline-lg:** saans 44px at weight 652, line height 1.09, tracking -0.009em (12px on mobile). Section headings (h2).
- **headline-md:** saans 24px at weight 652, line height 1.25. Sub-section headings.
- **headline-sm:** saans 20px at weight 600, line height 1.3. Card and feature titles.
- **body-md:** saans 16px at weight 456, line height 1.38, tracking 0.013em. Body text.
- **body-sm:** saans 14px at weight 456, line height 1.43, tracking 0.014em. Secondary and small text.
- **caption:** saans 12px at weight 456, line height 1.33, tracking 0.017em. Captions and fine print.
- **label-md:** saans 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** saans 14px at weight 600, line height 1.43, tracking 0.014em. Small labels and badges.

## Layout

Spacing follows a 4px grid: 96% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 2px, sm 8px, md 12px, lg 20px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1728px.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 560px, 720px, 768px, 769px, 840px, 980px, 1024px, 1199px, 1200px, 1201px, 1280px, 1440px, 1536px, 1728px, 1920px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#FFFFFFF5 → #FFFFFFE6) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.946552 0.0000431836 0.0000188947 / 0.08) 0px 0px 0px 1px inset`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **lg (32px):** 66 elements.
- **full (9999px):** 44 elements.
- **md (24px):** 12 elements.
- **sm (3.33px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Join for free”):** #141414 fill, #FFFFFF text, 16px/600, 9999px radius, padding 0px 16px.
- **button-primary-hover:** background #262626, text #FFFFFF on hover.
- **button-outline (“Accept”):** #FFFFFFF5 fill, #141414 text, 14px/600, 9999px radius, padding 0px 12px.
- **button-outline-hover:** background #FFFFFFE0, text #141414 on hover.
- **button-ghost (“Deny”):** transparent fill, #FFFFFF text, 14px/600, 9999px radius, padding 0px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.946552 0.0000431836 0.0000188947 / 0.08) 0px 0px 0px 1px inset`.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FFFFFFF5, #FFFFFFE6.
- Do keep text in 3 levels: #141414, #707070, #ADADAD.
- Do let contrast carry emphasis; primary actions use #141414 on #FFFFFF.
- Do set headlines in saans with tight tracking (-0.007em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 32px corners.
- Don't use #ADADAD for body text; it reaches 2.2:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond saans.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.2s.

- **Easing:** `cubic-bezier(0, 0, 0.2, 1)`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mobbin.com/), the free DESIGN.md generator.
