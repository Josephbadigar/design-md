---
version: alpha
name: Monzo
description: "Light interface measured from monzo.com: MonzoSansDisplay type with MonzoSansText, red accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#6B747B"
  on-background: "#6B747B"
  on-surface-strong: "#000000"
  on-surface-variant: "#091723"
  surface-container-low: "#F2F8F3"
  outline: "#0917231A"
  primary: "#FF4F40"
  on-primary: "#000000"
  secondary: "#EAA240"
  tertiary: "#EA560D"
  error: "#E30613"
  warning: "#F59E00"
typography:
  headline-display:
    fontFamily: MonzoSansDisplay
    fontSize: 49px
    fontWeight: 800
    lineHeight: 1.2
  headline-lg:
    fontFamily: MonzoSansDisplay
    fontSize: 44px
    fontWeight: 800
    lineHeight: 1.2
  headline-md:
    fontFamily: MonzoSansDisplay
    fontSize: 39px
    fontWeight: 800
    lineHeight: 1.2
  headline-sm:
    fontFamily: MonzoSansDisplay
    fontSize: 31px
    fontWeight: 700
    lineHeight: 1.2
  title-lg:
    fontFamily: MonzoSansDisplay
    fontSize: 25px
    fontWeight: 700
    lineHeight: 1.4
  body-md:
    fontFamily: MonzoSansText
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.4
  label-md:
    fontFamily: MonzoSansText
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  headline-display-mobile:
    fontFamily: MonzoSansDisplay
    fontSize: 41px
    fontWeight: 800
    lineHeight: 1.2
  headline-md-mobile:
    fontFamily: MonzoSansDisplay
    fontSize: 34px
    fontWeight: 800
    lineHeight: 1.2
  title-lg-mobile:
    fontFamily: MonzoSansDisplay
    fontSize: 23px
    fontWeight: 700
    lineHeight: 1.26
rounded:
  xs: 4px
  sm: 16px
  md: 32px
  lg: 64px
  xl: 128px
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 64px
  gutter: 24px
  section: 64px
  margin: 24px
  container: 1568px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 24px
    height: 51px
  button-outline:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 0px
    height: 48px
  button-outline-hover:
    backgroundColor: "{colors.outline}"
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 24px
    height: 48px
  link:
    textColor: "{colors.background}"
---

# Monzo Design System

## Overview

Monzo describes itself as: “Your salary sorted into Pots. Your spare change turned into savings. Your money, doing what it should with Monzo.” The interface is light, built on **White (#FFFFFF)** with **Cool Slate (#6B747B)** text, and **Red (#FF4F40)** as the main accent.

Type is set in **MonzoSansDisplay** and **MonzoSansText**. Headlines run large; body text is 13px. The surface language is flat. Corners are mostly 4px.

Measured from [monzo.com](https://monzo.com/) on October 21, 2026 at 1440×900 and 390×844 from 484 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 10 times. Token `background`.
- **Cool Slate (#6B747B):** Primary text and headings. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 2 times. Token `on-surface-strong`.
- **Deep Blue (#091723):** Secondary text, seen 51 times. Token `on-surface-variant`.
- **Snow (#F2F8F3):** Raised areas one step from the page, seen 15 times. Token `surface-container-low`.
- **Deep Blue 10% (#0917231A):** Borders and dividers, seen 2 times. Token `outline`.
- **Red (#FF4F40):** Brand color in the logo, seen 14 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Orange (#EAA240):** Accent, seen 4 times. Token `secondary`.
- **Vivid Orange (#EA560D):** Accent, seen 4 times. Token `tertiary`.
- **Vivid Red (#E30613):** Errors and destructive states, seen 4 times. Token `error`.
- **Vivid Orange (#F59E00):** Warnings and highlights, seen 4 times. Token `warning`.

## Typography

**MonzoSansDisplay** and **MonzoSansText** share the interface. Fallback stack: `MonzoSansDisplay, sans-serif`.

- **headline-display:** MonzoSansDisplay 49px at weight 800, line height 1.2 (41px on mobile). Page title (h1).
- **headline-lg:** MonzoSansDisplay 44px at weight 800, line height 1.2. Section headings (h2).
- **headline-md:** MonzoSansDisplay 39px at weight 800, line height 1.2 (34px on mobile). Sub-section headings.
- **headline-sm:** MonzoSansDisplay 31px at weight 700, line height 1.2. Card and feature titles.
- **title-lg:** MonzoSansDisplay 25px at weight 700, line height 1.4 (23px on mobile). Small titles.
- **body-md:** MonzoSansText 13px at weight 400, line height 1.4. Body text.
- **label-md:** MonzoSansText 16px at weight 400, line height 1.4. Buttons, navigation and labels.

## Layout

Spacing follows a 8px grid: 90% of measured gaps and paddings are multiples of 8px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1568px.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 600px, 1440px, 1567px, 1568px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F2F8F3) and #0917231A borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **xs (4px):** 156 elements.
- **xl (128px):** 136 elements.
- **md (32px):** 52 elements.
- **sm (16px):** 40 elements.
- **lg (64px):** 30 elements.
- **full (9999px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #091723 fill, #FFFFFF text, 16px/600, 500px radius, padding 12px 24px, border 1px solid #091723.
- **button-outline (“Customise”):** transparent fill, #091723 text, 16px/400, 128px radius, padding 0px, border 2px solid #091723.
- **button-outline-hover:** background #0917231A, text #091723 on hover.
- **button-ghost (“Open a free Monzo account”):** #FFFFFF fill, #091723 text, 16px/600, 500px radius, padding 12px 24px, border 1px solid #FFFFFF.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F2F8F3.
- Do keep text in 3 levels: #6B747B, #000000, #091723.
- Do use #FF4F40 as the brand accent: header, logo and key highlights.
- Do keep spacing on the 8px grid.
- Do use 4px corners on most elements; larger surfaces also use 128px, 32px and 16px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond MonzoSansDisplay and MonzoSansText.
- Don't use #FF4F40 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.1s.

- **Easing:** `cubic-bezier(0, 0, 1, 1)`, `ease`, `cubic-bezier(0.22, 0, 0.12, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/monzo.com/), the free DESIGN.md generator.
