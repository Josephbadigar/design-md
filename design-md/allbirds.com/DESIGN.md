---
version: alpha
name: Allbirds
description: "Light monochrome interface measured from allbirds.com: Self Modern type with Geograph, tonal surfaces and 20px corners."
colors:
  background: "#ECE9E2"
  surface: "#ECE9E2"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#212121"
  surface-container-low: "#FFFFFF"
  outline: "#FFFFFF"
  primary: "#212121"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: Self Modern
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.5
  headline-lg:
    fontFamily: Geograph
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: 0.025em
  body-md:
    fontFamily: Geograph
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: 0.05em
  body-sm:
    fontFamily: Geograph
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-lg:
    fontFamily: Geograph
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Geograph
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Geograph
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: 0.025em
  code:
    fontFamily: Akkurat Mono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: 0.1em
rounded:
  sm: 4px
  md: 6px
  lg: 20px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 8px
  section: 80px
  margin: 40px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 12px 0px
    height: 48px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    padding: 8px 16px
    height: 33px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    padding: 8px 16px
    height: 33px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    padding: 10px 80px 10px 12px
  link:
    textColor: "{colors.on-primary}"
---

# Allbirds Design System

## Overview

Allbirds describes itself as: “Allbirds: The world’s most comfortable shoes, flats, and clothing made with natural materials like merino wool and eucalyptus. FREE shipping & returns.” The interface is light, built on **Warm Mist (#ECE9E2)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Self Modern** and **Geograph**, with **Akkurat Mono** for code. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 20px.

Measured from [allbirds.com](https://www.allbirds.com/) on October 21, 2026 at 1440×900 and 390×844 from 162 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **Warm Mist (#ECE9E2):** Page background, seen 1 time. Token `background`, CSS `--color-natural-white-60`.
- **Near Black (#000000):** Primary text and headings, seen 11 times. Token `on-surface`.
- **Charcoal (#212121):** Secondary text, seen 9 times. Token `on-surface-variant`, CSS `--ab-qa-ink`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`, CSS `--tw-ring-offset-color`.
- **White (#FFFFFF):** Borders and dividers, seen 6 times. Token `outline`, CSS `--tw-ring-offset-color`.
- **Charcoal (#212121):** Primary buttons and calls to action, seen 25 times. Token `primary`, CSS `--ab-qa-ink`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**Self Modern**, **Geograph** and **Akkurat Mono** (monospace) share the interface. Fallback stack: `Self Modern, ui-serif, serif`. Other loaded fonts: Barlow.

- **headline-display:** Self Modern 40px at weight 400, line height 1.5. Page title (h1).
- **headline-lg:** Geograph 24px at weight 400, line height 1.33, tracking 0.025em. Section headings (h2).
- **body-md:** Geograph 14px at weight 400, line height 1.43, tracking 0.05em. Body text.
- **body-sm:** Geograph 12px at weight 400, line height 1.33. Secondary and small text.
- **label-lg:** Geograph 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** Geograph 14px at weight 500, line height 1.43, tracking 0.05em. Buttons, navigation and labels.
- **label-sm:** Geograph 12px at weight 500, line height 1.25, tracking 0.025em, uppercase. Small labels and badges.
- **code:** Akkurat Mono 12px at weight 400, line height 1.33, tracking 0.1em, uppercase. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (80% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 600px, 767px, 768px, 3120px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF) and #FFFFFF borders.

## Shapes

Most elements use 20px corners. Measured radii, most used first:

- **lg (20px):** 16 elements.
- **md (6px):** 8 elements.
- **sm (4px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“CONFIRM”):** #212121 fill, #FFFFFF text, 16px/400, 6px radius, padding 12px 0px.
- **button-outline (“SHOP MEN”):** #FFFFFF fill, #212121 text, 12px/500, 3.35544e+07px radius, padding 8px 16px, border 1px solid #FFFFFF.
- **button-ghost (“SHOP MEN”):** transparent fill, #FFFFFF text, 12px/500, 3.35544e+07px radius, padding 8px 16px, border 1px solid #FFFFFF.
- **input-field (“Email Address”):** #FFFFFF fill, #212121 text, 16px/400, 3.35544e+07px radius, padding 10px 80px 10px 12px, border 1px solid #212121.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #ECE9E2 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 2 levels: #000000, #212121.
- Do let contrast carry emphasis; primary actions use #212121 on #ECE9E2.
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do use 20px corners on most elements; larger surfaces also use 6px and 4px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Self Modern, Geograph and Akkurat Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s.

- **Easing:** `cubic-bezier(0.37, 0, 0.63, 1)`, `cubic-bezier(0.61, 1, 0.88, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/allbirds.com/), the free DESIGN.md generator.
