---
version: alpha
name: Cash App
description: "Light interface measured from cash.app: Cash Sans type with Arial, vivid green accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#999999"
  outline: "#0000004D"
  primary: "#00E013"
  on-primary: "#000000"
typography:
  headline-display:
    fontFamily: Cash Sans
    fontSize: 56px
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Cash Sans
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.03em
  body-md:
    fontFamily: Cash Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  body-lg:
    fontFamily: Cash Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.03em
  body-sm:
    fontFamily: Cash Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  label-md:
    fontFamily: Arial
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.03em
  label-sm:
    fontFamily: Cash Sans
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-display-mobile:
    fontFamily: Cash Sans
    fontSize: 42px
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: -0.03em
  headline-lg-mobile:
    fontFamily: Cash Sans
    fontSize: 42px
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: -0.03em
rounded:
  md: 100px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 10.5px
  lg: 19.88px
  xl: 40px
  gutter: 10.5px
  section: 90px
  margin: 20px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 14px 19.88px
    height: 42px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 0px 20px
    height: 46px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 0px 20px
    height: 46px
  link:
    textColor: "{colors.on-surface}"
---

# Cash App Design System

## Overview

Cash App describes itself as: “Download Cash App to send & receive money instantly, spend with the Cash App Card, buy bitcoin, invest in stocks, & manage your finances.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Green (#00E013)** as the main accent.

Type is set in **Cash Sans** and **Arial**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [cash.app](https://cash.app/) on November 4, 2026 at 1440×900 and 390×844 from 205 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 6 roles.

- **White (#FFFFFF):** Page background, seen 5 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 72 times. Token `on-surface`.
- **Gray (#999999):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Near Black 30% (#0000004D):** Borders and dividers, seen 4 times. Token `outline`.
- **Vivid Green (#00E013):** Brand color on large areas, seen 3 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.

## Typography

**Cash Sans** and **Arial** share the interface. Fallback stack: `Cash Sans, Helvetica Neue, helvetica, sans-serif`.

- **headline-display:** Cash Sans 56px at weight 400, line height 0.95, tracking -0.03em (42px on mobile). Page title (h1).
- **headline-lg:** Cash Sans 40px at weight 400, line height 1.1, tracking -0.03em (42px on mobile). Section headings (h2).
- **body-md:** Cash Sans 16px at weight 400, line height 1. Body text.
- **body-lg:** Cash Sans 18px at weight 400, line height 1.4, tracking -0.03em. Lead paragraphs.
- **body-sm:** Cash Sans 14px at weight 400, line height 1, tracking -0.02em. Secondary and small text.
- **label-md:** Arial 16px at weight 400, line height 1.2, tracking -0.03em. Buttons, navigation and labels.
- **label-sm:** Cash Sans 12px at weight 500, line height 1.2, tracking -0.02em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 39% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 10.5px, lg 19.88px, xl 40px.
- **Sections:** 90px vertical padding between major sections.
- **Gaps:** 10.5px is the most common gap in flex and grid layouts.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 391px, 400px, 425px, 426px, 550px, 600px, 640px, 758px, 759px, 760px, 896px, 1023px, 1024px, 1400px, 1440px, 1480px, 1680px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #0000004D borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (100px):** 36 elements.
- **full (9999px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #00E013 fill, #000000 text, 14px/400, 100px radius, padding 14px 19.88px.
- **button-secondary (“Log in”):** #000000 fill, #FFFFFF text, 12px/400, 999px radius, padding 0px 20px.
- **button-outline (“Sign up”):** #FFFFFF fill, #000000 text, 12px/500, 999px radius, padding 0px 20px, border 1px solid #000000.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #000000, #999999.
- Do use #00E013 as the brand accent: header, logo and key highlights.
- Do set headlines in Cash Sans with tight tracking (-0.03em).
- Do reuse the measured spacing steps (8px, 10.5px, 19.88px).
- Do make buttons and chips fully rounded (9999px); most other elements use 100px corners.
- Don't use #999999 for body text; it reaches 2.85:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Cash Sans and Arial.
- Don't use #00E013 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.6s, 0.3s, 0.4s, 0.2s.

- **Easing:** `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cash.app/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
