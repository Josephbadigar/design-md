---
version: alpha
name: Linear
description: "Dark monochrome interface measured from linear.app: Inter Variable type, tonal surfaces and pill-shaped controls."
colors:
  background: "#08090A"
  surface: "#08090A"
  on-surface: "#F7F8F8"
  on-background: "#F7F8F8"
  on-surface-variant: "#D0D6E0"
  on-surface-muted: "#8A8F98"
  on-surface-subtle: "#62666D"
  surface-container-low: "#0F1011"
  surface-container: "#121414"
  surface-container-high: "#161718"
  surface-container-highest: "#1C1C1D"
  overlay: "#FFFFFF05"
  overlay-strong: "#FFFFFF0D"
  outline: "#FFFFFF14"
  outline-variant: "#2E2E32"
  primary: "#E5E5E6"
  on-primary: "#08090A"
  secondary: "#F0BF00"
typography:
  headline-display:
    fontFamily: Inter Variable
    fontSize: 64px
    fontWeight: 510
    lineHeight: 1
    letterSpacing: -0.022em
  headline-lg:
    fontFamily: Inter Variable
    fontSize: 48px
    fontWeight: 510
    lineHeight: 1
    letterSpacing: -0.022em
  headline-md:
    fontFamily: Inter Variable
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.022em
  headline-sm:
    fontFamily: Inter Variable
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: -0.012em
  body-md:
    fontFamily: Inter Variable
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Inter Variable
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.01em
  caption:
    fontFamily: Inter Variable
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.17
  label-lg:
    fontFamily: Inter Variable
    fontSize: 16px
    fontWeight: 510
  label-md:
    fontFamily: Inter Variable
    fontSize: 13px
    fontWeight: 510
  label-sm:
    fontFamily: Inter Variable
    fontSize: 12px
    fontWeight: 510
    lineHeight: 1.17
  code:
    fontFamily: Berkeley Mono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
  headline-display-mobile:
    fontFamily: Inter Variable
    fontSize: 38px
    fontWeight: 510
    lineHeight: 1.1
    letterSpacing: -0.022em
  headline-lg-mobile:
    fontFamily: Inter Variable
    fontSize: 24px
    fontWeight: 510
    lineHeight: 1.33
    letterSpacing: -0.012em
rounded:
  sm: 4px
  md: 8px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 36px
  gutter: 8px
  section: 128px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px 12px
    height: 32px
  button-outline:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.caption}"
    rounded: 16px
    padding: 0px 11px 0px 7px
    height: 24px
  button-ghost:
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 0px 12px
  input-field:
    backgroundColor: "#3B3B3B"
    textColor: "#FFFFFF"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 6px
    padding: 11px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Linear Design System

## Overview

Linear describes itself as: “Purpose-built for planning and building products with AI agents.” The interface is dark, built on **Near Black (#08090A)** with **Snow (#F7F8F8)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Inter Variable**, with **Berkeley Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [linear.app](https://linear.app/) on October 28, 2026 at 1440×900 and 390×844 from 438 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #B2D5FF, #DFD1FF.

- **Near Black (#08090A):** Page background, seen 3 times. Token `background`.
- **Snow (#F7F8F8):** Primary text and headings, seen 20 times. Token `on-surface`.
- **Cool Silver (#D0D6E0):** Secondary text, seen 25 times. Token `on-surface-variant`, CSS `--color-text-secondary`.
- **Cool Gray (#8A8F98):** Muted text and metadata, seen 25 times. Token `on-surface-muted`, CSS `--color-text-tertiary`.
- **Cool Slate (#62666D):** Subtle text and placeholders, seen 33 times. Token `on-surface-subtle`.
- **Charcoal (#0F1011):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Charcoal (#121414):** Cards and panels, seen 1 time. Token `surface-container`.
- **Charcoal (#161718):** Hover and pressed fills, seen 3 times. Token `surface-container-high`.
- **Charcoal (#1C1C1D):** Highest raised elements, seen 1 time. Token `surface-container-highest`.
- **White 2% (#FFFFFF05):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **White 5% (#FFFFFF0D):** Stronger translucent fill, seen 2 times. Token `overlay-strong`, CSS `--sx-1urpf9d`.
- **White 8% (#FFFFFF14):** Borders and dividers, seen 6 times. Token `outline`.
- **Graphite (#2E2E32):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Mist (#E5E5E6):** Primary buttons and calls to action, seen 82 times. Token `primary`.
- **Near Black (#08090A):** Text and icons on primary. Token `on-primary`.
- **Vivid Amber (#F0BF00):** Accent, seen 6 times. Token `secondary`.

## Typography

**Inter Variable** and **Berkeley Mono** (monospace) share the interface. Fallback stack: `Inter Variable, SF Pro Display, -apple-system, BlinkMacSystemFont`.

- **headline-display:** Inter Variable 64px at weight 510, line height 1, tracking -0.022em (38px on mobile). Page title (h1).
- **headline-lg:** Inter Variable 48px at weight 510, line height 1, tracking -0.022em (24px on mobile). Section headings (h2).
- **headline-md:** Inter Variable 32px at weight 400, line height 1.13, tracking -0.022em. Sub-section headings.
- **headline-sm:** Inter Variable 24px at weight 400, line height 1.33, tracking -0.012em. Card and feature titles.
- **body-md:** Inter Variable 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Inter Variable 13px at weight 400, line height 1.5, tracking -0.01em. Secondary and small text.
- **caption:** Inter Variable 12px at weight 400, line height 1.17. Captions and fine print.
- **label-lg:** Inter Variable 16px at weight 510. Large buttons and tabs.
- **label-md:** Inter Variable 13px at weight 510. Buttons, navigation and labels.
- **label-sm:** Inter Variable 12px at weight 510, line height 1.17. Small labels and badges.
- **code:** Berkeley Mono 12px at weight 400, line height 1.4. Code and technical values.

## Layout

Spacing does not follow a strict grid: 54% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 36px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 640px, 641px, 768px, 769px, 928px, 1024px, 1140px, 1280px, 1281px, 1439px, 1440px, 1536px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#0F1011 → #121414 → #161718 → #1C1C1D):

- `rgba(255, 255, 255, 0.05) 0px 0px 0px 1px inset`
- `rgba(255, 255, 255, 0.08) 0px 0px 0px 0.5px inset`
- `rgba(0, 0, 0, 0.2) 0px 0px 0px 1px`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0) 0px 8px 2px 0px, rgba(0, 0, 0, 0.01) 0px 5px 2px 0px, rgba(0, 0, 0, 0.04) 0px 3px 2px 0px, rgba(0, 0, 0, 0.07) 0px 1px 1px 0px, rgba(0, 0, 0, 0.08) 0px 0px 1px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 92 elements.
- **sm (4px):** 80 elements.
- **md (8px):** 80 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #E5E5E6 fill, #08090A text, 13px/510, 9999px radius, padding 0px 12px, border 1px solid #E5E5E6, shadow `rgba(0, 0, 0, 0) 0px 8px 2px 0px, rgba(0, 0, 0, 0.01) 0px 5px 2px 0px, rgba(0, 0, 0, 0.04) 0px 3px 2px 0px, rgba(0, 0, 0, 0.07) 0px 1px 1px 0px, rgba(0, 0, 0, 0.08) 0px 0px 1px 0px`.
- **button-outline (“Performance”):** transparent fill, #D0D6E0 text, 12px/400, 16px radius, padding 0px 11px 0px 7px, border 1px solid #2E2E32.
- **button-ghost (“Product”):** transparent fill, #8A8F98 text, 13px/400, 9999px radius, padding 0px 12px.
- **input-field:** #3B3B3B fill, #FFFFFF text, 13.3333px/400, padding 0px.
- **card:** #161718 fill, #F7F8F8 text, 16px/400, 6px radius, padding 11px, border 1px solid #FFFFFF0F.
- **link:** transparent fill, #8A8F98 text, padding 0px.

## Do's and Don'ts

- Do use #08090A for the page and lift surfaces in small steps: #0F1011, #121414, #161718, #1C1C1D.
- Do keep text in 4 levels: #F7F8F8, #D0D6E0, #8A8F98, #62666D.
- Do let contrast carry emphasis; primary actions use #E5E5E6 on #08090A.
- Do set headlines in Inter Variable with tight tracking (-0.022em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't use #62666D for body text; it reaches 3.4:1 on #08090A. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Inter Variable and Berkeley Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.16s, 0.1s, 0.2s, 0.15s. Longer ambient animations run 2.8s, 1.6s, 3.2s.

- **Easing:** `cubic-bezier(0.25, 0.46, 0.45, 0.94)`, `ease`, `cubic-bezier(0.165, 0.84, 0.44, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/linear.app/), the free DESIGN.md generator.
