---
version: alpha
name: Gusto
description: "Light interface measured from gusto.com: Boogy Brut type with Matter, dark cyan accents, tonal surfaces and 8px corners."
colors:
  background: "#FDFDFB"
  surface: "#FDFDFB"
  on-surface: "#1C1B1A"
  on-background: "#1C1B1A"
  on-surface-variant: "#03393D"
  on-surface-muted: "#56514E"
  surface-container-low: "#FFFFFF"
  overlay: "#FFFFFF4D"
  overlay-strong: "#1C1B1A4D"
  outline: "#D1CECC"
  outline-variant: "#FFFFFF"
  primary: "#0F6469"
  on-primary: "#FFFFFF"
  secondary: "#1E7676"
  tertiary: "#FFA5B4"
typography:
  headline-display:
    fontFamily: Boogy Brut
    fontSize: 110px
    fontWeight: 400
    lineHeight: 1.05
  headline-lg:
    fontFamily: Boogy Brut
    fontSize: 72px
    fontWeight: 700
    lineHeight: 1
  headline-md:
    fontFamily: Matter
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.5
  headline-sm:
    fontFamily: Matter
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.2
  title-lg:
    fontFamily: Matter
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.3
  body-md:
    fontFamily: Matter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Matter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Matter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Matter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Boogy Brut
    fontSize: 52px
    fontWeight: 400
    lineHeight: 1.05
rounded:
  sm: 8px
  md: 12px
  lg: 14px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 24px
  section: 96px
  margin: 56px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 0px 2px 0px
    height: 56px
  button-primary-hover:
    backgroundColor: "#357D81"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 0px 2px 0px
    height: 42px
  button-outline-hover:
    backgroundColor: "#F0F0F0"
    textColor: "{colors.on-surface}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 8px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Gusto Design System

## Overview

Gusto describes itself as: “Gusto | Gusto offers fully integrated online HR services: payroll, benefits and everything else.” The interface is light, built on **Snow (#FDFDFB)** with **Charcoal (#1C1B1A)** text, and **Dark Cyan (#0F6469)** as the main accent.

Type is set in **Boogy Brut** and **Matter**. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 8px.

Measured from [gusto.com](https://gusto.com/) on November 4, 2026 at 1440×900 and 390×844 from 435 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #FF8316, #3FA199, #CE63DE, #FF5765.

- **Snow (#FDFDFB):** Page background, seen 27 times. Token `background`.
- **Charcoal (#1C1B1A):** Primary text and headings, seen 66 times. Token `on-surface`, CSS `--gwb-input-neutral-color-border-active`.
- **Deep Cyan (#03393D):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Warm Slate (#56514E):** Muted text and metadata, seen 5 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`, CSS `--gwb-button-tertiary-inverse-color-text-default`.
- **White 30% (#FFFFFF4D):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Charcoal 30% (#1C1B1A4D):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Silver (#D1CECC):** Borders and dividers, seen 29 times. Token `outline`.
- **White (#FFFFFF):** Secondary dividers, seen 2 times. Token `outline-variant`, CSS `--gwb-button-tertiary-inverse-color-text-default`.
- **Dark Cyan (#0F6469):** Primary buttons and calls to action, seen 2 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Cyan (#1E7676):** Accent (CSS variable), seen 10 times. Token `secondary`, CSS `--gwb-color-brand-primary-text-default`.
- **Light Red (#FFA5B4):** Accent (CSS variable). Token `tertiary`.

## Typography

**Boogy Brut** and **Matter** share the interface. Fallback stack: `Boogy Brut, Georgia, serif`.

- **headline-display:** Boogy Brut 110px at weight 400, line height 1.05 (52px on mobile). Page title (h1).
- **headline-lg:** Boogy Brut 72px at weight 700, line height 1. Section headings (h2).
- **headline-md:** Matter 32px at weight 600, line height 1.5. Sub-section headings.
- **headline-sm:** Matter 24px at weight 500, line height 1.2. Card and feature titles.
- **title-lg:** Matter 20px at weight 400, line height 1.3. Small titles.
- **body-md:** Matter 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Matter 18px at weight 400, line height 1.5. Lead paragraphs.
- **label-md:** Matter 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Matter 14px at weight 500, line height 1. Small labels and badges.

## Layout

Spacing follows a 4px grid: 92% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Page margin:** 56px on each side of full-width sections.
- **Breakpoints:** 400px, 426px, 500px, 530px, 550px, 600px, 768px, 896px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF) and #D1CECC borders.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 196 elements.
- **lg (14px):** 136 elements.
- **md (12px):** 40 elements.
- **full (9999px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Create free account”):** #0F6469 fill, #FFFFFF text, 16px/400, 12px radius, padding 0px 0px 2px 0px.
- **button-primary-hover:** background #357D81, text #FFFFFF on hover.
- **button-outline (“Create free account”):** #FFFFFF fill, #03393D text, 16px/400, 12px radius, padding 0px 0px 2px 0px.
- **button-outline-hover:** background #F0F0F0, text #1C1B1A on hover.
- **button-ghost (“Products”):** transparent fill, #1C1B1A text, 16px/400, 8px radius, padding 8px.
- **link:** transparent fill, #56514E text, padding 0px.

## Do's and Don'ts

- Do use #FDFDFB for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 3 levels: #1C1B1A, #03393D, #56514E.
- Do reserve #0F6469 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do use 8px corners on most elements; larger surfaces also use 14px and 12px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Boogy Brut and Matter.
- Don't use #0F6469 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.1s, 0.32s. Longer ambient animations run 8s.

- **Easing:** `ease`, `ease-out`, `cubic-bezier(0.22, 1, 0.36, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/gusto.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
