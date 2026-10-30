---
version: alpha
name: Savee
description: "Light monochrome interface measured from savee.com: saveeFont type, tonal surfaces and 16px corners."
colors:
  background: "#F3F3F3"
  surface: "#F3F3F3"
  on-surface: "#404040"
  on-background: "#404040"
  on-surface-strong: "#050505"
  on-surface-variant: "#464646"
  on-surface-muted: "#A3A3A3"
  surface-container-low: "#FDFDFDE6"
  surface-container: "#FDFDFD"
  surface-container-high: "#E4E4E4"
  surface-container-highest: "#DADADA"
  primary: "#050505"
  on-primary: "#FDFDFD"
  secondary: "#22C55E"
typography:
  headline-display:
    fontFamily: saveeFont
    fontSize: 96px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: saveeFont
    fontSize: 65px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.025em
  body-md:
    fontFamily: saveeFont
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: saveeFont
    fontSize: 21px
    fontWeight: 500
    lineHeight: 1.29
    letterSpacing: -0.03em
  label-md:
    fontFamily: saveeFont
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: -0.01em
  label-sm:
    fontFamily: saveeFont
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.01em
  headline-display-mobile:
    fontFamily: saveeFont
    fontSize: 45.5px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.035em
  headline-lg-mobile:
    fontFamily: saveeFont
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.025em
rounded:
  sm: 16px
  md: 17.24px
  lg: 32px
spacing:
  xs: 2px
  sm: 6px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 12px
  section: 212px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    padding: 20px 40px
    height: 56px
  button-outline:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.headline-display}"
    rounded: "{rounded.md}"
    padding: 0px
    height: 90px
  button-secondary:
    backgroundColor: "{colors.surface-container-highest}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    padding: 20px 40px
    height: 56px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    padding: 16px 20px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Savee Design System

## Overview

Savee describes itself as: “Savee is a curated place for visual inspiration. Discover references chosen by designers, collect what matters, and build a sharper eye without ads or clutter.” The interface is light, built on **Mist (#F3F3F3)** with **Graphite (#404040)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **saveeFont**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 16px.

Measured from [savee.com](https://savee.com/) on October 29, 2026 at 1440×900 and 390×844 from 332 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Mist (#F3F3F3):** Page background. Token `background`.
- **Graphite (#404040):** Primary text and headings, seen 32 times. Token `on-surface`.
- **Near Black (#050505):** Headings and emphasis, seen 28 times. Token `on-surface-strong`.
- **Graphite (#464646):** Secondary text, seen 25 times. Token `on-surface-variant`.
- **Gray (#A3A3A3):** Muted text and metadata, seen 11 times. Token `on-surface-muted`.
- **Snow 90% (#FDFDFDE6):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#FDFDFD):** Cards and panels, seen 6 times. Token `surface-container`.
- **Mist (#E4E4E4):** Hover and pressed fills, seen 9 times. Token `surface-container-high`.
- **Silver (#DADADA):** Highest raised elements, seen 9 times. Token `surface-container-highest`.
- **Near Black (#050505):** Primary buttons and calls to action, seen 50 times. Token `primary`.
- **Snow (#FDFDFD):** Text and icons on primary. Token `on-primary`.
- **Green (#22C55E):** Accent, seen 1 time. Token `secondary`, CSS `--color-green-500`.

## Typography

**saveeFont** carries the whole interface. Fallback stack: `saveeFont, saveeFont Fallback`.

- **headline-display:** saveeFont 96px at weight 500, line height 1, tracking -0.035em (45.5px on mobile). Page title (h1).
- **headline-lg:** saveeFont 65px at weight 500, line height 1.05, tracking -0.025em (36px on mobile). Section headings (h2).
- **body-md:** saveeFont 14px at weight 400, line height 1.43. Body text.
- **body-lg:** saveeFont 21px at weight 500, line height 1.29, tracking -0.03em. Lead paragraphs.
- **label-md:** saveeFont 16px at weight 400, line height 1.38, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** saveeFont 14px at weight 500, line height 1, tracking -0.01em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 69% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 12px, lg 20px, xl 40px.
- **Sections:** 212px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 600px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 10px 15px -3px, rgba(0, 0, 0, 0.1) 0px 4px 6px -4px`

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **sm (16px):** 24 elements.
- **md (17.24px):** 12 elements.
- **lg (32px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Join for free”):** #050505 fill, #FDFDFD text, 16px/500, 3.35544e+07px radius, padding 20px 40px.
- **button-outline (“Show another save”):** #E4E4E4 fill, #050505 text, 95.76px/500, 17.2368px radius, padding 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`.
- **button-secondary (“See plans”):** #DADADA fill, #464646 text, 16px/400, 3.35544e+07px radius, padding 20px 40px.
- **button-ghost (“Log in”):** transparent fill, #404040 text, 14px/400, 3.35544e+07px radius, padding 16px 20px.
- **link:** transparent fill, #464646 text, padding 0px.

## Do's and Don'ts

- Do use #F3F3F3 for the page and lift surfaces in small steps: #FDFDFDE6, #FDFDFD, #E4E4E4, #DADADA.
- Do keep text in 4 levels: #404040, #050505, #464646, #A3A3A3.
- Do let contrast carry emphasis; primary actions use #050505 on #F3F3F3.
- Do set headlines in saveeFont with tight tracking (-0.035em).
- Do reuse the measured spacing steps (6px, 12px, 20px).
- Do use 16px corners on most elements; larger surfaces also use 17.24px and 32px.
- Don't use #A3A3A3 for body text; it reaches 2.27:1 on #F3F3F3. Keep it for large text or metadata.
- Don't introduce new font families beyond saveeFont.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.15s, 0.18s, 0.6s, 0.3s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`, `cubic-bezier(0.16, 1, 0.3, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/savee.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
