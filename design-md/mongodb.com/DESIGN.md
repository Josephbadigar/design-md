---
version: alpha
name: MongoDB
description: "Dark interface measured from mongodb.com: Sohne Condensed type with Sohne, vivid green accents, tonal surfaces and 12px corners."
colors:
  background: "#061621"
  surface: "#061621"
  on-surface: "#FAFBFC"
  on-background: "#FAFBFC"
  on-surface-variant: "#E7EEEC"
  on-surface-muted: "#B8C4C2"
  surface-container-low: "#14242F"
  outline: "#21313C"
  outline-variant: "#FFFFFF1A"
  primary: "#00ED64"
  on-primary: "#061621"
  secondary: "#00684A"
  tertiary: "#3D6BF5"
typography:
  headline-display:
    fontFamily: Sohne Condensed
    fontSize: 101px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Sohne Condensed
    fontSize: 96px
    fontWeight: 700
    lineHeight: 1
  headline-md:
    fontFamily: Sohne Condensed
    fontSize: 56px
    fontWeight: 700
    lineHeight: 0.95
  headline-sm:
    fontFamily: Sohne Condensed
    fontSize: 36px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.01em
  title-lg:
    fontFamily: Sohne Condensed
    fontSize: 20px
    fontWeight: 700
    lineHeight: 0.95
  body-md:
    fontFamily: Sohne
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Sohne
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-lg:
    fontFamily: Sohne
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: Sohne
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.33
  label-sm:
    fontFamily: Sohne
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  code:
    fontFamily: Sohne Mono
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: 0.1em
  headline-display-mobile:
    fontFamily: Sohne Condensed
    fontSize: 33px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.01em
  headline-md-mobile:
    fontFamily: Sohne Condensed
    fontSize: 34px
    fontWeight: 700
    lineHeight: 0.95
  title-lg-mobile:
    fontFamily: Sohne Condensed
    fontSize: 18px
    fontWeight: 700
    lineHeight: 0.95
rounded:
  sm: 8px
  md: 12px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 36px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: 4px
    padding: 15px 24px
    height: 48px
  button-secondary:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
    height: 36px
  button-tertiary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 8px 20px
    height: 40px
  button-ghost:
    textColor: "#FFFFFF"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  input-field:
    textColor: "#FFFFFF"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "#001E2B"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# MongoDB Design System

## Overview

MongoDB describes itself as: “MongoDB is the intelligent data platform for the AI era. Get your ideas to market faster with flexible, real-time data that scales across any cloud.” The interface is dark, built on **Deep Blue (#061621)** with **Snow (#FAFBFC)** text, and **Vivid Green (#00ED64)** as the main accent.

Type is set in **Sohne Condensed** and **Sohne**, with **Sohne Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 12px.

Measured from [mongodb.com](https://www.mongodb.com/) on October 29, 2026 at 1440×900 and 390×844 from 361 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Deep Blue (#061621):** Page background, seen 23 times. Token `background`, CSS `--color-link-inline-hover`.
- **Snow (#FAFBFC):** Primary text and headings, seen 58 times. Token `on-surface`, CSS `--icon-primary`.
- **Mist (#E7EEEC):** Secondary text, seen 6 times. Token `on-surface-variant`, CSS `--color-surface-knockout-secondary`.
- **Silver (#B8C4C2):** Muted text and metadata, seen 6 times. Token `on-surface-muted`.
- **Deep Blue (#14242F):** Raised areas one step from the page, seen 28 times. Token `surface-container-low`.
- **Deep Blue (#21313C):** Borders and dividers, seen 55 times. Token `outline`, CSS `--color-surface-secondary`.
- **White 10% (#FFFFFF1A):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Vivid Green (#00ED64):** Primary buttons and calls to action, seen 10 times. Token `primary`.
- **Deep Blue (#061621):** Text and icons on primary. Token `on-primary`.
- **Deep Teal (#00684A):** Secondary buttons, seen 7 times. Token `secondary`, CSS `--color-state-link-cta-hover`.
- **Vivid Blue (#3D6BF5):** Secondary buttons, seen 1 time. Token `tertiary`.

## Typography

**Sohne Condensed**, **Sohne** and **Sohne Mono** (monospace) share the interface. Fallback stack: `Sohne Condensed, Helvetica Neue, Helvetica, Arial`. Other loaded fonts: MongoDB Value Serif, Noto Sans KR.

- **headline-display:** Sohne Condensed 101px at weight 700, line height 0.95, tracking -0.01em, uppercase (33px on mobile). Page title (h1).
- **headline-lg:** Sohne Condensed 96px at weight 700, line height 1. Section headings (h2).
- **headline-md:** Sohne Condensed 56px at weight 700, line height 0.95 (34px on mobile). Sub-section headings.
- **headline-sm:** Sohne Condensed 36px at weight 700, line height 0.95, tracking -0.01em. Card and feature titles.
- **title-lg:** Sohne Condensed 20px at weight 700, line height 0.95 (18px on mobile). Small titles.
- **body-md:** Sohne 16px at weight 400, line height 1.5. Body text.
- **body-sm:** Sohne 12px at weight 400, line height 1.33. Secondary and small text.
- **label-lg:** Sohne 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** Sohne 15px at weight 500, line height 1.33. Buttons, navigation and labels.
- **label-sm:** Sohne 14px at weight 500, line height 1.43. Small labels and badges.
- **code:** Sohne Mono 12px at weight 500, line height 1.33, tracking 0.1em, uppercase. Code and technical values.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 36px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 460px, 768px, 1024px, 1025px, 1280px, 1281px, 1374px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(6, 22, 33, 0.06) 0px 1px 2px 0px, rgba(6, 22, 33, 0.04) 0px 4px 12px 0px`

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **md (12px):** 152 elements.
- **sm (8px):** 116 elements.
- **full (9999px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #00ED64 fill, #061621 text, 16px/500, 4px radius, padding 15px 24px, border 1px solid #00ED64.
- **button-secondary (“Builder”):** #3D6BF5 fill, #FAFBFC text, 14px/500, 8px radius, padding 8px 16px.
- **button-tertiary (“Learn more”):** #FAFBFC fill, #061621 text, 16px/500, 8px radius, padding 8px 20px.
- **button-ghost (“Products”):** transparent fill, #FFFFFF text, 16px/400, padding 0px.
- **input-field (“Ask MongoDB Assistant”):** transparent fill, #FFFFFF text, 14px/400, padding 0px.
- **card:** #001E2B fill, #061621 text, 16px/400, 12px radius, padding 0px, border 1px solid #FFFFFF1A.
- **link:** transparent fill, #FAFBFC text, padding 0px.

## Do's and Don'ts

- Do use #061621 for the page and lift surfaces in small steps: #14242F.
- Do keep text in 3 levels: #FAFBFC, #E7EEEC, #B8C4C2.
- Do reserve #00ED64 for primary actions and key highlights.
- Do set headlines in Sohne Condensed with tight tracking (-0.01em).
- Do keep spacing on the 4px grid.
- Do use 12px corners on most elements; larger surfaces also use 8px.
- Don't introduce new font families beyond Sohne Condensed, Sohne and Sohne Mono.
- Don't use #00ED64 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.3s, 0.24s. Longer ambient animations run 0.7s.

- **Easing:** `ease`, `cubic-bezier(0.2, 0, 0, 1)`, `cubic-bezier(0.33, 1, 0.68, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mongodb.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
