---
version: alpha
name: IKEA
description: "Light interface measured from ikea.com: Omani Rial type, dark blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFEFB"
  surface: "#FFFEFB"
  on-surface: "#111111"
  on-background: "#111111"
  on-surface-strong: "#000000"
  surface-container-low: "#FFFFFF"
  surface-container: "#DADADA"
  primary: "#0058A3"
  on-primary: "#FFFFFF"
  secondary: "#0000EE"
  tertiary: "#FFF094"
  warning: "#FFDB00"
  success: "#1A7E3B"
typography:
  headline-display:
    fontFamily: Omani Rial
    fontSize: 46px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: Omani Rial
    fontSize: 36.5px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Omani Rial
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.62
  body-md:
    fontFamily: Omani Rial
    fontSize: 16px
    fontWeight: 400
  body-sm:
    fontFamily: Omani Rial
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.57
  label-md:
    fontFamily: Omani Rial
    fontSize: 12px
    fontWeight: 700
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Omani Rial
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.027em
rounded:
  md: 8px
  full: 9999px
spacing:
  xs: 2px
  sm: 7.2px
  md: 16px
  lg: 24px
  xl: 60px
  gutter: 20px
  section: 60px
  margin: 24px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 24px
    padding: 12px 18px
    height: 40px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    padding: 0px
    height: 56px
  button-outline-hover:
    backgroundColor: "#F5F5F5"
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px 0px 12px 42px
  link:
    textColor: "{colors.secondary}"
---

# IKEA Design System

## Overview

IKEA describes itself as: “Furniture, home accessories, design ideas and inspiration for big dreams and small budgets. A better everyday life begins at home!” The interface is light, built on **Snow (#FFFEFB)** with **Charcoal (#111111)** text, and **Dark Blue (#0058A3)** as the main accent.

Type is set in **Omani Rial**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [ikea.com](https://www.ikea.com/) on October 21, 2026 at 1440×900 and 390×844 from 302 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Snow (#FFFEFB):** Page background, seen 4 times. Token `background`, CSS `--breadcrumbs-background`.
- **Charcoal (#111111):** Primary text and headings, seen 49 times. Token `on-surface`, CSS `--breadcrumbs-text-color`.
- **Near Black (#000000):** Headings and emphasis, seen 2 times. Token `on-surface-strong`, CSS `--footer-background-color-override`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 8 times. Token `surface-container-low`, CSS `--light-onetrust`.
- **Silver (#DADADA):** Cards and panels, seen 1 time. Token `surface-container`.
- **Dark Blue (#0058A3):** Brand color on large areas, seen 39 times. Token `primary`, CSS `--confirm-onetrust`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#0000EE):** Links and interactive text, seen 12 times. Token `secondary`.
- **Light Amber (#FFF094):** Brand color on large areas, seen 7 times. Token `tertiary`.
- **Vivid Amber (#FFDB00):** Warnings and highlights, seen 2 times. Token `warning`.
- **Dark Green (#1A7E3B):** Success and positive states, seen 1 time. Token `success`.

## Typography

**Omani Rial** carries the whole interface. Fallback stack: `Omani Rial, Emirati Dirham, Saudi Riyal, Noto IKEA`. Other loaded fonts: Noto IKEA.

- **headline-display:** Omani Rial 46px at weight 700, line height 1.1, tracking -0.035em (28px on mobile). Page title (h1).
- **headline-lg:** Omani Rial 36.5px at weight 700, line height 1.25, tracking -0.03em. Section headings (h2).
- **headline-md:** Omani Rial 20px at weight 400, line height 1.62. Sub-section headings.
- **body-md:** Omani Rial 16px at weight 400. Body text.
- **body-sm:** Omani Rial 14px at weight 400, line height 1.57. Secondary and small text.
- **label-md:** Omani Rial 12px at weight 700, line height 1. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (75% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 7.2px, md 16px, lg 24px, xl 60px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 24px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF → #DADADA).

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (8px):** 54 elements.
- **full (9999px):** 44 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Accept”):** #111111 fill, #FFFFFF text, 12px/700, 24px radius, padding 12px 18px, border 1px solid #111111.
- **button-outline (“Play video of a FRAKTA carrier b”):** #FFFFFF fill, #111111 text, 13.3333px/400, 50% radius, padding 0px.
- **button-outline-hover:** background #F5F5F5, text #111111 on hover.
- **input-field (“Find online store”):** #FFFFFF fill, #000000 text, 16px/400, 8px radius, padding 12px 0px 12px 42px.
- **link:** transparent fill, #0000EE text, padding 0px.

## Do's and Don'ts

- Do use #FFFEFB for the page and lift surfaces in small steps: #FFFFFF, #DADADA.
- Do keep text in 2 levels: #111111, #000000.
- Do use #0058A3 as the brand accent: header, logo and key highlights.
- Do set headlines in Omani Rial with tight tracking (-0.035em).
- Do reuse the measured spacing steps (7.2px, 16px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Omani Rial.
- Don't use #0058A3 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.4s, 0.5s, 0.15s.

- **Easing:** `ease`, `ease-in`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/ikea.com/), the free DESIGN.md generator.
