---
version: alpha
name: Webflow
description: "Dark interface measured from webflow.com: WF Visual Sans Variable type, vivid blue accents, tonal surfaces and 4px corners."
colors:
  background: "#080808"
  surface: "#080808"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#ABABAB"
  surface-container-low: "#171717"
  outline: "#363636"
  primary: "#146EF5"
  on-primary: "#FFFFFF"
  secondary: "#3B89FF"
typography:
  headline-display:
    fontFamily: WF Visual Sans Variable
    fontSize: 80px
    fontWeight: 600
    lineHeight: 1.04
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: WF Visual Sans Variable
    fontSize: 56px
    fontWeight: 600
    lineHeight: 1.04
  headline-md:
    fontFamily: WF Visual Sans Variable
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.2
  headline-sm:
    fontFamily: WF Visual Sans Variable
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.4
  body-md:
    fontFamily: WF Visual Sans Variable
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: WF Visual Sans Variable
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.6
  label-md:
    fontFamily: WF Visual Sans Variable
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.01em
  label-sm:
    fontFamily: WF Visual Sans Variable
    fontSize: 14.5px
    fontWeight: 550
    lineHeight: 1.2
  headline-display-mobile:
    fontFamily: WF Visual Sans Variable
    fontSize: 46px
    fontWeight: 600
    lineHeight: 1.04
    letterSpacing: -0.01em
  headline-sm-mobile:
    fontFamily: WF Visual Sans Variable
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.4
rounded:
  sm: 4px
  md: 8px
  full: 9999px
spacing:
  xs: 3.2px
  sm: 6px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 32px
  section: 80px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 16px 24px
    height: 51px
  button-primary-hover:
    backgroundColor: "#0055D4"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 1.6px 0.8px 1.6px 3.2px
    height: 31px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 20.77px 0px 19.18px 0px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 24px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Webflow Design System

## Overview

Webflow describes itself as: “Design, build, optimize, and rank in AI search — all in Webflow. Enterprise-grade security, CMS, hosting, and AEO built in. Trusted by over 300k teams.” The interface is dark, built on **Near Black (#080808)** with **White (#FFFFFF)** text, and **Vivid Blue (#146EF5)** as the main accent.

Type is set in **WF Visual Sans Variable**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [webflow.com](https://webflow.com/) on October 21, 2026 at 1440×900 and 390×844 from 309 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Near Black (#080808):** Page background, seen 4 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 75 times. Token `on-surface`.
- **Gray (#ABABAB):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Charcoal (#171717):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`, CSS `--mkto-embed-checkbox-background`.
- **Graphite (#363636):** Borders and dividers, seen 4 times. Token `outline`.
- **Vivid Blue (#146EF5):** Primary buttons and calls to action, seen 6 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#3B89FF):** Most used accent color, seen 6 times. Token `secondary`.

## Typography

**WF Visual Sans Variable** carries the whole interface. Fallback stack: `WF Visual Sans Variable, Arial, sans-serif`.

- **headline-display:** WF Visual Sans Variable 80px at weight 600, line height 1.04, tracking -0.01em (46px on mobile). Page title (h1).
- **headline-lg:** WF Visual Sans Variable 56px at weight 600, line height 1.04. Section headings (h2).
- **headline-md:** WF Visual Sans Variable 32px at weight 600, line height 1.2. Sub-section headings.
- **headline-sm:** WF Visual Sans Variable 20px at weight 500, line height 1.4 (18px on mobile). Card and feature titles.
- **body-md:** WF Visual Sans Variable 16px at weight 400, line height 1.6. Body text.
- **body-sm:** WF Visual Sans Variable 14px at weight 400, line height 1.6. Secondary and small text.
- **label-md:** WF Visual Sans Variable 16px at weight 500, line height 1.2, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** WF Visual Sans Variable 14.5px at weight 550, line height 1.2. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 48% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.2px, sm 6px, md 16px, lg 24px, xl 48px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 32px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 767px, 768px, 991px, 992px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(8, 8, 8, 0.08) 0px 4px 4px 0px, rgba(8, 8, 8, 0.2) 0px 1px 2px 0px, rgba(255, 255, 255, 0.12) 0px 6px 12px 0px inset, rgba(255, 255, 255, 0.2) 0px 1px 1px 0px inset`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 68 elements.
- **md (8px):** 32 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Contact Sales”):** #146EF5 fill, #FFFFFF text, 16px/500, 4px radius, padding 16px 24px.
- **button-primary-hover:** background #0055D4, text #FFFFFF on hover.
- **button-outline (“marketing teams”):** #080808 fill, #FFFFFF text, 16px/400, 4px radius, padding 1.6px 0.8px 1.6px 3.2px, border 1px solid #363636.
- **button-ghost (“Platform”):** transparent fill, #FFFFFF text, 15.9808px/500, padding 20.77px 0px 19.18px 0px.
- **input-field (“Work Email”):** #171717 fill, #FFFFFF text, 16px/400, 4px radius, padding 24px, border 1px solid #5A5A5A, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **link:** transparent fill, #ABABAB text, padding 0px.

## Do's and Don'ts

- Do use #080808 for the page and lift surfaces in small steps: #171717.
- Do keep text in 2 levels: #FFFFFF, #ABABAB.
- Do reserve #146EF5 for primary actions and key highlights.
- Do set headlines in WF Visual Sans Variable with tight tracking (-0.01em).
- Do reuse the measured spacing steps (6px, 16px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 8px.
- Don't introduce new font families beyond WF Visual Sans Variable.
- Don't use #146EF5 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.3s.

- **Easing:** `cubic-bezier(0.165, 0.84, 0.44, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/webflow.com/), the free DESIGN.md generator.
