---
version: alpha
name: wix.com
description: "Light interface measured from wix.com: wix-madefor-display-v2 type with wix-madefor-text-v2, light cyan accents, flat surfaces and 50px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#514B3D"
  primary: "#9FEAFF"
  on-primary: "#000000"
  secondary: "#166AEA"
  tertiary: "#1A6AFF"
typography:
  headline-display:
    fontFamily: wix-madefor-display-v2
    fontSize: 82.5px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: wix-madefor-display-v2
    fontSize: 72px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  headline-md:
    fontFamily: wix-madefor-display-v2
    fontSize: 54px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: wix-madefor-display-v2
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.14
    letterSpacing: -0.02em
  title-lg:
    fontFamily: wix-madefor-display-v2
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  body-md:
    fontFamily: wix-madefor-text-v2
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
  body-lg:
    fontFamily: wix-madefor-display-v2
    fontSize: 19px
    fontWeight: 500
    lineHeight: 1.15
  body-sm:
    fontFamily: Arial
    fontSize: 10px
    fontWeight: 400
  label-md:
    fontFamily: wix-madefor-display-v2
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: wix-madefor-display-v2
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-display-mobile:
    fontFamily: wix-madefor-display-v2
    fontSize: 41px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-md-mobile:
    fontFamily: wix-madefor-display-v2
    fontSize: 17px
    fontWeight: 500
    lineHeight: 1.5
rounded:
  sm: 42px
  md: 50px
  lg: 300px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 30px
  xl: 61.92px
  gutter: 22.5px
  container: 99999px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 0px 10px 0px 34px
    height: 54px
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 8px 30px
    height: 40px
  button-secondary-hover:
    backgroundColor: "#2D83FF"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px 12px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: 3px 194.4px 3px 52px
  link:
    textColor: "{colors.on-surface}"
---

# wix.com Design System

## Overview

wix.com describes itself as: “Get everything you need to build a website your way. Wix’s free, easy-to-use website builder offers 2,000+ templates, built-in AI tools and a custom domain.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Light Cyan (#9FEAFF)** as the main accent.

Type is set in **wix-madefor-display-v2** and **wix-madefor-text-v2**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 50px.

Measured from [wix.com](https://www.wix.com/) on October 21, 2026 at 1440×900 and 390×844 from 455 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles, plus gradient stops #49877E.

- **White (#FFFFFF):** Page background, seen 5 times. Token `background`, CSS `--wst-color-fill-background-primary`.
- **Near Black (#000000):** Primary text and headings, seen 129 times. Token `on-surface`, CSS `--wst-color-line`.
- **Dark Amber (#514B3D):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Light Cyan (#9FEAFF):** Brand color on large areas. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#166AEA):** Secondary buttons, seen 29 times. Token `secondary`.
- **Vivid Blue (#1A6AFF):** Brand accent (CSS variable), seen 24 times. Token `tertiary`.

## Typography

**wix-madefor-display-v2**, **wix-madefor-text-v2** and **Arial** share the interface. Fallback stack: `wix-madefor-display-v2, sans-serif`. Other loaded fonts: madefor-display, madefor-display-bold, madefor-text, madefor-text-mediumbold.

- **headline-display:** wix-madefor-display-v2 82.5px at weight 400, line height 1.2, tracking -0.02em (41px on mobile). Page title (h1).
- **headline-lg:** wix-madefor-display-v2 72px at weight 400, line height 1, tracking -0.02em. Section headings (h2).
- **headline-md:** wix-madefor-display-v2 54px at weight 400, line height 1.1, tracking -0.02em (17px on mobile). Sub-section headings.
- **headline-sm:** wix-madefor-display-v2 48px at weight 400, line height 1.14, tracking -0.02em. Card and feature titles.
- **title-lg:** wix-madefor-display-v2 30px at weight 500, line height 1, tracking -0.02em. Small titles.
- **body-md:** wix-madefor-text-v2 16px at weight 400, line height 1.3. Body text.
- **body-lg:** wix-madefor-display-v2 19px at weight 500, line height 1.15. Lead paragraphs.
- **body-sm:** Arial 10px at weight 400. Secondary and small text.
- **label-md:** wix-madefor-display-v2 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** wix-madefor-display-v2 14px at weight 500, line height 1.1, tracking -0.02em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 48% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 12px, lg 30px, xl 61.92px.
- **Gaps:** 22.5px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 99999px.
- **Breakpoints:** 767px, 768px, 769px, 1099px, 1100px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(133, 154, 255, 0.4) 0px 30px 250px 20px, rgba(139, 142, 238, 0.16) 0px 16px 50px 0px`

## Shapes

Most elements use 50px corners. Measured radii, most used first:

- **md (50px):** 44 elements.
- **full (9999px):** 8 elements.
- **sm (42px):** 4 elements.
- **lg (300px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #000000 fill, #000000 text, 10px/400, 50px radius, padding 0px 10px 0px 34px.
- **button-secondary (“Start for free”):** #166AEA fill, #FFFFFF text, 16px/400, 42px radius, padding 8px 30px.
- **button-secondary-hover:** background #2D83FF, text #FFFFFF on hover.
- **button-ghost (“Product”):** transparent fill, #000000 text, 16px/400, padding 0px 12px.
- **input-field (“Type the domain you want”):** #FFFFFF fill, #000000 text, 22px/400, 999px radius, padding 3px 194.4px 3px 52px, shadow `rgba(133, 154, 255, 0.4) 0px 30px 250px 20px, rgba(139, 142, 238, 0.16) 0px 16px 50px 0px`.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #000000, #514B3D.
- Do use #9FEAFF as the brand accent: header, logo and key highlights.
- Do set headlines in wix-madefor-display-v2 with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 30px).
- Do use 50px corners on most elements; larger surfaces also use 42px and 300px.
- Don't introduce new font families beyond wix-madefor-display-v2, wix-madefor-text-v2 and Arial.
- Don't use #9FEAFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.4s, 0.6s. Longer ambient animations run 12s.

- **Easing:** `ease`, `ease-in-out`, `cubic-bezier(0.2, 1, 0, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/wix.com/), the free DESIGN.md generator.
