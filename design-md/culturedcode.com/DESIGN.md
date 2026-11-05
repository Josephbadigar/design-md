---
version: alpha
name: Cultured Code
description: "Light monochrome interface measured from culturedcode.com: system-ui type, tonal surfaces and 6px corners."
colors:
  background: "#F2F5F7"
  surface: "#F2F5F7"
  on-surface: "#303336"
  on-background: "#303336"
  on-surface-variant: "#44474B"
  on-surface-muted: "#8E9196"
  on-surface-subtle: "#8792A1"
  surface-container-low: "#ECEEF0"
  surface-container: "#FFFFFF"
  outline: "#DFE3E8"
  primary: "#303336"
  on-primary: "#FFFFFF"
  secondary: "#5C9CF5"
typography:
  headline-display:
    fontFamily: system-ui
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1
  headline-lg:
    fontFamily: system-ui
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.25
  body-md:
    fontFamily: system-ui
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.2
  body-lg:
    fontFamily: system-ui
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.2
  body-sm:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.2
  label-md:
    fontFamily: system-ui
    fontSize: 15px
    fontWeight: 600
    lineHeight: 1.6
  label-sm:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.2
  headline-lg-mobile:
    fontFamily: system-ui
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.25
rounded:
  sm: 3px
  md: 6px
  lg: 12.8px
  xl: 18px
spacing:
  xs: 2px
  sm: 6.5px
  md: 12.8px
  lg: 18px
  xl: 36px
  gutter: 16px
components:
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px
  input-field:
    backgroundColor: "{colors.surface-container}"
    textColor: "#000000"
    rounded: 6.4px
    padding: 8px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.xl}"
    padding: 18px
  link:
    textColor: "#000F2475"
---

# Cultured Code Design System

## Overview

Cultured Code describes itself as: “Things is the award-winning personal task manager that helps you plan your day, manage your projects, and make real progress toward your goals.” The interface is light, built on **Snow (#F2F5F7)** with **Cool Graphite (#303336)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **system-ui**. Headlines run large; body text is 15px. Depth comes from soft drop shadows. Corners are mostly 6px.

Measured from [culturedcode.com](https://culturedcode.com/things/) on November 4, 2026 at 1440×900 and 390×844 from 247 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Snow (#F2F5F7):** Page background, seen 5 times. Token `background`.
- **Cool Graphite (#303336):** Primary text and headings, seen 41 times. Token `on-surface`.
- **Cool Graphite (#44474B):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Cool Gray (#8E9196):** Muted text and metadata, seen 16 times. Token `on-surface-muted`.
- **Blue (#8792A1):** Subtle text and placeholders, seen 7 times. Token `on-surface-subtle`.
- **Mist (#ECEEF0):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **White (#FFFFFF):** Cards and panels, seen 9 times. Token `surface-container`.
- **Cool Mist (#DFE3E8):** Borders and dividers, seen 1 time. Token `outline`.
- **Cool Graphite (#303336):** Primary actions (the main text color; the palette is monochrome), seen 46 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#5C9CF5):** Accent in text, fills and borders, seen 2 times. Token `secondary`.

## Typography

**system-ui** carries the whole interface. Fallback stack: `ui-sans-serif, -apple-system, BlinkMacSystemFont, Roboto`.

- **headline-display:** system-ui 36px at weight 700, line height 1. Page title (h1).
- **headline-lg:** system-ui 24px at weight 400, line height 1.25 (20px on mobile). Section headings (h2).
- **body-md:** system-ui 15px at weight 400, line height 1.2. Body text.
- **body-lg:** system-ui 18px at weight 400, line height 1.2. Lead paragraphs.
- **body-sm:** system-ui 13px at weight 400, line height 1.2. Secondary and small text.
- **label-md:** system-ui 15px at weight 600, line height 1.6. Buttons, navigation and labels.
- **label-sm:** system-ui 13px at weight 700, line height 1.2. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 4% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6.5px, md 12.8px, lg 18px, xl 36px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 340px, 420px, 480px, 520px, 600px, 620px, 720px, 734px, 739px, 740px, 899px, 972px, 1002px, 1106px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 2px 8px 0px, rgba(0, 0, 0, 0.1) 0px 0px 2px 0px`

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 52 elements.
- **sm (3px):** 32 elements.
- **lg (12.8px):** 32 elements.
- **xl (18px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Things”):** transparent fill, #303336 text, 15px/600, 6px radius, padding 0px.
- **input-field (“me@example.com”):** #FFFFFF fill, #000000 text, 16px/400, 6.4px radius, padding 8px, border 1px solid #DFE3E8.
- **card:** #F2F5F7 fill, #303336 text, 18px/400, 18px radius, padding 18px.
- **link:** transparent fill, #000F2475 text, padding 0px.

## Do's and Don'ts

- Do use #F2F5F7 for the page and lift surfaces in small steps: #ECEEF0, #FFFFFF.
- Do keep text in 4 levels: #303336, #44474B, #8E9196, #8792A1.
- Do let contrast carry emphasis; primary actions use #303336 on #F2F5F7.
- Do reuse the measured spacing steps (6.5px, 12.8px, 18px).
- Do use 6px corners on most elements; larger surfaces also use 3px, 12.8px and 18px.
- Don't use #8E9196 for body text; it reaches 2.89:1 on #F2F5F7. Keep it for large text or metadata.
- Don't use #8792A1 for body text; it reaches 2.88:1 on #F2F5F7. Keep it for large text or metadata.
- Don't introduce new font families beyond system-ui.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.1s.

## Motion

Interface transitions are quick: 0.1s.

- **Easing:** `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/culturedcode.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
