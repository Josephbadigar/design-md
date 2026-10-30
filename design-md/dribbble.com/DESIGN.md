---
version: alpha
name: Dribbble
description: "Light interface measured from dribbble.com: Mona Sans type, pink accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0D0C22"
  on-background: "#0D0C22"
  on-surface-strong: "#060318"
  on-surface-variant: "#524B63"
  on-surface-muted: "#BEB9CA"
  surface-container-low: "#FAF9FB"
  surface-container: "#ECEBF0"
  overlay: "#EA4C891A"
  outline: "#E7E7E9"
  outline-variant: "#FAF9FB"
  primary: "#EA4C89"
  on-primary: "#FFFFFF"
  inverse-surface: "#3A3546"
typography:
  headline-display:
    fontFamily: Mona Sans
    fontSize: 52px
    fontWeight: 600
    lineHeight: 1.2
  body-md:
    fontFamily: Mona Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 2
  body-lg:
    fontFamily: Mona Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.75
  label-lg:
    fontFamily: Mona Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.38
  label-md:
    fontFamily: Mona Sans
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  label-sm:
    fontFamily: Mona Sans
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Mona Sans
    fontSize: 27px
    fontWeight: 600
    lineHeight: 1.2
rounded:
  sm: 4px
  md: 8px
  lg: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 5px
  md: 16px
  lg: 24px
  xl: 36px
  gutter: 8px
  margin: 72px
  container: 1650px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    padding: 0px
    height: 40px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    padding: 0px 24px
    height: 48px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    padding: 4px 16px 4px 4px
    height: 40px
  input-field:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px 0px 0px 24px
  link:
    textColor: "{colors.on-surface}"
---

# Dribbble Design System

## Overview

Dribbble describes itself as: “Find Top Designers & Creative Professionals on Dribbble. We are where designers gain inspiration, feedback, community, and jobs. Your best resource to discover and connect with designers worldwide.” The interface is light, built on **White (#FFFFFF)** with **Deep Indigo (#0D0C22)** text, and **Pink (#EA4C89)** as the main accent.

Type is set in **Mona Sans**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [dribbble.com](https://dribbble.com/) on October 29, 2026 at 1440×900 and 390×844 from 333 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 12 times. Token `background`, CSS `--btn-text-color-hover`.
- **Deep Indigo (#0D0C22):** Primary text and headings, seen 85 times. Token `on-surface`.
- **Deep Indigo (#060318):** Headings and emphasis, seen 6 times. Token `on-surface-strong`.
- **Dark Violet (#524B63):** Secondary text, seen 16 times. Token `on-surface-variant`.
- **Cool Silver (#BEB9CA):** Muted text and metadata, seen 9 times. Token `on-surface-muted`.
- **Snow (#FAF9FB):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Mist (#ECEBF0):** Cards and panels, seen 16 times. Token `surface-container`.
- **Pink 10% (#EA4C891A):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Mist (#E7E7E9):** Borders and dividers, seen 9 times. Token `outline`.
- **Snow (#FAF9FB):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Pink (#EA4C89):** Primary buttons and calls to action, seen 6 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Cool Graphite (#3A3546):** High-contrast fills, seen 8 times. Token `inverse-surface`.

## Typography

**Mona Sans** carries the whole interface. Fallback stack: `Mona Sans, Helvetica Neue, Helvetica, Arial`.

- **headline-display:** Mona Sans 52px at weight 600, line height 1.2 (27px on mobile). Page title (h1).
- **body-md:** Mona Sans 14px at weight 400, line height 2. Body text.
- **body-lg:** Mona Sans 16px at weight 400, line height 1.75. Lead paragraphs.
- **label-lg:** Mona Sans 16px at weight 500, line height 1.38. Large buttons and tabs.
- **label-md:** Mona Sans 14px at weight 600, line height 1.43. Buttons, navigation and labels.
- **label-sm:** Mona Sans 13px at weight 600, line height 1. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 49% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 5px, md 16px, lg 24px, xl 36px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1650px.
- **Page margin:** 72px on each side of full-width sections.
- **Breakpoints:** 500px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.14) 0px 3px 6px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 96 elements.
- **md (8px):** 4 elements.
- **lg (12px):** 4 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Search”):** #EA4C89 fill, #FFFFFF text, 13px/600, 50% radius, padding 0px, border 1px solid #EA4C89.
- **button-secondary (“Log in”):** #0D0C22 fill, #FFFFFF text, 14px/600, 1e+07px radius, padding 0px 24px, border 1px solid #0D0C22.
- **button-outline (“Panthera Designs”):** #FFFFFF fill, #0D0C22 text, 12px/500, 1e+07px radius, padding 4px 16px 4px 4px, shadow `rgba(0, 0, 0, 0.14) 0px 3px 6px 0px`.
- **input-field (“What type of design are you inte”):** transparent fill, #060318 text, 14px/400, 12px radius, padding 0px 0px 0px 24px.
- **link:** transparent fill, #0D0C22 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAF9FB, #ECEBF0.
- Do keep text in 4 levels: #0D0C22, #060318, #524B63, #BEB9CA.
- Do reserve #EA4C89 for primary actions and key highlights.
- Do reuse the measured spacing steps (5px, 16px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 8px and 12px.
- Don't use #BEB9CA for body text; it reaches 1.91:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Mona Sans.
- Don't use #EA4C89 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.1s, 0.05s, 0.2s, 0.6s. Longer ambient animations run 0.7s.

- **Easing:** `ease`, `cubic-bezier(0.32, 0, 0.59, 0.03)`, `cubic-bezier(0.34, 1.56, 0.64, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/dribbble.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
