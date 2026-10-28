---
version: alpha
name: The Verge
description: "Dark interface measured from theverge.com: polySans type with fkRomanStandard, vivid teal accents, tonal surfaces and 1px corners."
colors:
  background: "#131313"
  surface: "#131313"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#E9E9E9"
  on-surface-muted: "#949494"
  surface-container-low: "#000000"
  surface-container: "#313131"
  overlay: "#1313138C"
  outline: "#313131"
  primary: "#3CFFD0"
  on-primary: "#000000"
  secondary: "#D6F31F"
typography:
  headline-display:
    fontFamily: polySans
    fontSize: 34px
    fontWeight: 700
    lineHeight: 1
  headline-lg:
    fontFamily: polySans
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1
  headline-md:
    fontFamily: polySans
    fontSize: 26px
    fontWeight: 700
    lineHeight: 1.1
  headline-sm:
    fontFamily: polySans
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: 0.01em
  title-lg:
    fontFamily: polySans
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1
  body-md:
    fontFamily: fkRomanStandard
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.01em
  body-lg:
    fontFamily: polySans
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.2
  body-sm:
    fontFamily: polySans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.3
  caption:
    fontFamily: polySans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.1
  label-lg:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: polySans
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.2
  label-sm:
    fontFamily: polySans
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0.1em
  code:
    fontFamily: polySansMono
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.18
    letterSpacing: 0.1em
  headline-sm-mobile:
    fontFamily: polySans
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: 0.01em
rounded:
  sm: 1px
  md: 24px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 40px
  gutter: 20px
  container: 1300px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.caption}"
    rounded: "{rounded.md}"
    padding: 10px 24px
    height: 44px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 10px 18px
    height: 42px
  button-secondary:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.caption}"
    rounded: "{rounded.md}"
    padding: 10px 24px
    height: 44px
  button-ghost:
    textColor: "{colors.primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 20px
  link:
    textColor: "{colors.on-surface}"
---

# The Verge Design System

## Overview

The Verge describes itself as: “The Verge is about technology and how it makes us feel. Founded in 2011, we offer our audience everything from breaking news to reviews to award-winning features and investigations, on our site, in video, and in podcasts” The interface is dark, built on **Charcoal (#131313)** with **White (#FFFFFF)** text, and **Vivid Teal (#3CFFD0)** as the main accent.

Type is set in **polySans** and **fkRomanStandard**, with **polySansMono** for code. Headlines run large; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 1px.

Measured from [theverge.com](https://www.theverge.com/) on October 21, 2026 at 1440×900 and 392×849 from 444 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Charcoal (#131313):** Page background, seen 2 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 64 times. Token `on-surface`.
- **Mist (#E9E9E9):** Secondary text, seen 10 times. Token `on-surface-variant`.
- **Gray (#949494):** Muted text and metadata, seen 10 times. Token `on-surface-muted`.
- **Near Black (#000000):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Graphite (#313131):** Cards and panels, seen 4 times. Token `surface-container`.
- **Charcoal 55% (#1313138C):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Graphite (#313131):** Borders and dividers, seen 49 times. Token `outline`.
- **Vivid Teal (#3CFFD0):** Brand color on large areas, seen 31 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Lime (#D6F31F):** Accent, seen 8 times. Token `secondary`.

## Typography

**polySans**, **fkRomanStandard**, **system-ui** and **polySansMono** (monospace) share the interface. Fallback stack: `polySans, polySans Fallback, Helvetica, Arial`. Other loaded fonts: fkRomanStandard Fallback, manuka, manuka Fallback, polySans Fallback.

- **headline-display:** polySans 34px at weight 700, line height 1. Page title (h1).
- **headline-lg:** polySans 28px at weight 700, line height 1. Section headings (h2).
- **headline-md:** polySans 26px at weight 700, line height 1.1. Sub-section headings.
- **headline-sm:** polySans 24px at weight 700, line height 1.1, tracking 0.01em (20px on mobile). Card and feature titles.
- **title-lg:** polySans 20px at weight 700, line height 1. Small titles.
- **body-md:** fkRomanStandard 16px at weight 400, line height 1.3, tracking -0.01em. Body text.
- **body-lg:** polySans 18px at weight 700, line height 1.2. Lead paragraphs.
- **body-sm:** polySans 14px at weight 400, line height 1.3. Secondary and small text.
- **caption:** polySans 12px at weight 400, line height 1.1. Captions and fine print.
- **label-lg:** system-ui 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** polySans 15px at weight 700, line height 1.2. Buttons, navigation and labels.
- **label-sm:** polySans 11px at weight 400, line height 1.2, tracking 0.1em, uppercase. Small labels and badges.
- **code:** polySansMono 11px at weight 400, line height 1.18, tracking 0.1em. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (71% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 40px.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1300px.
- **Breakpoints:** 768px, 900px, 901px, 1024px, 1179px, 1180px, 1181px, 1200px, 1300px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#000000 → #313131) and hairline rings:

- `rgb(60, 255, 208) 0px -1px 0px 0px inset`

## Shapes

Most elements use 1px corners. Measured radii, most used first:

- **sm (1px):** 8 elements.
- **md (24px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“LATEST”):** #3CFFD0 fill, #000000 text, 12px/600, 24px radius, padding 10px 24px.
- **button-outline (“Accept”):** #000000 fill, #FFFFFF text, 14px/400, padding 10px 18px.
- **button-secondary (“FOLLOWING”):** #313131 fill, #E9E9E9 text, 12px/600, 24px radius, padding 10px 24px.
- **button-ghost (“SKIP TO MAIN CONTENT”):** transparent fill, #3CFFD0 text, 11px/500, 1px radius, padding 0px 20px, border 1px solid #3CFFD0.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #131313 for the page and lift surfaces in small steps: #000000, #313131.
- Do keep text in 3 levels: #FFFFFF, #E9E9E9, #949494.
- Do use #3CFFD0 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do use 1px corners on most elements; larger surfaces also use 24px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond polySans, fkRomanStandard, system-ui and polySansMono.
- Don't use #3CFFD0 for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/theverge.com/), the free DESIGN.md generator.
