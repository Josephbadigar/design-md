---
version: alpha
name: Dinamo
description: "Light interface measured from abcdinamo.com: Monument Grotesk type, vivid yellow accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  surface-container-low: "#E6E9EB"
  surface-container: "#D9D9D9"
  primary: "#FFEA00"
  on-primary: "#000000"
  secondary: "#0052FF"
typography:
  headline-display:
    fontFamily: Monument Grotesk
    fontSize: 74px
    fontWeight: 400
    lineHeight: 0.9
  headline-lg:
    fontFamily: Monument Grotesk
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.1
  headline-md:
    fontFamily: Monument Grotesk
    fontSize: 24.5px
    fontWeight: 400
    lineHeight: 1.1
  body-md:
    fontFamily: Monument Grotesk
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.1
  body-sm:
    fontFamily: Monument Grotesk
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.3
  label-md:
    fontFamily: Monument Grotesk
    fontSize: 9px
    fontWeight: 400
    lineHeight: 1.1
  code:
    fontFamily: Monument Grotesk Mono
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.02em
  headline-display-mobile:
    fontFamily: Monument Grotesk
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: Monument Grotesk Mono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.02em
rounded:
  xs: 8.88px
  sm: 10.25px
  md: 13.66px
  lg: 23.91px
  xl: 32.79px
  full: 9999px
spacing:
  xs: 2.73px
  sm: 6.83px
  md: 9.56px
  lg: 20.49px
  xl: 33.06px
  gutter: 29.29px
  section: 109.85px
  margin: 13.66px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 11.61px
    padding: 0px 0px 0px 6.83px
    height: 29px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: 11.61px
    padding: 0px 0px 0px 6.83px
    height: 29px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px 0px 0px 6.83px
  input-field:
    textColor: "{colors.background}"
    typography: "{typography.headline-lg}"
    rounded: "{rounded.sm}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Dinamo Design System

## Overview

Dinamo describes itself as: “Dinamo is a Berlin-based type design studio offering retail and bespoke typefaces, design software, research, and consultancy.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Yellow (#FFEA00)** as the main accent.

Type is set in **Monument Grotesk**, with **Monument Grotesk Mono** for code. Headlines run large; body text is 19px. The surface language is flat. Controls are pill-shaped.

Measured from [abcdinamo.com](https://abcdinamo.com/) on November 4, 2026 at 1440×900 and 390×844 from 256 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`, CSS `--buttonHighlightFont`.
- **Near Black (#000000):** Primary text and headings, seen 100 times. Token `on-surface`, CSS `--buttonHighlightBackground`.
- **Mist (#E6E9EB):** Raised areas one step from the page, seen 33 times. Token `surface-container-low`, CSS `--featureBackground`.
- **Silver (#D9D9D9):** Cards and panels, seen 1 time. Token `surface-container`.
- **Vivid Yellow (#FFEA00):** Brand color on large areas, seen 1 time. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0052FF):** Accent on large areas, seen 1 time. Token `secondary`.

## Typography

**Monument Grotesk** and **Monument Grotesk Mono** (monospace) share the interface. Fallback stack: `Monument Grotesk, Helvetica Neue, Helvetica, Arial`. Other loaded fonts: DinamoLoading, bng-rg-A, cnt-nl-A, cnt-flt-A.

- **headline-display:** Monument Grotesk 74px at weight 400, line height 0.9, uppercase (44px on mobile). Page title (h1).
- **headline-lg:** Monument Grotesk 30px at weight 400, line height 1.1 (12px on mobile). Section headings (h2).
- **headline-md:** Monument Grotesk 24.5px at weight 400, line height 1.1. Sub-section headings.
- **body-md:** Monument Grotesk 19px at weight 400, line height 1.1. Body text.
- **body-sm:** Monument Grotesk 15px at weight 400, line height 1.3. Secondary and small text.
- **label-md:** Monument Grotesk 9px at weight 400, line height 1.1. Buttons, navigation and labels.
- **code:** Monument Grotesk Mono 15px at weight 400, line height 1.3, tracking -0.02em. Code and technical values.

## Layout

Spacing does not follow a strict grid: 0% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2.73px, sm 6.83px, md 9.56px, lg 20.49px, xl 33.06px.
- **Sections:** 109.85px vertical padding between major sections.
- **Gaps:** 29.29px is the most common gap in flex and grid layouts.
- **Page margin:** 13.66px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#E6E9EB → #D9D9D9).

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **xs (8.88px):** 44 elements.
- **full (9999px):** 24 elements.
- **md (13.66px):** 8 elements.
- **sm (10.25px):** 4 elements.
- **lg (23.91px):** 4 elements.
- **xl (32.79px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Trial fonts”):** #E6E9EB fill, #000000 text, 9.15391px/400, 11.6122px radius, padding 0px 0px 0px 6.83px.
- **button-secondary (“Bag (0)”):** #000000 fill, #FFFFFF text, 9.15391px/400, 11.6122px radius, padding 0px 0px 0px 6.83px.
- **button-ghost (“Trial fonts”):** transparent fill, #000000 text, 9.15391px/400, padding 0px 0px 0px 6.83px.
- **input-field (“Email*”):** transparent fill, #FFFFFF text, 30.0552px/400, 10.2461px radius, padding 0px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #E6E9EB, #D9D9D9.
- Do use #FFEA00 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (6.83px, 9.56px, 20.49px).
- Do make buttons and chips fully rounded (9999px); most other elements use 8.88px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Monument Grotesk and Monument Grotesk Mono.
- Don't use #FFEA00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.25s, 0.5s, 0.1s. Longer ambient animations run 1s, 2s, 5.2s.

- **Easing:** `cubic-bezier(0.55, 0.08, 0, 1)`, `cubic-bezier(0.1, 0.6, 0.4, 1)`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/abcdinamo.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
