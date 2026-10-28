---
version: alpha
name: Framer
description: "Dark monochrome interface measured from framer.com: GT Walsheim Medium type with Inter, flat surfaces and 8px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#CCCCCC"
  on-surface-muted: "#999999"
  on-surface-subtle: "#666666"
  overlay: "#FFFFFF1A"
  overlay-strong: "#FFFFFF4D"
  outline: "#FFFFFF1A"
  primary: "#FFFFFF"
  on-primary: "#0000EE"
  secondary: "#0099FF"
  tertiary: "#4CD963"
  success: "#00BB88"
  error: "#D67A5C"
typography:
  headline-display:
    fontFamily: GT Walsheim Medium
    fontSize: 54px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: GT Walsheim Medium
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.04em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.04em
  body-md:
    fontFamily: Inter Variable
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.35
    letterSpacing: -0.011em
  body-sm:
    fontFamily: Inter Variable
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.007em
  caption:
    fontFamily: Inter Variable
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.2
  label-lg:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.6
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.2
  label-sm:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: 500
    lineHeight: 1.2
  code:
    fontFamily: Input Mono Regular
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  headline-display-mobile:
    fontFamily: GT Walsheim Medium
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.04em
  headline-lg-mobile:
    fontFamily: GT Walsheim Medium
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.04em
rounded:
  md: 8px
spacing:
  xs: 3px
  sm: 5px
  md: 10px
  lg: 20px
  xl: 40px
  gutter: 10px
  section: 120px
  margin: 20px
  container: 1200px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.caption}"
    rounded: "{rounded.md}"
    padding: 8px 10px
    height: 30px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-primary}"
---

# Framer Design System

## Overview

Framer describes itself as: “Go from idea to launch with an agent that designs and builds on the canvas. Keep each change editable, with hosting, security, analytics, CMS, and SEO built in.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **GT Walsheim Medium** and **Inter**, with **Input Mono Regular** for code. Headlines run large with tight negative tracking; body text is 18px. The surface language is flat. Corners are mostly 8px.

Measured from [framer.com](https://www.framer.com/) on October 21, 2026 at 1440×900 and 390×844 from 406 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Near Black (#000000):** Page background, seen 9 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 51 times. Token `on-surface`.
- **Silver (#CCCCCC):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Gray (#999999):** Muted text and metadata, seen 48 times. Token `on-surface-muted`.
- **Slate (#666666):** Subtle text and placeholders, seen 8 times. Token `on-surface-subtle`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **White 30% (#FFFFFF4D):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 6 times. Token `outline`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 61 times. Token `primary`.
- **Vivid Indigo (#0000EE):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0099FF):** Most used accent color, seen 11 times. Token `secondary`.
- **Green (#4CD963):** Accent, seen 3 times. Token `tertiary`.
- **Dark Teal (#00BB88):** Success and positive states, seen 5 times. Token `success`.
- **Red (#D67A5C):** Errors and destructive states, seen 5 times. Token `error`.

## Typography

**GT Walsheim Medium**, **Inter**, **Inter Variable** and **Input Mono Regular** (monospace) share the interface. Fallback stack: `GT Walsheim Medium, GT Walsheim Medium Placeholder, sans-serif`. Other loaded fonts: JetBrains Mono, Inter Medium, Input Mono Bold, GT Walsheim Medium Placeholder.

- **headline-display:** GT Walsheim Medium 54px at weight 500, line height 1, tracking -0.04em (36px on mobile). Page title (h1).
- **headline-lg:** GT Walsheim Medium 44px at weight 500, line height 1.1, tracking -0.04em (28px on mobile). Section headings (h2).
- **headline-md:** Inter 20px at weight 600, line height 1.2, tracking -0.04em. Sub-section headings.
- **body-md:** Inter Variable 18px at weight 400, line height 1.35, tracking -0.011em. Body text.
- **body-sm:** Inter Variable 14px at weight 400, line height 1.4, tracking -0.007em. Secondary and small text.
- **caption:** Inter Variable 12px at weight 400, line height 1.2. Captions and fine print.
- **label-lg:** Inter 13px at weight 500, line height 1.6. Large buttons and tabs.
- **label-md:** Inter 12px at weight 500, line height 1.2. Buttons, navigation and labels.
- **label-sm:** Inter 10px at weight 500, line height 1.2. Small labels and badges.
- **code:** Input Mono Regular 12px at weight 400, line height 1.33. Code and technical values.

## Layout

Spacing does not follow a strict grid: 18% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 5px, md 10px, lg 20px, xl 40px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1200px.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 809px, 809.98px, 810px, 1199px, 1199.98px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #FFFFFF1A borders.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 252 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #FFFFFF fill, #0000EE text, 12px/400, 8px radius, padding 8px 10px.
- **input-field (“Add follow up...”):** transparent fill, #FFFFFF text, 12px/500, padding 0px.
- **link:** transparent fill, #0000EE text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page.
- Do keep text in 4 levels: #FFFFFF, #CCCCCC, #999999, #666666.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #000000.
- Do set headlines in GT Walsheim Medium with tight tracking (-0.04em).
- Do reuse the measured spacing steps (5px, 10px, 20px).
- Do use 8px corners on most elements.
- Don't use #666666 for body text; it reaches 3.7:1 on #000000. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond GT Walsheim Medium, Inter, Inter Variable and Input Mono Regular.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.

Generated by [Sitepeel](https://sitepeel.dev/design-md/framer.com/), the free DESIGN.md generator.
