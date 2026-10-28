---
version: alpha
name: Pitch
description: "Light interface measured from pitch.com: Mark Pro Bold type with Mark Pro Regular, light violet accents, tonal surfaces and 40px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0C021C"
  on-background: "#0C021C"
  surface-container-low: "#EBE3FE"
  primary: "#C6A5FF"
  on-primary: "#000000"
  secondary: "#280F62"
  tertiary: "#5318EB"
typography:
  headline-display:
    fontFamily: Mark Pro Bold
    fontSize: 180px
    fontWeight: 700
    lineHeight: 0.8
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Mark Pro Regular
    fontSize: 64px
    fontWeight: 400
    lineHeight: 0.9
    letterSpacing: -0.04em
  headline-md:
    fontFamily: Mark Pro Bold
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.04em
  headline-sm:
    fontFamily: Mark Pro Bold
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.04em
  title-lg:
    fontFamily: Mark Pro Bold
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-md:
    fontFamily: Eina 03 Regular
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
  body-lg:
    fontFamily: Eina 03 Regular
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: -0.02em
  body-sm:
    fontFamily: Eina 03 Regular
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.6
  label-md:
    fontFamily: Eina 03 Bold
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.02em
  label-sm:
    fontFamily: sans-serif
    fontSize: 12px
    fontWeight: 400
  code:
    fontFamily: Space Mono
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: -0.02em
  headline-display-mobile:
    fontFamily: Mark Pro Bold
    fontSize: 82px
    fontWeight: 700
    lineHeight: 0.8
    letterSpacing: -0.04em
rounded:
  xs: 4px
  sm: 8px
  md: 30px
  lg: 40px
  xl: 100px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  gutter: 8px
  section: 120px
  margin: 24px
components:
  button-primary:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.background}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.xs}"
    padding: 8px 12px 8px 16px
    height: 36px
  button-secondary:
    backgroundColor: "#C4EE87"
    textColor: "#0000EE"
    typography: "{typography.label-sm}"
    rounded: "{rounded.xs}"
    padding: 10px 12px
    height: 44px
  button-secondary-hover:
    backgroundColor: "{colors.primary}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 4px 12px 4px 8px
  input-field:
    textColor: "#0D031D"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Pitch Design System

## Overview

Pitch describes itself as: “Pitch is the collaborative presentation platform for teams that want to create, share, and deliver better work.” The interface is light, built on **White (#FFFFFF)** with **Deep Violet (#0C021C)** text, and **Light Violet (#C6A5FF)** as the main accent.

Type is set in **Mark Pro Bold** and **Mark Pro Regular**, with **Space Mono** for code. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 40px.

Measured from [pitch.com](https://pitch.com/) on October 21, 2026 at 1440×900 and 390×844 from 252 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **White (#FFFFFF):** Page background, seen 6 times. Token `background`.
- **Deep Violet (#0C021C):** Primary text and headings, seen 58 times. Token `on-surface`.
- **Pale Violet (#EBE3FE):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **Light Violet (#C6A5FF):** Brand color in the header, seen 1 time. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Dark Violet (#280F62):** Brand color in logos and imagery, seen 47 times. Token `secondary`.
- **Vivid Violet (#5318EB):** Secondary buttons, seen 36 times. Token `tertiary`.

## Typography

**Mark Pro Bold**, **Mark Pro Regular**, **Eina 03 Regular**, **Eina 03 Bold**, **sans-serif** and **Space Mono** (monospace) share the interface. Fallback stack: `Mark Pro Bold, Mark Pro Bold Placeholder, sans-serif`. Other loaded fonts: Inter, Eina 03 Regular Placeholder, Mark Pro Bold Placeholder, Eina 03 Bold Placeholder.

- **headline-display:** Mark Pro Bold 180px at weight 700, line height 0.8, tracking -0.04em (82px on mobile). Page title (h1).
- **headline-lg:** Mark Pro Regular 64px at weight 400, line height 0.9, tracking -0.04em. Section headings (h2).
- **headline-md:** Mark Pro Bold 48px at weight 700, line height 1.2, tracking -0.04em. Sub-section headings.
- **headline-sm:** Mark Pro Bold 32px at weight 700, line height 1.2, tracking -0.04em. Card and feature titles.
- **title-lg:** Mark Pro Bold 28px at weight 700, line height 1.2, tracking -0.02em. Small titles.
- **body-md:** Eina 03 Regular 16px at weight 400, line height 1.6. Body text.
- **body-lg:** Eina 03 Regular 18px at weight 400, line height 1.6, tracking -0.02em. Lead paragraphs.
- **body-sm:** Eina 03 Regular 14px at weight 400, line height 1.6. Secondary and small text.
- **label-md:** Eina 03 Bold 16px at weight 700, line height 1.2, tracking -0.02em. Buttons, navigation and labels.
- **label-sm:** sans-serif 12px at weight 400. Small labels and badges.
- **code:** Space Mono 18px at weight 400, line height 1.6, tracking -0.02em. Code and technical values.

## Layout

Spacing follows a 4px grid: 92% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 809px, 809.98px, 810px, 1199px, 1199.98px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#EBE3FE).

## Shapes

Most elements use 40px corners. Measured radii, most used first:

- **lg (40px):** 20 elements.
- **xs (4px):** 12 elements.
- **md (30px):** 8 elements.
- **sm (8px):** 4 elements.
- **xl (100px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Generate”):** #5318EB fill, #FFFFFF text, 14px/400, 4px radius, padding 8px 12px 8px 16px.
- **button-secondary (“Sign up”):** #C4EE87 fill, #0000EE text, 12px/400, 4px radius, padding 10px 12px.
- **button-secondary-hover:** background #C6A5FF, text #0000EE on hover.
- **button-ghost (“Prompts”):** transparent fill, #0C021C text, 14px/600, 8px radius, padding 4px 12px 4px 8px.
- **input-field (“Generate a sales presentation fo”):** transparent fill, #0D031D text, 16px/400, padding 0px.
- **link:** transparent fill, #0C021C text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #EBE3FE.
- Do use #C6A5FF as the brand accent: header, logo and key highlights.
- Do set headlines in Mark Pro Bold with tight tracking (-0.04em).
- Do keep spacing on the 4px grid.
- Do use 40px corners on most elements; larger surfaces also use 4px, 30px and 8px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Mark Pro Bold, Mark Pro Regular, Eina 03 Regular, Eina 03 Bold, sans-serif and Space Mono.
- Don't use #C6A5FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s, 0.12s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/pitch.com/), the free DESIGN.md generator.
