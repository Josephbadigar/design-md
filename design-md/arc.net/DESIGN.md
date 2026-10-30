---
version: alpha
name: Arc
description: "Dark monochrome interface measured from arc.net: Exposure VAR type with ABC Oracle, tonal surfaces and pill-shaped controls."
colors:
  background: "#0B0B0B"
  surface: "#0B0B0B"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#7F7F7F"
  on-surface-muted: "#727272"
  surface-container-low: "#000000"
  overlay: "#00000012"
  overlay-strong: "#0000009E"
  primary: "#FFFFFF"
  on-primary: "#000000"
  secondary: "#5B45E0"
  tertiary: "#C86B00"
typography:
  headline-display:
    fontFamily: Exposure VAR
    fontSize: 76px
    fontWeight: 600
    lineHeight: 1.13
    letterSpacing: -0.032em
  headline-lg:
    fontFamily: Exposure VAR
    fontSize: 64px
    fontWeight: 600
    lineHeight: 1.06
    letterSpacing: -0.03em
  headline-md:
    fontFamily: ABC Oracle
    fontSize: 22px
    fontWeight: 350
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-md:
    fontFamily: ABC Oracle
    fontSize: 17px
    fontWeight: 350
    lineHeight: 1.41
    letterSpacing: -0.03em
  body-lg:
    fontFamily: ABC Oracle
    fontSize: 20px
    fontWeight: 350
    lineHeight: 1.42
    letterSpacing: -0.02em
  body-sm:
    fontFamily: ABC Oracle
    fontSize: 16px
    fontWeight: 350
  caption:
    fontFamily: system-ui
    fontSize: 13px
    fontWeight: 350
    lineHeight: 1.23
  code:
    fontFamily: ABC Favorit Mono
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0.14em
  headline-display-mobile:
    fontFamily: Exposure VAR
    fontSize: 52px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.03em
  headline-md-mobile:
    fontFamily: ABC Oracle
    fontSize: 20px
    fontWeight: 350
    lineHeight: 1.2
    letterSpacing: -0.02em
rounded:
  sm: 3px
  md: 10px
  lg: 12px
  xl: 60px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 47px
  gutter: 24px
  section: 158.4px
components:
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 0px 24px
    height: 60px
  button-ghost:
    textColor: "{colors.on-primary}"
    rounded: "{rounded.lg}"
    padding: 0px 24px
  link:
    textColor: "{colors.on-primary}"
---

# Arc Design System

## Overview

Arc describes itself as: “Arc is sunsetting on December 22, 2026. What happens next and the transition to Dia.” The interface is dark, built on **Near Black (#0B0B0B)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Exposure VAR** and **ABC Oracle**, with **ABC Favorit Mono** for code. Headlines run large with tight negative tracking; body text is 17px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [arc.net](https://arc.net/) on October 29, 2026 at 1440×900 and 390×844 from 201 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Near Black (#0B0B0B):** Page background, seen 4 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 17 times. Token `on-surface`, CSS `--colors-lowContrast`.
- **Slate (#7F7F7F):** Secondary text, seen 10 times. Token `on-surface-variant`.
- **Slate (#727272):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Near Black (#000000):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`, CSS `--colors-highContrast`.
- **Near Black 7% (#00000012):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Near Black 62% (#0000009E):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White (#FFFFFF):** Primary actions (the main text color; the palette is monochrome), seen 28 times. Token `primary`, CSS `--colors-lowContrast`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Indigo (#5B45E0):** Accent in text, fills and borders, seen 3 times. Token `secondary`.
- **Orange (#C86B00):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.

## Typography

**Exposure VAR**, **ABC Oracle**, **system-ui** and **ABC Favorit Mono** (monospace) share the interface. Fallback stack: `Exposure VAR, Iowan Old Style, Georgia, serif`. Other loaded fonts: Marlin.

- **headline-display:** Exposure VAR 76px at weight 600, line height 1.13, tracking -0.032em (52px on mobile). Page title (h1).
- **headline-lg:** Exposure VAR 64px at weight 600, line height 1.06, tracking -0.03em. Section headings (h2).
- **headline-md:** ABC Oracle 22px at weight 350, line height 1.2, tracking -0.02em (20px on mobile). Sub-section headings.
- **body-md:** ABC Oracle 17px at weight 350, line height 1.41, tracking -0.03em. Body text.
- **body-lg:** ABC Oracle 20px at weight 350, line height 1.42, tracking -0.02em. Lead paragraphs.
- **body-sm:** ABC Oracle 16px at weight 350. Secondary and small text.
- **caption:** system-ui 13px at weight 350, line height 1.23. Captions and fine print.
- **code:** ABC Favorit Mono 13px at weight 400, line height 1.43, tracking 0.14em, uppercase. Code and technical values.

## Layout

Spacing does not follow a strict grid: 62% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 47px.
- **Sections:** 158.4px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Breakpoints:** 640px, 641px, 799px, 800px, 1099px, 1100px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#000000):

- `rgba(0, 0, 0, 0.12) 0px 0px 0px 0.5px inset`
- `rgb(0, 0, 0) 0px 0px 0px 1px`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0.25) 0px 0px 2px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 20 elements.
- **lg (12px):** 12 elements.
- **sm (3px):** 8 elements.
- **md (10px):** 4 elements.
- **xl (60px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Download Dia”):** #0B0B0B fill, #FFFFFF text, 18px/350, 12px radius, padding 0px 24px.
- **button-ghost (“Download Dia”):** transparent fill, #000000 text, 18px/350, 12px radius, padding 0px 24px, shadow `rgb(0, 0, 0) 0px 0px 0px 1px`.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #0B0B0B for the page and lift surfaces in small steps: #000000.
- Do keep text in 3 levels: #FFFFFF, #7F7F7F, #727272.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #0B0B0B.
- Do set headlines in Exposure VAR with tight tracking (-0.032em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 12px corners.
- Don't use #727272 for body text; it reaches 4.09:1 on #0B0B0B. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Exposure VAR, ABC Oracle, system-ui and ABC Favorit Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.45s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.2s, 0.45s.

- **Easing:** `ease`, `cubic-bezier(0.16, 1, 0.3, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/arc.net/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
