---
version: alpha
name: Dropbox
description: "Light interface measured from dropbox.com: Sharp Grotesk type with Sharp Grotesk 23, vivid blue accents, tonal surfaces and 16px corners."
colors:
  background: "#F7F5F2"
  surface: "#F7F5F2"
  on-surface: "#1E1919"
  on-background: "#1E1919"
  on-surface-variant: "#70695E"
  surface-container-low: "#FFFFFF"
  overlay: "#A6917133"
  primary: "#0061FE"
  on-primary: "#F7F5F2"
  secondary: "#0044AF"
  tertiary: "#CD2F7B"
typography:
  headline-display:
    fontFamily: Sharp Grotesk
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.2
  headline-lg:
    fontFamily: Sharp Grotesk 23
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.2
  headline-md:
    fontFamily: Sharp Grotesk
    fontSize: 26px
    fontWeight: 500
    lineHeight: 1.3
  headline-sm:
    fontFamily: Atlas Grotesk Web
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
  body-md:
    fontFamily: Times New Roman
    fontSize: 16px
    fontWeight: 400
  body-lg:
    fontFamily: Sharp Grotesk
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.2
  body-sm:
    fontFamily: Atlas Grotesk Web
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.57
  headline-display-mobile:
    fontFamily: Sharp Grotesk
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.2
  headline-lg-mobile:
    fontFamily: Sharp Grotesk 23
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.2
rounded:
  sm: 12px
  md: 16px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
    height: 40px
  button-primary-hover:
    backgroundColor: "#0057E5"
  button-ghost:
    textColor: "{colors.on-surface}"
    rounded: 0px
    padding: 16px 12px
  card:
    backgroundColor: "#1C1D21"
    textColor: "#000000"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 8px
  link:
    textColor: "{colors.on-primary}"
---

# Dropbox Design System

## Overview

Dropbox describes itself as: “Discover Dropbox – secure, easy cloud storage for file sharing and collaboration. With Dash, save time and organize all your company content in one place.” The interface is light, built on **Snow (#F7F5F2)** with **Charcoal (#1E1919)** text, and **Vivid Blue (#0061FE)** as the main accent.

Type is set in **Sharp Grotesk** and **Sharp Grotesk 23**. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 16px.

Measured from [dropbox.com](https://www.dropbox.com/) on October 29, 2026 at 1440×900 and 390×844 from 407 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **Snow (#F7F5F2):** Page background. Token `background`, CSS `--color__inverse__core__primary`.
- **Charcoal (#1E1919):** Primary text and headings, seen 31 times. Token `on-surface`, CSS `--dwg-theme__color__standard__text`.
- **Warm Slate (#70695E):** Secondary text, seen 13 times. Token `on-surface-variant`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Orange 20% (#A6917133):** Translucent fill for cards and controls, seen 1 time. Token `overlay`, CSS `--color__faint__border`.
- **Vivid Blue (#0061FE):** Primary buttons and calls to action, seen 9 times. Token `primary`, CSS `--color__core__accent`.
- **Snow (#F7F5F2):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#0044AF):** Accent in the logo, seen 4 times. Token `secondary`.
- **Pink (#CD2F7B):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.

## Typography

**Sharp Grotesk**, **Sharp Grotesk 23**, **Atlas Grotesk Web** and **Times New Roman** share the interface. Fallback stack: `Sharp Grotesk, SharpGrotesk, Sharp Grotesk KR, Sharp Grotesk Thai`.

- **headline-display:** Sharp Grotesk 40px at weight 500, line height 1.2 (32px on mobile). Page title (h1).
- **headline-lg:** Sharp Grotesk 23 32px at weight 400, line height 1.2 (24px on mobile). Section headings (h2).
- **headline-md:** Sharp Grotesk 26px at weight 500, line height 1.3. Sub-section headings.
- **headline-sm:** Atlas Grotesk Web 20px at weight 500, line height 1.2. Card and feature titles.
- **body-md:** Times New Roman 16px at weight 400. Body text.
- **body-lg:** Sharp Grotesk 18px at weight 500, line height 1.2. Lead paragraphs.
- **body-sm:** Atlas Grotesk Web 14px at weight 400, line height 1.57. Secondary and small text.

## Layout

Spacing follows a 4px grid: 95% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 48px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 480px, 648px, 767px, 768px, 1024px, 1279px, 1280px, 1344px, 1440px, 1920px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF).

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **md (16px):** 8 elements.
- **sm (12px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #0061FE fill, #F7F5F2 text, 16px/400, 12px radius, padding 0px 12px, border 2px solid #0061FE.
- **button-primary-hover:** background #0057E5, text #F7F5F2 on hover.
- **button-ghost (“Products”):** transparent fill, #1E1919 text, 13.3333px/400, padding 16px 12px.
- **card:** #1C1D21 fill, #000000 text, 16px/400, 16px radius, padding 8px.
- **link:** transparent fill, #F7F5F2 text, padding 0px.

## Do's and Don'ts

- Do use #F7F5F2 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 2 levels: #1E1919, #70695E.
- Do reserve #0061FE for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do use 16px corners on most elements; larger surfaces also use 12px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Sharp Grotesk, Sharp Grotesk 23, Atlas Grotesk Web and Times New Roman.
- Don't use #0061FE for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.1s, 0.125s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.6, 1)`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/dropbox.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
