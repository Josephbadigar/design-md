---
version: alpha
name: Screen Studio
description: "Dark monochrome interface measured from screen.studio: system-ui type, tonal surfaces and pill-shaped controls."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#F5F5F7"
  on-background: "#F5F5F7"
  on-surface-variant: "#86868B"
  on-surface-muted: "#6E6E73"
  surface-container-low: "#111112"
  overlay: "#FFFFFF0D"
  overlay-strong: "#4D2FF557"
  primary: "#F5F5F7"
  on-primary: "#000000"
  secondary: "#4D2FF5"
typography:
  headline-display:
    fontFamily: system-ui
    fontSize: 72px
    fontWeight: 600
    lineHeight: 1.06
  headline-lg:
    fontFamily: system-ui
    fontSize: 56px
    fontWeight: 600
    lineHeight: 1.07
  headline-md:
    fontFamily: system-ui
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.08
  headline-sm:
    fontFamily: system-ui
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.14
  title-lg:
    fontFamily: system-ui
    fontSize: 21px
    fontWeight: 600
    lineHeight: 1.19
  body-md:
    fontFamily: system-ui
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.47
  body-lg:
    fontFamily: system-ui
    fontSize: 19px
    fontWeight: 500
    lineHeight: 1.42
  body-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  caption:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-lg:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.71
  label-sm:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1.33
  headline-display-mobile:
    fontFamily: system-ui
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: system-ui
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.13
rounded:
  md: 22.4px
  full: 9999px
spacing:
  sm: 8px
  md: 12px
  lg: 18px
  xl: 56px
  gutter: 8px
  section: 144px
components:
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 9.6px
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Screen Studio Design System

## Overview

Screen Studio describes itself as: “Screen recorder for macOS. Create engaging product demos, courses, tutorial and social media videos. Add automatic zoom on mouse actions, smooth mouse movement, and other powerful effects and animations. Designed for mac” The interface is dark, built on **Near Black (#000000)** with **Snow (#F5F5F7)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **system-ui**. Headlines run large; body text is 17px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [screen.studio](https://screen.studio/) on November 4, 2026 at 1440×900 and 390×844 from 433 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Near Black (#000000):** Page background, seen 12 times. Token `background`.
- **Snow (#F5F5F7):** Primary text and headings, seen 77 times. Token `on-surface`.
- **Gray (#86868B):** Secondary text, seen 49 times. Token `on-surface-variant`.
- **Slate (#6E6E73):** Muted text and metadata, seen 3 times. Token `on-surface-muted`.
- **Charcoal (#111112):** Raised areas one step from the page, seen 11 times. Token `surface-container-low`.
- **White 5% (#FFFFFF0D):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Vivid Indigo 34% (#4D2FF557):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Snow (#F5F5F7):** Primary actions (the main text color; the palette is monochrome), seen 81 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#4D2FF5):** Accent on large areas. Token `secondary`.

## Typography

**system-ui** carries the whole interface. Fallback stack: `BlinkMacSystemFont, -apple-system, SF Pro Display, SF Pro`. Other loaded fonts: Inter, Material Symbols Rounded.

- **headline-display:** system-ui 72px at weight 600, line height 1.06 (40px on mobile). Page title (h1).
- **headline-lg:** system-ui 56px at weight 600, line height 1.07 (32px on mobile). Section headings (h2).
- **headline-md:** system-ui 48px at weight 600, line height 1.08. Sub-section headings.
- **headline-sm:** system-ui 28px at weight 600, line height 1.14. Card and feature titles.
- **title-lg:** system-ui 21px at weight 600, line height 1.19. Small titles.
- **body-md:** system-ui 17px at weight 400, line height 1.47. Body text.
- **body-lg:** system-ui 19px at weight 500, line height 1.42. Lead paragraphs.
- **body-sm:** system-ui 14px at weight 400, line height 1.43. Secondary and small text.
- **caption:** system-ui 12px at weight 400, line height 1.33. Captions and fine print.
- **label-lg:** system-ui 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** system-ui 14px at weight 500, line height 1.71. Buttons, navigation and labels.
- **label-sm:** system-ui 12px at weight 600, line height 1.33. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 69% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 8px, md 12px, lg 18px, xl 56px.
- **Sections:** 144px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 734px, 884px, 1068px, 1600px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#111112):

- `rgba(255, 255, 255, 0.04) 0px 0px 0px 1px inset`
- `rgb(255, 255, 255) 0px 0px 0px 1px inset`
- `rgba(255, 255, 255, 0.28) 0px 0px 0px 1px inset`

A few raised panels add a soft drop shadow: `rgba(157, 139, 255, 0.5) 0px 0px 0px 1px inset, rgba(77, 47, 245, 0.22) 0px 10px 30px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 368 elements.
- **md (22.4px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“Explore”):** transparent fill, #F5F5F7 text, 16px/400, 9.6px radius, padding 0px.
- **link:** transparent fill, #86868B text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #111112.
- Do keep text in 3 levels: #F5F5F7, #86868B, #6E6E73.
- Do let contrast carry emphasis; primary actions use #F5F5F7 on #000000.
- Do reuse the measured spacing steps (8px, 12px, 18px).
- Do make buttons and chips fully rounded (9999px); most other elements use 22.4px corners.
- Don't use #6E6E73 for body text; it reaches 4.14:1 on #000000. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond system-ui.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.42s.

## Motion

Interface transitions are quick: 0.2s, 0.42s, 0.25s. Longer ambient animations run 1s.

- **Easing:** `ease`, `cubic-bezier(0.23, 1, 0.32, 1)`, `cubic-bezier(0.32, 0.72, 0, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/screen.studio/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
