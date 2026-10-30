---
version: alpha
name: Sentry
description: "Dark interface measured from sentry.io: Dammit Sans type with Rubik, indigo accents, flat surfaces and 8px corners."
colors:
  background: "#1F1633"
  surface: "#1F1633"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  overlay: "#FFFFFF2E"
  outline: "#584674"
  primary: "#6A5FC1"
  on-primary: "#FFFFFF"
  secondary: "#FD44B0"
  tertiary: "#C2EF4E"
typography:
  headline-display:
    fontFamily: Dammit Sans
    fontSize: 88px
    fontWeight: 700
    lineHeight: 1.2
  headline-lg:
    fontFamily: Dammit Sans
    fontSize: 60px
    fontWeight: 500
    lineHeight: 1.1
  headline-md:
    fontFamily: Rubik
    fontSize: 27px
    fontWeight: 500
    lineHeight: 1.25
  headline-sm:
    fontFamily: Rubik
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.25
  body-md:
    fontFamily: Rubik
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
  label-lg:
    fontFamily: Rubik
    fontSize: 16px
    fontWeight: 400
    lineHeight: 2
  label-md:
    fontFamily: Rubik
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.25
  label-sm:
    fontFamily: Rubik
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.29
  headline-display-mobile:
    fontFamily: Dammit Sans
    fontSize: 50px
    fontWeight: 500
    lineHeight: 1.2
  headline-lg-mobile:
    fontFamily: Dammit Sans
    fontSize: 45px
    fontWeight: 700
    lineHeight: 1.15
rounded:
  sm: 6px
  md: 8px
  lg: 12px
  xl: 13px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 34.85px
  gutter: 20px
  section: 128px
components:
  button-primary:
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 40px
  button-secondary:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 12px 16px
  input-field:
    backgroundColor: "#422082"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 8px 16px
  link:
    textColor: "{colors.on-surface}"
---

# Sentry Design System

## Overview

Sentry describes itself as: “Application performance monitoring for developers & software teams to see errors clearer, solve issues faster & continue learning continuously. Get started at sentry.io.” The interface is dark, built on **Deep Violet (#1F1633)** with **White (#FFFFFF)** text, and **Indigo (#6A5FC1)** as the main accent.

Type is set in **Dammit Sans** and **Rubik**. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [sentry.io](https://sentry.io/welcome/) on October 29, 2026 at 1440×900 and 390×844 from 417 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles, plus gradient stops #FA7FAA, #FF9691, #FFB287, #C83852.

- **Deep Violet (#1F1633):** Page background, seen 4 times. Token `background`, CSS `--bg-primary`.
- **White (#FFFFFF):** Primary text and headings, seen 74 times. Token `on-surface`, CSS `--tw-ring-offset-color`.
- **White 18% (#FFFFFF2E):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Dark Violet (#584674):** Borders and dividers, seen 1 time. Token `outline`, CSS `--color-md-violet`.
- **Indigo (#6A5FC1):** Most used accent color, seen 12 times. Token `primary`, CSS `--color-blurple`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Pink (#FD44B0):** Accent in text, fills and borders, seen 5 times. Token `secondary`, CSS `--color-hot-pink`.
- **Lime (#C2EF4E):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.

## Typography

**Dammit Sans** and **Rubik** share the interface. Fallback stack: `Dammit Sans, sans-serif`.

- **headline-display:** Dammit Sans 88px at weight 700, line height 1.2 (50px on mobile). Page title (h1).
- **headline-lg:** Dammit Sans 60px at weight 500, line height 1.1 (45px on mobile). Section headings (h2).
- **headline-md:** Rubik 27px at weight 500, line height 1.25. Sub-section headings.
- **headline-sm:** Rubik 24px at weight 500, line height 1.25. Card and feature titles.
- **body-md:** Rubik 14px at weight 400, line height 1.71. Body text.
- **label-lg:** Rubik 16px at weight 400, line height 2. Large buttons and tabs.
- **label-md:** Rubik 15px at weight 500, line height 1.25. Buttons, navigation and labels.
- **label-sm:** Rubik 14px at weight 500, line height 1.29. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (85% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 34.85px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Breakpoints:** 576px, 640px, 767px, 768px, 991px, 992px, 1024px, 1151px, 1152px, 1440px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights:

- `rgba(0, 0, 0, 0.15) 0px 2px 10px 0px inset`
- `rgba(0, 0, 0, 0.1) 0px 1px 3px 0px inset`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0.08) 0px 2px 8px 0px`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 68 elements.
- **sm (6px):** 4 elements.
- **lg (12px):** 4 elements.
- **xl (13px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“GET STARTED”):** transparent fill, #1F1633 text, 14px/700, 8px radius, padding 12px 16px.
- **button-secondary (“GET DEMO”):** transparent fill, #FFFFFF text, 14px/700, 8px radius, padding 12px 16px.
- **button-ghost (“PLATFORM”):** transparent fill, #FFFFFF text, 14px/500, 8px radius, padding 12px 16px.
- **input-field (“Installation Dropdown 23”):** #422082 fill, #FFFFFF text, 16px/500, 8px radius, padding 8px 16px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #1F1633 for the page.
- Do reserve #6A5FC1 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do use 8px corners on most elements; larger surfaces also use 6px, 12px and 13px.
- Don't use heavy drop shadows; keep depth to hairline rings.
- Don't introduce new font families beyond Dammit Sans and Rubik.
- Don't use #6A5FC1 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.15s. Longer ambient animations run 0.8s, 0.75s.

- **Easing:** `ease-out`, `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/sentry.io/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
