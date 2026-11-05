---
version: alpha
name: Databricks
description: "Dark interface measured from databricks.com: DM Sans type, vivid red accents, tonal surfaces and 20px corners."
colors:
  background: "#0B2026"
  surface: "#0B2026"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#C4CCD6"
  on-surface-muted: "#90A5B1"
  on-surface-subtle: "#5A6F77"
  surface-container-low: "#1B3139"
  overlay: "#EDF2F81A"
  overlay-strong: "#EDF2F80D"
  outline: "#FFFFFF33"
  primary: "#EB1600"
  on-primary: "#FFFFFF"
  secondary: "#016BC1"
  tertiary: "#FF5F46"
typography:
  headline-display:
    fontFamily: DM Sans
    fontSize: 56px
    fontWeight: 500
    lineHeight: 1.21
  headline-lg:
    fontFamily: DM Sans
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.2
  headline-md:
    fontFamily: DM Sans
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
  headline-sm:
    fontFamily: DM Sans
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.29
  title-lg:
    fontFamily: DM Sans
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.33
  body-md:
    fontFamily: DM Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-sm:
    fontFamily: DM Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.67
  label-md:
    fontFamily: DM Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  code:
    fontFamily: DM Mono
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: DM Sans
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.18
  headline-md-mobile:
    fontFamily: DM Sans
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.4
rounded:
  sm: 2px
  md: 20px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 12px
  section: 80px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 12px
    height: 40px
  button-primary-hover:
    backgroundColor: "{colors.surface-container-low}"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 8px 24px
    height: 40px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 24px 12px 20px 12px
  card:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Databricks Design System

## Overview

Databricks describes itself as: “Databricks offers a unified platform for data, analytics and AI. Build better AI with a data-centric approach. Simplify ETL, data warehousing, governance and AI on the Data + AI Platform.” The interface is dark, built on **Deep Cyan (#0B2026)** with **White (#FFFFFF)** text, and **Vivid Red (#EB1600)** as the main accent.

Type is set in **DM Sans**, with **DM Mono** for code. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 20px.

Measured from [databricks.com](https://www.databricks.com/) on November 4, 2026 at 1440×900 and 390×844 from 413 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #90A5B1, #0B2026, #016BC1, #8ACAFF.

- **Deep Cyan (#0B2026):** Page background, seen 5 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 59 times. Token `on-surface`, CSS `--tw-ring-offset-color`.
- **Light Blue (#C4CCD6):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Blue (#90A5B1):** Muted text and metadata, seen 46 times. Token `on-surface-muted`.
- **Cyan (#5A6F77):** Subtle text and placeholders, seen 5 times. Token `on-surface-subtle`.
- **Deep Cyan (#1B3139):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **Cool Mist 10% (#EDF2F81A):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **Cool Mist 5% (#EDF2F80D):** Stronger translucent fill, seen 4 times. Token `overlay-strong`.
- **White 20% (#FFFFFF33):** Borders and dividers, seen 1 time. Token `outline`.
- **Vivid Red (#EB1600):** Primary buttons and calls to action, seen 4 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#016BC1):** Accent in text, fills and borders, seen 13 times. Token `secondary`.
- **Red (#FF5F46):** Accent in text, fills and borders, seen 9 times. Token `tertiary`.

## Typography

**DM Sans** and **DM Mono** (monospace) share the interface. Fallback stack: `DM Sans, sans-serif`. Other loaded fonts: icomoon.

- **headline-display:** DM Sans 56px at weight 500, line height 1.21 (44px on mobile). Page title (h1).
- **headline-lg:** DM Sans 40px at weight 400, line height 1.2. Section headings (h2).
- **headline-md:** DM Sans 32px at weight 500, line height 1.25 (20px on mobile). Sub-section headings.
- **headline-sm:** DM Sans 28px at weight 400, line height 1.29. Card and feature titles.
- **title-lg:** DM Sans 24px at weight 400, line height 1.33. Small titles.
- **body-md:** DM Sans 14px at weight 400, line height 1.43. Body text.
- **body-sm:** DM Sans 12px at weight 400, line height 1.67. Secondary and small text.
- **label-md:** DM Sans 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **code:** DM Mono 16px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing follows a 4px grid: 95% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 360px, 480px, 481px, 767px, 768px, 991px, 1100px, 1280px, 1336px, 1366px, 1536px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(27, 49, 57, 0.07) 0px 72px 104px 0px, rgba(27, 49, 57, 0.05) 0px 32px 40px 0px, rgba(27, 49, 57, 0.04) 0px 16px 24px 0px, rgba(27, 49, 57, 0.035) 0px 9px 13px 0px, rgba(27, 49, 57, 0.04) 0px 4px 8px 0px, rgba(27, 49, 57, 0.02) 0px 2px 3px 0px`

## Shapes

Most elements use 20px corners. Measured radii, most used first:

- **md (20px):** 28 elements.
- **sm (2px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try Databricks”):** #EB1600 fill, #FFFFFF text, 16px/500, padding 12px.
- **button-primary-hover:** background #1B3139, text #FFFFFF on hover.
- **button-outline (“See demo”):** #1B3139 fill, #FFFFFF text, 16px/500, padding 8px 24px.
- **button-secondary (“Platform”):** #FFFFFF fill, #1B3139 text, 16px/700, 20px radius, padding 12px 16px.
- **button-ghost (“Why Databricks”):** transparent fill, #1B3139 text, 16px/400, padding 24px 12px 20px 12px.
- **card:** #FFFFFF fill, #1B3139 text, 16px/400, padding 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(27, 49, 57, 0.07) 0px 72px 104px 0px, rgba(27, 49, 57, 0.05) 0px 32px 40px 0px, rgba(27, 49, 57, 0.04) 0px 16px 24px 0px, rgba(27, 49, 57, 0.035) 0px 9px 13px 0px, rgba(27, 49, 57, 0.04) 0px 4px 8px 0px, rgba(27, 49, 57, 0.02) 0px 2px 3px 0px`.
- **link:** transparent fill, #90A5B1 text, padding 0px.

## Do's and Don'ts

- Do use #0B2026 for the page and lift surfaces in small steps: #1B3139.
- Do keep text in 4 levels: #FFFFFF, #C4CCD6, #90A5B1, #5A6F77.
- Do reserve #EB1600 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do use 20px corners on most elements; larger surfaces also use 2px.
- Don't use #5A6F77 for body text; it reaches 3.18:1 on #0B2026. Keep it for large text or metadata.
- Don't introduce new font families beyond DM Sans and DM Mono.
- Don't use #EB1600 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.2s, 0.075s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.4, 0, 1, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/databricks.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
