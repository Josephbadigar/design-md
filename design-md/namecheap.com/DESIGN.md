---
version: alpha
name: Namecheap
description: "Light interface measured from namecheap.com: GB Museo Sans type, indigo accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#353535"
  on-background: "#353535"
  on-surface-strong: "#1F1F1F"
  on-surface-variant: "#434343"
  on-surface-muted: "#4A4A4A"
  surface-container-low: "#C7C7C7"
  overlay: "#4343430D"
  overlay-strong: "#FFFFFF0D"
  outline: "#EDEDED"
  outline-variant: "#C7C7C7"
  primary: "#42379B"
  on-primary: "#FFFFFF"
  inverse-surface: "#6E6E6E"
  secondary: "#F05422"
  tertiary: "#2165B3"
  error: "#D3321F"
typography:
  headline-display:
    fontFamily: GB Museo Sans
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.5
  headline-lg:
    fontFamily: GB Museo Sans
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.33
  body-md:
    fontFamily: GB Museo Sans
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.5
  body-lg:
    fontFamily: GB Museo Sans
    fontSize: 18px
    fontWeight: 300
    lineHeight: 1.5
  body-sm:
    fontFamily: GB Museo Sans
    fontSize: 14px
    fontWeight: 300
    lineHeight: 1.31
  label-lg:
    fontFamily: GB Museo Sans
    fontSize: 18px
    fontWeight: 700
    lineHeight: 2
  label-md:
    fontFamily: GB Museo Sans
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
  label-sm:
    fontFamily: GB Museo Sans
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.86
  headline-display-mobile:
    fontFamily: GB Museo Sans
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.42
  headline-lg-mobile:
    fontFamily: GB Museo Sans
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.2
rounded:
  xs: 4px
  sm: 6px
  md: 8px
  lg: 10px
  xl: 16px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 64px
  gutter: 8px
  section: 80px
  margin: 64px
components:
  button-primary:
    backgroundColor: "{colors.error}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px 12px
    height: 56px
  button-primary-hover:
    backgroundColor: "#962416"
  button-secondary:
    backgroundColor: "#387070"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 0px 12px
    height: 38px
  button-secondary-hover:
    backgroundColor: "#2B5757"
  button-ghost:
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 8px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 0px 247px 0px 16px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 16px
  link:
    textColor: "{colors.on-primary}"
---

# Namecheap Design System

## Overview

Namecheap describes itself as: “Register domain names at Namecheap. Buy cheap domain names and enjoy 24/7 support. With over 18 million domains under management, you know you’re in good hands.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#353535)** text, and **Indigo (#42379B)** as the main accent.

Type is set in **GB Museo Sans**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [namecheap.com](https://www.namecheap.com/) on November 4, 2026 at 1440×900 and 390×844 from 415 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles.

- **White (#FFFFFF):** Page background, seen 13 times. Token `background`.
- **Graphite (#353535):** Primary text and headings, seen 43 times. Token `on-surface`.
- **Charcoal (#1F1F1F):** Headings and emphasis, seen 14 times. Token `on-surface-strong`.
- **Graphite (#434343):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Graphite (#4A4A4A):** Muted text and metadata, seen 33 times. Token `on-surface-muted`.
- **Silver (#C7C7C7):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Graphite 5% (#4343430D):** Translucent fill for cards and controls, seen 8 times. Token `overlay`.
- **White 5% (#FFFFFF0D):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Mist (#EDEDED):** Borders and dividers, seen 2 times. Token `outline`.
- **Silver (#C7C7C7):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Indigo (#42379B):** Brand color on large areas. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Slate (#6E6E6E):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Vivid Red (#F05422):** Accent in text, fills and borders, seen 5 times. Token `secondary`.
- **Blue (#2165B3):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.
- **Red (#D3321F):** Errors and destructive states, seen 35 times. Token `error`.

## Typography

**GB Museo Sans** carries the whole interface. Fallback stack: `GB Museo Sans, Arial, Helvetica, sans-serif`. Other loaded fonts: gb-icon-font.

- **headline-display:** GB Museo Sans 32px at weight 700, line height 1.5 (24px on mobile). Page title (h1).
- **headline-lg:** GB Museo Sans 24px at weight 700, line height 1.33 (20px on mobile). Section headings (h2).
- **body-md:** GB Museo Sans 16px at weight 300, line height 1.5. Body text.
- **body-lg:** GB Museo Sans 18px at weight 300, line height 1.5. Lead paragraphs.
- **body-sm:** GB Museo Sans 14px at weight 300, line height 1.31. Secondary and small text.
- **label-lg:** GB Museo Sans 18px at weight 700, line height 2. Large buttons and tabs.
- **label-md:** GB Museo Sans 16px at weight 700, line height 1.5. Buttons, navigation and labels.
- **label-sm:** GB Museo Sans 14px at weight 700, line height 1.86. Small labels and badges.

## Layout

Spacing follows a 4px grid: 91% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 64px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 64px on each side of full-width sections.
- **Breakpoints:** 400px, 426px, 479px, 480px, 530px, 550px, 600px, 767px, 768px, 896px, 979px, 980px, 1060px, 1199px, 1200px, 1439px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.16) 0px 2px 4px -1px, rgba(0, 0, 0, 0.05) 0px 4px 5px 0px, rgba(0, 0, 0, 0.08) 0px 1px 10px 0px`
- `rgb(159, 203, 254) 0px 0px 8px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 88 elements.
- **lg (10px):** 80 elements.
- **xs (4px):** 68 elements.
- **xl (16px):** 24 elements.
- **sm (6px):** 16 elements.
- **full (9999px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Search”):** #D3321F fill, #FFFFFF text, 18px/700, 0px 8px 8px 0px radius, padding 0px 12px.
- **button-primary-hover:** background #962416, text #FFFFFF on hover.
- **button-secondary (“Featured”):** #387070 fill, #FFFFFF text, 18px/700, 10px radius, padding 0px 12px.
- **button-secondary-hover:** background #2B5757, text #FFFFFF on hover.
- **button-ghost (“Contact us”):** transparent fill, #4A4A4A text, 16px/700, 8px radius, padding 0px 8px.
- **input-field:** #FFFFFF fill, #353535 text, 18px/700, 8px radius, padding 0px 247px 0px 16px, border 1px solid #2F8EFC, shadow `rgb(159, 203, 254) 0px 0px 8px 0px`.
- **card:** #FFFFFF fill, #4A4A4A text, 16px/300, 16px radius, padding 16px, shadow `rgba(0, 0, 0, 0.16) 0px 2px 4px -1px, rgba(0, 0, 0, 0.05) 0px 4px 5px 0px, rgba(0, 0, 0, 0.08) 0px 1px 10px 0px`.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #C7C7C7.
- Do keep text in 4 levels: #353535, #1F1F1F, #434343, #4A4A4A.
- Do use #42379B as the brand accent: header, logo and key highlights.
- Do keep spacing on the 4px grid.
- Do use 8px corners on most elements; larger surfaces also use 10px, 4px and 16px.
- Don't introduce new font families beyond GB Museo Sans.
- Don't use #42379B for large backgrounds or body text.
- Don't make interface transitions slower than 0.333s.

## Motion

Interface transitions are quick: 0.333s.

- **Easing:** `ease`, `cubic-bezier(0.7, 0.01, 0.3, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/namecheap.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
