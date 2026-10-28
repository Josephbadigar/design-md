---
version: alpha
name: Brex
description: "Light interface measured from brex.com: inter type, vivid red accents, tonal surfaces and 10px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#15191E"
  on-background: "#15191E"
  on-surface-variant: "#60646C"
  on-surface-muted: "#8B8D98"
  on-surface-subtle: "#B9BBC6"
  surface-container-low: "#F9F9FB"
  surface-container: "#F3F3F7"
  outline: "#42578A26"
  primary: "#FF3D00"
  on-primary: "#FCFCFD"
  inverse-surface: "#000710"
typography:
  headline-display:
    fontFamily: inter
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: inter
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  headline-md:
    fontFamily: inter
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: inter
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.21
    letterSpacing: -0.02em
  title-lg:
    fontFamily: inter
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-md:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.02em
  body-sm:
    fontFamily: inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: -0.02em
  label-md:
    fontFamily: inter
    fontSize: 16px
    fontWeight: 400
  label-sm:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: inter
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.02em
rounded:
  sm: 6px
  md: 8px
  lg: 10px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px 12px
    height: 36px
  button-primary-hover:
    backgroundColor: "#FF6B18"
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 16px
    height: 40px
  button-secondary-hover:
    backgroundColor: "#FF6B18"
  button-ghost:
    textColor: "#000000"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 4px 8px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 8px 2px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Brex Design System

## Overview

Brex describes itself as: “Simplify expense management with Brex's finance platform. From company cards to banking, Brex helps you drive growth, automate processes, & earn more.” The interface is light, built on **White (#FFFFFF)** with **Cool Charcoal (#15191E)** text, and **Vivid Red (#FF3D00)** as the main accent.

Type is set in **inter**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 10px.

Measured from [brex.com](https://www.brex.com/) on October 21, 2026 at 1440×900 and 390×844 from 369 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 15 times. Token `background`.
- **Cool Charcoal (#15191E):** Primary text and headings, seen 50 times. Token `on-surface`.
- **Cool Slate (#60646C):** Secondary text, seen 21 times. Token `on-surface-variant`.
- **Cool Gray (#8B8D98):** Muted text and metadata, seen 31 times. Token `on-surface-muted`.
- **Cool Silver (#B9BBC6):** Subtle text and placeholders, seen 26 times. Token `on-surface-subtle`.
- **Snow (#F9F9FB):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#F3F3F7):** Cards and panels, seen 6 times. Token `surface-container`.
- **Blue 15% (#42578A26):** Borders and dividers, seen 1 time. Token `outline`, CSS `--_1k5xs267n`.
- **Vivid Red (#FF3D00):** Primary buttons and calls to action, seen 20 times. Token `primary`.
- **Snow (#FCFCFD):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000710):** High-contrast fills, seen 3 times. Token `inverse-surface`.

## Typography

**inter** carries the whole interface. Fallback stack: `inter, inter Fallback, sans-serif`. Other loaded fonts: inter Fallback, flecha, flecha Fallback.

- **headline-display:** inter 72px at weight 500, line height 1, tracking -0.02em. Page title (h1).
- **headline-lg:** inter 48px at weight 500, line height 1, tracking -0.02em (30px on mobile). Section headings (h2).
- **headline-md:** inter 36px at weight 500, line height 1, tracking -0.02em. Sub-section headings.
- **headline-sm:** inter 24px at weight 500, line height 1.21, tracking -0.02em. Card and feature titles.
- **title-lg:** inter 20px at weight 500, line height 1.2, tracking -0.02em. Small titles.
- **body-md:** inter 14px at weight 400, line height 1.5, tracking -0.02em. Body text.
- **body-sm:** inter 12px at weight 400, line height 1.33, tracking -0.02em. Secondary and small text.
- **label-md:** inter 16px at weight 400. Buttons, navigation and labels.
- **label-sm:** inter 14px at weight 500, line height 1.5, tracking -0.02em. Small labels and badges.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 766px, 767px, 830px, 900px, 960px, 1023px, 1024px, 1680px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F9F9FB → #F3F3F7) and #42578A26 borders.

## Shapes

Most elements use 10px corners. Measured radii, most used first:

- **lg (10px):** 36 elements.
- **sm (6px):** 12 elements.
- **full (9999px):** 8 elements.
- **md (8px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #FF3D00 fill, #FCFCFD text, 14px/400, 10px radius, padding 0px 12px, border 1px solid #FF3D00.
- **button-primary-hover:** background #FF6B18, text #FCFCFD on hover.
- **button-secondary (“Get started”):** #FF3D00 fill, #FFFFFF text, 14px/400, 8px radius, padding 0px 16px, border 1px solid #42578A26.
- **button-secondary-hover:** background #FF6B18, text #FFFFFF on hover.
- **button-ghost (“Products”):** transparent fill, #000000 text, 16px/400, 6px radius, padding 4px 8px.
- **input-field (“Enter your work email”):** transparent fill, #15191E text, 14px/400, padding 8px 2px.
- **link:** transparent fill, #8B8D98 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F9F9FB, #F3F3F7.
- Do keep text in 4 levels: #15191E, #60646C, #8B8D98, #B9BBC6.
- Do reserve #FF3D00 for primary actions and key highlights.
- Do set headlines in inter with tight tracking (-0.02em).
- Do keep spacing on the 4px grid.
- Do use 10px corners on most elements; larger surfaces also use 6px and 8px.
- Don't use #8B8D98 for body text; it reaches 3.3:1 on #FFFFFF. Keep it for large text or metadata.
- Don't use #B9BBC6 for body text; it reaches 1.9:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond inter.
- Don't use #FF3D00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.125s, 0.5s.

- **Easing:** `linear`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/brex.com/), the free DESIGN.md generator.
