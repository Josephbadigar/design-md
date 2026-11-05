---
version: alpha
name: draw.io
description: "Light interface measured from drawio.com: Inter type, vivid orange accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#475467"
  on-background: "#475467"
  on-surface-strong: "#101828"
  on-surface-variant: "#667085"
  on-surface-muted: "#A4A7AE"
  surface-container-low: "#F8F9FB"
  overlay: "#FFFFFF29"
  overlay-strong: "#FFFFFF0A"
  outline: "#E4E7EC"
  outline-variant: "#D0D5DD"
  primary: "#DC6803"
  on-primary: "#FFFFFF"
  secondary: "#F08705"
  tertiary: "#C65D03"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 60px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: -0.03em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.65
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.015em
  body-sm:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.4
  caption:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.7
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: -0.005em
  label-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.65
  label-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.65
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: -0.04em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: -0.03em
rounded:
  sm: 8px
  md: 10px
  lg: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 36px
  gutter: 8px
  section: 96px
  margin: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.caption}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
    height: 34px
  button-primary-hover:
    backgroundColor: "#C4520B"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 4px 12px
    height: 29px
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 11px 22px
    height: 48px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.caption}"
    rounded: "{rounded.sm}"
    padding: 0px 13.6px 0px 36px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.secondary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# draw.io Design System

## Overview

draw.io describes itself as: “Free diagramming application with 100M+ users. Store your data wherever you want—we can't access it.” The interface is light, built on **White (#FFFFFF)** with **Dark Blue (#475467)** text, and **Vivid Orange (#DC6803)** as the main accent.

Type is set in **Inter**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [drawio.com](https://www.drawio.com/) on November 4, 2026 at 1440×900 and 390×844 from 135 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **White (#FFFFFF):** Page background, seen 22 times. Token `background`, CSS `--ifm-background-surface-color`.
- **Dark Blue (#475467):** Primary text and headings, seen 26 times. Token `on-surface`, CSS `--ifm-navbar-link-color`.
- **Deep Blue (#101828):** Headings and emphasis, seen 17 times. Token `on-surface-strong`, CSS `--ifm-table-head-color`.
- **Blue (#667085):** Secondary text, seen 10 times. Token `on-surface-variant`.
- **Cool Gray (#A4A7AE):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Snow (#F8F9FB):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **White 16% (#FFFFFF29):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **White 4% (#FFFFFF0A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Cool Mist (#E4E7EC):** Borders and dividers, seen 18 times. Token `outline`, CSS `--dw-border`.
- **Cool Silver (#D0D5DD):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Vivid Orange (#DC6803):** Primary buttons and calls to action, seen 7 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Orange (#F08705):** Accent (CSS variable), seen 11 times. Token `secondary`, CSS `--ifm-color-primary-lighter`.
- **Orange (#C65D03):** Accent (CSS variable). Token `tertiary`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont`. Other loaded fonts: JetBrains Mono.

- **headline-display:** Inter 60px at weight 700, line height 1.05, tracking -0.04em (40px on mobile). Page title (h1).
- **headline-lg:** Inter 40px at weight 700, line height 1.15, tracking -0.03em (30px on mobile). Section headings (h2).
- **body-md:** Inter 16px at weight 400, line height 1.65. Body text.
- **body-lg:** Inter 18px at weight 600, line height 1.25, tracking -0.015em. Lead paragraphs.
- **body-sm:** Inter 15px at weight 400, line height 1.4. Secondary and small text.
- **caption:** Inter 14px at weight 400, line height 1.7. Captions and fine print.
- **label-lg:** Inter 16px at weight 600, line height 1.5, tracking -0.005em. Large buttons and tabs.
- **label-md:** Inter 15px at weight 500, line height 1.65. Buttons, navigation and labels.
- **label-sm:** Inter 13px at weight 500, line height 1.65. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 63% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 36px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 48px on each side of full-width sections.
- **Breakpoints:** 576px, 768px, 996px, 997px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(16, 24, 40, 0.05) 0px 1px 2px 0px`
- `rgb(228, 231, 236) 0px 0px 0px 1px, rgba(16, 24, 40, 0.05) 0px 1px 2px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (8px):** 32 elements.
- **full (9999px):** 28 elements.
- **md (10px):** 24 elements.
- **lg (12px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Open draw.io”):** #DC6803 fill, #FFFFFF text, 14px/600, 8px radius, padding 8px 16px, shadow `rgba(16, 24, 40, 0.05) 0px 1px 2px 0px`.
- **button-primary-hover:** background #C4520B, text #FFFFFF on hover.
- **button-outline (“Sketch”):** #FFFFFF fill, #101828 text, 13px/500, 999px radius, padding 4px 12px, shadow `rgb(228, 231, 236) 0px 0px 0px 1px, rgba(16, 24, 40, 0.05) 0px 1px 2px 0px`.
- **button-ghost (“Desktop App”):** #FFFFFF fill, #101828 text, 16px/600, 8px radius, padding 11px 22px, border 1px solid #D0D5DD, shadow `rgba(16, 24, 40, 0.05) 0px 1px 2px 0px`.
- **input-field (“Search”):** #F8F9FB fill, #101828 text, 14px/400, 8px radius, padding 0px 13.6px 0px 36px, border 1px solid #E4E7EC.
- **card:** #FFFFFF fill, #F08705 text, 16px/400, 10px radius, padding 0px, border 1px solid #E4E7EC, shadow `rgba(16, 24, 40, 0.05) 0px 1px 2px 0px`.
- **link:** transparent fill, #475467 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8F9FB.
- Do keep text in 4 levels: #475467, #101828, #667085, #A4A7AE.
- Do reserve #DC6803 for primary actions and key highlights.
- Do set headlines in Inter with tight tracking (-0.04em).
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't use #A4A7AE for body text; it reaches 2.41:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Inter.
- Don't use #DC6803 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s.

- **Easing:** `ease`, `cubic-bezier(0.08, 0.52, 0.52, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/drawio.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
