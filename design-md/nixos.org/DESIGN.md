---
version: alpha
name: NixOS
description: "Dark interface measured from nixos.org: Route159 type with Roboto Flex Variable, dark blue accents, flat surfaces and 16px corners."
colors:
  background: "#3B5487"
  surface: "#3B5487"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#EEEEEE"
  on-surface-muted: "#000000"
  on-surface-subtle: "#0B0B0B"
  outline: "#506FB2"
  primary: "#28395F"
  on-primary: "#FFFFFF"
  secondary: "#4D6FB7"
  tertiary: "#A4D5F7"
typography:
  headline-display:
    fontFamily: Route159
    fontSize: 61px
    fontWeight: 700
    lineHeight: 1.25
  headline-lg:
    fontFamily: Route159
    fontSize: 39px
    fontWeight: 700
    lineHeight: 1.25
  headline-md:
    fontFamily: Route159
    fontSize: 22.5px
    fontWeight: 700
    lineHeight: 1.5
  body-md:
    fontFamily: Roboto Flex Variable
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.5
  body-lg:
    fontFamily: Route159
    fontSize: 19px
    fontWeight: 700
    lineHeight: 1.5
  body-sm:
    fontFamily: Roboto Flex Variable
    fontSize: 14px
    fontWeight: 300
    lineHeight: 1
  label-md:
    fontFamily: Roboto Flex Variable
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
rounded:
  sm: 16px
  md: 24px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 24px
  xl: 64px
  gutter: 16px
  section: 112px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 10px 14px
    height: 62px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 8px 24px
    height: 40px
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 10px 32px
    height: 44px
  button-ghost:
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 10px 32px
  link:
    textColor: "{colors.on-surface-variant}"
---

# NixOS Design System

## Overview

NixOS describes itself as: “Nix is a tool that takes a unique approach to package management and system configuration. Learn how to make reproducible, declarative and reliable systems.” The interface is dark, built on **Blue (#3B5487)** with **White (#FFFFFF)** text, and **Dark Blue (#28395F)** as the main accent.

Type is set in **Route159** and **Roboto Flex Variable**. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 16px.

Measured from [nixos.org](https://nixos.org/) on November 4, 2026 at 1440×900 and 390×844 from 218 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Blue (#3B5487):** Page background, seen 3 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 30 times. Token `on-surface`, CSS `--tw-ring-offset-color`.
- **Mist (#EEEEEE):** Secondary text, seen 21 times. Token `on-surface-variant`.
- **Near Black (#000000):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Near Black (#0B0B0B):** Subtle text and placeholders, seen 5 times. Token `on-surface-subtle`.
- **Blue (#506FB2):** Borders and dividers, seen 15 times. Token `outline`.
- **Dark Blue (#28395F):** Brand color on large areas, seen 10 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#4D6FB7):** Secondary buttons, seen 21 times. Token `secondary`.
- **Light Blue (#A4D5F7):** Accent in text, fills and borders, seen 10 times. Token `tertiary`.

## Typography

**Route159** and **Roboto Flex Variable** share the interface. Fallback stack: `Route159, -apple-system, BlinkMacSystemFont, Segoe UI`.

- **headline-display:** Route159 61px at weight 700, line height 1.25. Page title (h1).
- **headline-lg:** Route159 39px at weight 700, line height 1.25. Section headings (h2).
- **headline-md:** Route159 22.5px at weight 700, line height 1.5. Sub-section headings.
- **body-md:** Roboto Flex Variable 16px at weight 300, line height 1.5. Body text.
- **body-lg:** Route159 19px at weight 700, line height 1.5. Lead paragraphs.
- **body-sm:** Roboto Flex Variable 14px at weight 300, line height 1. Secondary and small text.
- **label-md:** Roboto Flex Variable 16px at weight 700, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (73% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 10px, lg 24px, xl 64px.
- **Sections:** 112px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #506FB2 borders.

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **sm (16px):** 48 elements.
- **md (24px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Explore”):** #28395F fill, #FFFFFF text, 14px/300, 16px radius, padding 10px 14px.
- **button-outline (“Download Nix 2.35.4”):** #3B5487 fill, #FFFFFF text, 16px/700, 16px radius, padding 8px 24px.
- **button-secondary (“Search”):** #4D6FB7 fill, #FFFFFF text, 16px/700, 24px radius, padding 10px 32px.
- **button-ghost (“Search”):** transparent fill, 16px/700, 24px radius, padding 10px 32px.
- **link:** transparent fill, #EEEEEE text, padding 0px.

## Do's and Don'ts

- Do use #3B5487 for the page.
- Do keep text in 4 levels: #FFFFFF, #EEEEEE, #000000, #0B0B0B.
- Do use #28395F as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 10px, 24px).
- Do use 16px corners on most elements; larger surfaces also use 24px.
- Don't use #000000 for body text; it reaches 2.80:1 on #3B5487. Keep it for large text or metadata.
- Don't use #0B0B0B for body text; it reaches 2.63:1 on #3B5487. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Route159 and Roboto Flex Variable.
- Don't use #28395F for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/nixos.org/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
