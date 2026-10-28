---
version: alpha
name: Wise
description: "Light interface measured from wise.com: Wise Sans type with Inter, green accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#163300"
  on-background: "#163300"
  on-surface-strong: "#0E0F0C"
  on-surface-variant: "#454745"
  overlay: "#3E3B0712"
  overlay-strong: "#16330014"
  outline: "#9FE870"
  primary: "#9FE870"
  on-primary: "#000000"
  secondary: "#054D28"
  tertiary: "#B8232B"
typography:
  headline-display:
    fontFamily: Wise Sans
    fontSize: 105.5px
    fontWeight: 900
    lineHeight: 0.85
  headline-lg:
    fontFamily: Wise Sans
    fontSize: 89px
    fontWeight: 900
    lineHeight: 0.85
  headline-md:
    fontFamily: Wise Sans
    fontSize: 58.5px
    fontWeight: 900
    lineHeight: 0.85
  headline-sm:
    fontFamily: Wise Sans
    fontSize: 52px
    fontWeight: 400
    lineHeight: 1.5
  title-lg:
    fontFamily: Inter
    fontSize: 45.5px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.03em
  body-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.44
    letterSpacing: 0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: 0.005em
  body-sm:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.005em
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: 0.005em
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Wise Sans
    fontSize: 51px
    fontWeight: 900
    lineHeight: 0.85
rounded:
  md: 2px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 48px
  gutter: 12px
  section: 56.31px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.outline}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 8px 12px
    height: 32px
  button-primary-hover:
    backgroundColor: "#0D1F00"
    textColor: "#BBEF9A"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 8px 12px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-sm}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Wise Design System

## Overview

Wise describes itself as: “Banks charge a lot for overseas transfers. We don't. Transfer money abroad easily and quickly with our low cost money transfers.” The interface is light, built on **White (#FFFFFF)** with **Deep Lime (#163300)** text, and **Green (#9FE870)** as the main accent.

Type is set in **Wise Sans** and **Inter**. Headlines run large; body text is 18px. The surface language is flat. Controls are pill-shaped.

Measured from [wise.com](https://wise.com/) on October 21, 2026 at 1440×900 and 390×844 from 402 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`, CSS `--color-white`.
- **Deep Lime (#163300):** Primary text and headings, seen 103 times. Token `on-surface`.
- **Charcoal (#0E0F0C):** Headings and emphasis, seen 28 times. Token `on-surface-strong`, CSS `--color-content-link-active`.
- **Graphite (#454745):** Secondary text, seen 11 times. Token `on-surface-variant`.
- **Deep Yellow 7% (#3E3B0712):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Deep Lime 8% (#16330014):** Stronger translucent fill, seen 2 times. Token `overlay-strong`, CSS `--color-background-screen-hover`.
- **Green (#9FE870):** Borders and dividers, seen 3 times. Token `outline`, CSS `--color-interactive-accent`.
- **Green (#9FE870):** Brand color on large areas, seen 15 times. Token `primary`, CSS `--color-interactive-accent`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Deep Green (#054D28):** Brand accent (CSS variable), seen 12 times. Token `secondary`.
- **Red (#B8232B):** Brand accent (CSS variable), seen 12 times. Token `tertiary`.

## Typography

**Wise Sans** and **Inter** share the interface. Fallback stack: `Wise Sans, Inter, sans-serif`. Other loaded fonts: Averta.

- **headline-display:** Wise Sans 105.5px at weight 900, line height 0.85 (51px on mobile). Page title (h1).
- **headline-lg:** Wise Sans 89px at weight 900, line height 0.85. Section headings (h2).
- **headline-md:** Wise Sans 58.5px at weight 900, line height 0.85. Sub-section headings.
- **headline-sm:** Wise Sans 52px at weight 400, line height 1.5. Card and feature titles.
- **title-lg:** Inter 45.5px at weight 600, line height 1.25, tracking -0.03em. Small titles.
- **body-md:** Inter 18px at weight 400, line height 1.44, tracking 0.01em. Body text.
- **body-lg:** Inter 20px at weight 600, line height 1.4, tracking 0.005em. Lead paragraphs.
- **body-sm:** Inter 16px at weight 400, line height 1.5, tracking 0.005em. Secondary and small text.
- **label-md:** Inter 16px at weight 600, line height 1.5, tracking 0.005em. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 400, line height 1.5. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (86% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 32px, xl 48px.
- **Sections:** 56.31px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 0px, 479.98px, 480px, 575.98px, 576px, 767.98px, 768px, 991.98px, 992px, 1199.98px, 1200px, 1439.98px, 1440px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #9FE870 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (2px):** 320 elements.
- **full (9999px):** 96 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #163300 fill, #9FE870 text, 18px/600, 9999px radius, padding 8px 12px.
- **button-primary-hover:** background #0D1F00, text #BBEF9A on hover.
- **button-ghost (“Personal”):** transparent fill, #163300 text, 18px/600, 9999px radius, padding 8px 12px.
- **input-field (“0.00”):** transparent fill, #163300 text, 52px/400, padding 0px.
- **link:** transparent fill, #163300 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #163300, #0E0F0C, #454745.
- Do use #9FE870 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 32px).
- Do make buttons and chips fully rounded (9999px); most other elements use 2px corners.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Wise Sans and Inter.
- Don't use #9FE870 for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s. Longer ambient animations run 1s.

- **Easing:** `ease`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/wise.com/), the free DESIGN.md generator.
