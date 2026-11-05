---
version: alpha
name: Balsamiq
description: "Light interface measured from balsamiq.com: Lexend type, pink accents, tonal surfaces and 18px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#311C3B"
  on-background: "#311C3B"
  surface-container-low: "#EDE6FF"
  overlay: "#311C3B33"
  overlay-strong: "#F7F2EA66"
  outline: "#D8D8DC"
  primary: "#AE1C59"
  on-primary: "#FFFFFF"
  inverse-surface: "#666666"
  secondary: "#C4215D"
typography:
  headline-display:
    fontFamily: Lexend
    fontSize: 70px
    fontWeight: 500
    lineHeight: 1.15
  headline-lg:
    fontFamily: Lexend
    fontSize: 50px
    fontWeight: 500
    lineHeight: 1.15
  headline-md:
    fontFamily: Lexend
    fontSize: 45px
    fontWeight: 500
    lineHeight: 1.15
  headline-sm:
    fontFamily: Lexend
    fontSize: 35.5px
    fontWeight: 500
    lineHeight: 1.15
  title-lg:
    fontFamily: Lexend
    fontSize: 22.5px
    fontWeight: 600
    lineHeight: 1.4
  body-md:
    fontFamily: Lexend
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.5
  body-lg:
    fontFamily: Lexend
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.5
  body-sm:
    fontFamily: Lexend
    fontSize: 13.5px
    fontWeight: 300
    lineHeight: 1.33
  label-md:
    fontFamily: Lexend
    fontSize: 18px
    fontWeight: 300
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Lexend
    fontSize: 49px
    fontWeight: 500
    lineHeight: 1.15
  headline-lg-mobile:
    fontFamily: Lexend
    fontSize: 37px
    fontWeight: 500
    lineHeight: 1.15
  headline-sm-mobile:
    fontFamily: Lexend
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.15
rounded:
  sm: 9px
  md: 13.5px
  lg: 18px
spacing:
  xs: 4px
  md: 9px
  lg: 18px
  xl: 45px
  gutter: 9px
  section: 90px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 13.5px 27px
    height: 54px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 13.5px 27px
    height: 56px
  button-outline-hover:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 9px 0px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-primary}"
---

# Balsamiq Design System

## Overview

Balsamiq describes itself as: “Wireframes and prototypes without the friction. Balsamiq is the fast wireframing and prototyping tool for product, tech, and business minds. Sketch, test, refine your UI—fast.” The interface is light, built on **White (#FFFFFF)** with **Deep Violet (#311C3B)** text, and **Pink (#AE1C59)** as the main accent.

Type is set in **Lexend**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 18px.

Measured from [balsamiq.com](https://balsamiq.com/) on November 4, 2026 at 1440×900 and 390×844 from 374 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 25 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Deep Violet (#311C3B):** Primary text and headings, seen 65 times. Token `on-surface`, CSS `--color-eggplant`.
- **Pale Violet (#EDE6FF):** Raised areas one step from the page, seen 10 times. Token `surface-container-low`, CSS `--color-light-lavender`.
- **Deep Violet 20% (#311C3B33):** Translucent fill for cards and controls, seen 8 times. Token `overlay`.
- **Warm Mist 40% (#F7F2EA66):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Silver (#D8D8DC):** Borders and dividers, seen 1 time. Token `outline`.
- **Pink (#AE1C59):** Primary buttons and calls to action, seen 11 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Slate (#666666):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Pink (#C4215D):** Accent, seen 16 times. Token `secondary`.

## Typography

**Lexend** carries the whole interface. Fallback stack: `Lexend, sans-serif`. Other loaded fonts: Balsamiq Sans.

- **headline-display:** Lexend 70px at weight 500, line height 1.15 (49px on mobile). Page title (h1).
- **headline-lg:** Lexend 50px at weight 500, line height 1.15 (37px on mobile). Section headings (h2).
- **headline-md:** Lexend 45px at weight 500, line height 1.15. Sub-section headings.
- **headline-sm:** Lexend 35.5px at weight 500, line height 1.15 (28px on mobile). Card and feature titles.
- **title-lg:** Lexend 22.5px at weight 600, line height 1.4. Small titles.
- **body-md:** Lexend 16px at weight 300, line height 1.5. Body text.
- **body-lg:** Lexend 18px at weight 500, line height 1.5. Lead paragraphs.
- **body-sm:** Lexend 13.5px at weight 300, line height 1.33. Secondary and small text.
- **label-md:** Lexend 18px at weight 300, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 4% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, md 9px, lg 18px, xl 45px.
- **Sections:** 90px vertical padding between major sections.
- **Gaps:** 9px is the most common gap in flex and grid layouts.
- **Breakpoints:** 430px, 767px, 768px, 900px, 1050px, 1200px, 1280px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 4px 6px -1px, rgba(0, 0, 0, 0.1) 0px 2px 4px -2px`

## Shapes

Most elements use 18px corners. Measured radii, most used first:

- **lg (18px):** 100 elements.
- **md (13.5px):** 88 elements.
- **sm (9px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try it free”):** #AE1C59 fill, #FFFFFF text, 18px/300, 18px radius, padding 13.5px 27px.
- **button-primary-hover:** background #311C3B, text #FFFFFF on hover.
- **button-outline (“Log in”):** transparent fill, #311C3B text, 18px/300, 18px radius, padding 13.5px 27px, border 1px solid #311C3B.
- **button-outline-hover:** background #311C3B, text #FFFFFF on hover.
- **button-ghost (“Product”):** transparent fill, #311C3B text, 18px/300, 18px radius, padding 9px 0px.
- **card:** #EDE6FF fill, #311C3B text, 18px/300, 18px radius, padding 0px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #EDE6FF.
- Do reserve #AE1C59 for primary actions and key highlights.
- Do reuse the measured spacing steps (9px, 18px).
- Do use 18px corners on most elements; larger surfaces also use 13.5px and 9px.
- Don't introduce new font families beyond Lexend.
- Don't use #AE1C59 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s. Longer ambient animations run 1.1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/balsamiq.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
