---
version: alpha
name: Framer
description: "Dark monochrome interface measured from framer.com: GT Walsheim Medium type with Inter, tonal surfaces and 8px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#CCCCCC"
  on-surface-muted: "#999999"
  on-surface-subtle: "#666666"
  surface-container-low: "#1F1F1F"
  overlay: "#FFFFFF1A"
  overlay-strong: "#222222CC"
  outline: "#FFFFFF1A"
  outline-variant: "#0000001A"
  primary: "#FFFFFF"
  on-primary: "#000000"
  secondary: "#0099FF"
  success: "#00BB88"
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
  sm: 8px
  md: 10px
  lg: 18px
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
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 10px
    height: 30px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Framer Design System

## Overview

Framer describes itself as: “The free website builder with a design agent that takes you from idea to launch. Changes stay editable, with hosting, CMS, analytics, SEO, and AEO built in.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **GT Walsheim Medium** and **Inter**, with **Input Mono Regular** for code. Headlines run large with tight negative tracking; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [framer.com](https://www.framer.com/) on October 29, 2026 at 1440×900 and 390×844 from 434 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Near Black (#000000):** Page background, seen 14 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 61 times. Token `on-surface`.
- **Silver (#CCCCCC):** Secondary text, seen 7 times. Token `on-surface-variant`.
- **Gray (#999999):** Muted text and metadata, seen 52 times. Token `on-surface-muted`.
- **Slate (#666666):** Subtle text and placeholders, seen 10 times. Token `on-surface-subtle`.
- **Charcoal (#1F1F1F):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **Charcoal 80% (#222222CC):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 14 times. Token `outline`.
- **Near Black 10% (#0000001A):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 67 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0099FF):** Accent in text, fills and borders, seen 3 times. Token `secondary`.
- **Dark Teal (#00BB88):** Success and positive states, seen 4 times. Token `success`.

## Typography

**GT Walsheim Medium**, **Inter**, **Inter Variable** and **Input Mono Regular** (monospace) share the interface. Fallback stack: `GT Walsheim Medium, GT Walsheim Medium Placeholder, sans-serif`. Other loaded fonts: JetBrains Mono, Inter Medium, Input Mono Bold.

- **headline-display:** GT Walsheim Medium 54px at weight 500, line height 1, tracking -0.04em (36px on mobile). Page title (h1).
- **headline-lg:** GT Walsheim Medium 44px at weight 500, line height 1.1, tracking -0.04em (28px on mobile). Section headings (h2).
- **headline-md:** Inter 20px at weight 600, line height 1.2, tracking -0.04em. Sub-section headings.
- **body-md:** Inter Variable 18px at weight 400, line height 1.35, tracking -0.011em. Body text.
- **body-sm:** Inter Variable 12px at weight 400, line height 1.2. Secondary and small text.
- **label-lg:** Inter 13px at weight 500, line height 1.6. Large buttons and tabs.
- **label-md:** Inter 12px at weight 500, line height 1.2. Buttons, navigation and labels.
- **label-sm:** Inter 10px at weight 500, line height 1.2. Small labels and badges.
- **code:** Input Mono Regular 12px at weight 400, line height 1.33. Code and technical values.

## Layout

Spacing does not follow a strict grid: 26% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 5px, md 10px, lg 20px, xl 40px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1200px.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 809px, 809.98px, 810px, 1199px, 1199.98px, 1200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.2) 0px 2px 6px 0px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0.25) 0px 0px 0px 0px`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 124 elements.
- **lg (18px):** 32 elements.
- **md (10px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #FFFFFF fill, #000000 text, 12px/400, 8px radius, padding 8px 10px.
- **input-field (“Add follow up...”):** transparent fill, #FFFFFF text, 12px/500, padding 0px.
- **link:** transparent fill, #FFFFFF99 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #1F1F1F.
- Do keep text in 4 levels: #FFFFFF, #CCCCCC, #999999, #666666.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #000000.
- Do set headlines in GT Walsheim Medium with tight tracking (-0.04em).
- Do reuse the measured spacing steps (5px, 10px, 20px).
- Do use 8px corners on most elements; larger surfaces also use 18px and 10px.
- Don't use #666666 for body text; it reaches 3.66:1 on #000000. Keep it for large text or metadata.
- Don't introduce new font families beyond GT Walsheim Medium, Inter, Inter Variable and Input Mono Regular.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.

Generated by [Sitepeel](https://sitepeel.dev/design-md/framer.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
