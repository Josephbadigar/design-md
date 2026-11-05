---
version: alpha
name: Stability AI
description: "Dark interface measured from stability.ai: Archivo type with Figtree, light violet accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#1E1E1E"
  surface: "#1E1E1E"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#E5E7E6"
  on-surface-muted: "#BCBCBC"
  on-surface-subtle: "#888888"
  surface-container-low: "#000000"
  overlay: "#1E1E1E80"
  outline: "#60606099"
  primary: "#A381FF"
  on-primary: "#1E1E1E"
  inverse-surface: "#EEEEEE"
typography:
  headline-display:
    fontFamily: Archivo
    fontSize: 42px
    fontWeight: 400
    lineHeight: 0.98
  headline-lg:
    fontFamily: Archivo
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.05
  headline-md:
    fontFamily: Archivo
    fontSize: 26px
    fontWeight: 700
    lineHeight: 1.18
  headline-sm:
    fontFamily: Archivo
    fontSize: 24.5px
    fontWeight: 600
    lineHeight: 1.27
  title-lg:
    fontFamily: Archivo
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.25
  body-md:
    fontFamily: Archivo
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.25
  body-sm:
    fontFamily: Archivo
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.56
  caption:
    fontFamily: Archivo
    fontSize: 12px
    fontWeight: 400
  label-lg:
    fontFamily: Archivo
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Figtree
    fontSize: 14px
    fontWeight: 600
  label-sm:
    fontFamily: Archivo
    fontSize: 12px
    fontWeight: 700
    lineHeight: 1.07
  headline-lg-mobile:
    fontFamily: Archivo
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.23
rounded:
  xs: 11px
  sm: 15px
  md: 90.51px
  lg: 99px
  xl: 300px
  full: 9999px
spacing:
  sm: 8px
  md: 10px
  lg: 20px
  xl: 41px
  gutter: 8px
  section: 60px
  margin: 30px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.xl}"
    padding: 11.2px 20.8px
    height: 43px
  button-outline:
    backgroundColor: "#191919"
    textColor: "{colors.on-surface-subtle}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 11.4px 0px 13.69px
    height: 34px
  button-ghost:
    textColor: "{colors.primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 11px 22px
    height: 43px
  input-field:
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 12px 10px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Stability AI Design System

## Overview

Stability AI describes itself as: “Stability AI is the enterprise-ready creative partner for teams and creators, delivering professional-grade generative AI tools and solutions for content production at scale.” The interface is dark, built on **Charcoal (#1E1E1E)** with **White (#FFFFFF)** text, and **Light Violet (#A381FF)** as the main accent.

Type is set in **Archivo** and **Figtree**. Headlines run large; body text is 18px. The surface language is flat. Controls are pill-shaped.

Measured from [stability.ai](https://stability.ai/) on November 4, 2026 at 1440×900 and 390×844 from 252 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles, plus gradient stops #2F253AE6, #D9CBFF.

- **Charcoal (#1E1E1E):** Page background, seen 2 times. Token `background`, CSS `--tweak-product-basic-item-gallery-controls-color`.
- **White (#FFFFFF):** Primary text and headings, seen 23 times. Token `on-surface`, CSS `--siteBackgroundColor`.
- **Mist (#E5E7E6):** Secondary text, seen 10 times. Token `on-surface-variant`, CSS `--tweak-summary-block-background-color`.
- **Silver (#BCBCBC):** Muted text and metadata, seen 30 times. Token `on-surface-muted`.
- **Gray (#888888):** Subtle text and placeholders, seen 6 times. Token `on-surface-subtle`.
- **Near Black (#000000):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **Charcoal 50% (#1E1E1E80):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Slate 60% (#60606099):** Borders and dividers, seen 2 times. Token `outline`.
- **Light Violet (#A381FF):** Primary buttons and calls to action, seen 30 times. Token `primary`.
- **Charcoal (#1E1E1E):** Text and icons on primary. Token `on-primary`.
- **Mist (#EEEEEE):** High-contrast fills, seen 1 time. Token `inverse-surface`.

## Typography

**Archivo** and **Figtree** share the interface. Fallback stack: `Archivo`.

- **headline-display:** Archivo 42px at weight 400, line height 0.98. Page title (h1).
- **headline-lg:** Archivo 32px at weight 700, line height 1.05 (28px on mobile). Section headings (h2).
- **headline-md:** Archivo 26px at weight 700, line height 1.18. Sub-section headings.
- **headline-sm:** Archivo 24.5px at weight 600, line height 1.27. Card and feature titles.
- **title-lg:** Archivo 20px at weight 700, line height 1.25. Small titles.
- **body-md:** Archivo 18px at weight 400, line height 1.25. Body text.
- **body-sm:** Archivo 13px at weight 400, line height 1.56. Secondary and small text.
- **caption:** Archivo 12px at weight 400. Captions and fine print.
- **label-lg:** Archivo 18px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** Figtree 14px at weight 600. Buttons, navigation and labels.
- **label-sm:** Archivo 12px at weight 700, line height 1.07. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 33% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 8px, md 10px, lg 20px, xl 41px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 30px on each side of full-width sections.
- **Breakpoints:** 320px, 400px, 425px, 426px, 530px, 550px, 600px, 640px, 767px, 768px, 896px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#000000) and #60606099 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **xl (300px):** 44 elements.
- **full (9999px):** 40 elements.
- **xs (11px):** 16 elements.
- **lg (99px):** 8 elements.
- **sm (15px):** 4 elements.
- **md (90.51px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get in touch”):** #A381FF fill, #1E1E1E text, 16px/600, 300px radius, padding 11.2px 20.8px, border 1px solid #A381FF.
- **button-outline (“ISOLATE SFX”):** #191919 fill, #888888 text, 17.728px/400, 90.512px radius, padding 0px 11.4px 0px 13.69px, border 1px solid #60606099.
- **button-ghost (“Start creating”):** transparent fill, #A381FF text, 14px/600, 300px radius, padding 11px 22px, border 2px solid #A381FF.
- **input-field:** transparent fill, #FFFFFF text, 16px/400, 99px radius, padding 12px 10px, border 1px solid #FFFFFF.
- **card:** #1E1E1E fill, #FFFFFF text, 16px/400, padding 0px.
- **link:** transparent fill, #FFFFFFB3 text, padding 0px.

## Do's and Don'ts

- Do use #1E1E1E for the page and lift surfaces in small steps: #000000.
- Do keep text in 4 levels: #FFFFFF, #E5E7E6, #BCBCBC, #888888.
- Do reserve #A381FF for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 10px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 300px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Archivo and Figtree.
- Don't use #A381FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.55s.

## Motion

Interface transitions are quick: 0.25s, 0.1s, 0.17s, 0.55s. Longer ambient animations run 8s.

- **Easing:** `ease`, `ease-in-out`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/stability.ai/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
