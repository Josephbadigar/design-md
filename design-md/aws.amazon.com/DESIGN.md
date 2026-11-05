---
version: alpha
name: AWS
description: "Light monochrome interface measured from aws.amazon.com: Amazon Ember Display type with Arial, tonal surfaces and 40px corners."
colors:
  background: "#DEDEE3"
  surface: "#DEDEE3"
  on-surface: "#161D26"
  on-background: "#161D26"
  on-surface-variant: "#232B37"
  on-surface-muted: "#A4A4AD"
  surface-container-low: "#CCCCD1"
  surface-container: "#F3F3F7"
  surface-container-high: "#FFFFFF"
  overlay: "#FFFFFFBF"
  overlay-strong: "#0F141ABF"
  outline: "#D1D6DB"
  outline-variant: "#FFFFFF"
  primary: "#161D26"
  on-primary: "#FFFFFF"
  secondary: "#0972D3"
typography:
  headline-display:
    fontFamily: Amazon Ember Display
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.1
  headline-lg:
    fontFamily: Amazon Ember Display
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
  headline-md:
    fontFamily: Amazon Ember Display
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.29
  body-md:
    fontFamily: Amazon Ember Display
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Amazon Ember Display
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.33
  body-sm:
    fontFamily: Amazon Ember Display
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: Arial
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.6
  headline-display-mobile:
    fontFamily: Amazon Ember Display
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.29
  headline-lg-mobile:
    fontFamily: Amazon Ember Display
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
rounded:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
spacing:
  xs: 2px
  sm: 8px
  md: 10px
  lg: 26px
  xl: 64px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.xl}"
    padding: 10px 26px
    height: 44px
  button-secondary:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px
    height: 36px
  button-secondary-hover:
    backgroundColor: "{colors.surface-container}"
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 0px
  input-field:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px 16px
  link:
    textColor: "{colors.on-surface-muted}"
---

# AWS Design System

## Overview

AWS describes itself as: “Amazon Web Services offers reliable, scalable, and inexpensive cloud computing services. Free to join, pay only for what you use.” The interface is light, built on **Mist (#DEDEE3)** with **Cool Charcoal (#161D26)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Amazon Ember Display** and **Arial**. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 40px.

Measured from [aws.amazon.com](https://aws.amazon.com/) on November 4, 2026 at 1440×900 and 390×844 from 397 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #006CE0, #007E94, #008559, #00BD6B.

- **Mist (#DEDEE3):** Page background. Token `background`.
- **Cool Charcoal (#161D26):** Primary text and headings, seen 38 times. Token `on-surface`.
- **Deep Blue (#232B37):** Secondary text, seen 21 times. Token `on-surface-variant`.
- **Cool Gray (#A4A4AD):** Muted text and metadata, seen 11 times. Token `on-surface-muted`.
- **Silver (#CCCCD1):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#F3F3F7):** Cards and panels, seen 23 times. Token `surface-container`.
- **White (#FFFFFF):** Hover and pressed fills, seen 24 times. Token `surface-container-high`.
- **White 75% (#FFFFFFBF):** Translucent fill for cards and controls, seen 5 times. Token `overlay`.
- **Cool Charcoal 75% (#0F141ABF):** Stronger translucent fill, seen 5 times. Token `overlay-strong`.
- **Cool Silver (#D1D6DB):** Borders and dividers, seen 2 times. Token `outline`.
- **White (#FFFFFF):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Cool Charcoal (#161D26):** Primary buttons and calls to action, seen 69 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0972D3):** Accent in text, fills and borders, seen 2 times. Token `secondary`.

## Typography

**Amazon Ember Display** and **Arial** share the interface. Fallback stack: `Amazon Ember Display, Amazon Ember, Helvetica Neue, Helvetica`. Other loaded fonts: Amazon Ember Mono, FontAwesome.

- **headline-display:** Amazon Ember Display 40px at weight 500, line height 1.1 (28px on mobile). Page title (h1).
- **headline-lg:** Amazon Ember Display 32px at weight 500, line height 1.25 (24px on mobile). Section headings (h2).
- **headline-md:** Amazon Ember Display 28px at weight 500, line height 1.29. Sub-section headings.
- **body-md:** Amazon Ember Display 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Amazon Ember Display 18px at weight 500, line height 1.33. Lead paragraphs.
- **body-sm:** Amazon Ember Display 14px at weight 400, line height 1.43. Secondary and small text.
- **label-md:** Arial 14px at weight 400, line height 1.6. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 48% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 10px, lg 26px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 480px, 481px, 699px, 700px, 767px, 768px, 769px, 810px, 1020px, 1023px, 1024px, 1025px, 1279px, 1280px, 1599px, 1600px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#CCCCD1 → #F3F3F7 → #FFFFFF) and #D1D6DB borders.

## Shapes

Most elements use 40px corners. Measured radii, most used first:

- **xl (40px):** 152 elements.
- **sm (8px):** 80 elements.
- **md (16px):** 60 elements.
- **xs (4px):** 44 elements.
- **lg (24px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Create account”):** #161D26 fill, #FFFFFF text, 14px/400, 40px radius, padding 10px 26px.
- **button-secondary (“re:Invent”):** transparent fill, #232B37 text, 14px/400, padding 0px.
- **button-secondary-hover:** background #F3F3F7, text #232B37 on hover.
- **button-ghost (“English”):** transparent fill, #FFFFFF text, 14px/400, 8px radius, padding 0px.
- **input-field (“Search”):** transparent fill, #232B37 text, 16px/400, padding 0px 16px.
- **link:** transparent fill, #A4A4AD text, padding 0px.

## Do's and Don'ts

- Do use #DEDEE3 for the page and lift surfaces in small steps: #CCCCD1, #F3F3F7, #FFFFFF.
- Do keep text in 3 levels: #161D26, #232B37, #A4A4AD.
- Do let contrast carry emphasis; primary actions use #161D26 on #DEDEE3.
- Do reuse the measured spacing steps (8px, 10px, 26px).
- Do use 40px corners on most elements; larger surfaces also use 8px, 16px and 4px.
- Don't use #A4A4AD for body text; it reaches 1.84:1 on #DEDEE3. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Amazon Ember Display and Arial.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.3s, 0.4s.

- **Easing:** `ease`, `cubic-bezier(0, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/aws.amazon.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
