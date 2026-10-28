---
version: alpha
name: Todoist
description: "Light interface measured from todoist.com: Graphik type with Inter, red accents, tonal surfaces and 8px corners."
colors:
  background: "#FEFDFC"
  surface: "#FEFDFC"
  on-surface: "#25221E"
  on-background: "#25221E"
  on-surface-strong: "#000000"
  on-surface-variant: "#6F6D6A"
  surface-container-low: "#FFFFFF"
  surface-container: "#F9F7F6"
  surface-container-high: "#EBF5F0"
  overlay: "#25221ED4"
  overlay-strong: "#25221E12"
  outline: "#25221E2E"
  primary: "#E34432"
  on-primary: "#FFFFFF"
  secondary: "#0F66AE"
  tertiary: "#297ABC"
  error: "#EE6449"
typography:
  headline-display:
    fontFamily: Graphik
    fontSize: 55px
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Graphik
    fontSize: 38px
    fontWeight: 700
    lineHeight: 1.28
    letterSpacing: -0.005em
  body-md:
    fontFamily: Graphik
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  body-lg:
    fontFamily: Graphik
    fontSize: 22px
    fontWeight: 600
    lineHeight: 1.28
  body-sm:
    fontFamily: Inter
    fontSize: 14.5px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.013em
  label-lg:
    fontFamily: Inter
    fontSize: 15.5px
    fontWeight: 500
    lineHeight: 1.35
    letterSpacing: 0.01em
  label-md:
    fontFamily: Inter
    fontSize: 14.5px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.013em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.025em
  headline-display-mobile:
    fontFamily: Graphik
    fontSize: 37px
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: -0.01em
rounded:
  sm: 8px
  md: 10px
  lg: 15px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 9px
  lg: 24px
  xl: 48px
  gutter: 16px
  section: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 9px 14px
    height: 39px
  button-primary-hover:
    backgroundColor: "#CF3520"
  button-secondary:
    backgroundColor: "#E44232"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 9px 14px
    height: 39px
  button-secondary-hover:
    backgroundColor: "#F85646"
  button-ghost:
    textColor: "#6F6D6B"
    typography: "{typography.body-md}"
    padding: 0px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 7px 32px 7px 35px
  card:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "#25221EA8"
---

# Todoist Design System

## Overview

Todoist describes itself as: “Trusted by 30 million people and teams. Todoist is the world's favorite task manager and to-do list app. Finally become focused, organized and calm.” The interface is light, built on **Snow (#FEFDFC)** with **Warm Charcoal (#25221E)** text, and **Red (#E34432)** as the main accent.

Type is set in **Graphik** and **Inter**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [todoist.com](https://www.todoist.com/) on October 21, 2026 at 1440×900 and 390×844 from 292 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **Snow (#FEFDFC):** Page background, seen 1 time. Token `background`.
- **Warm Charcoal (#25221E):** Primary text and headings, seen 42 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 6 times. Token `on-surface-strong`.
- **Slate (#6F6D6A):** Secondary text, seen 50 times. Token `on-surface-variant`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **Snow (#F9F7F6):** Cards and panels, seen 5 times. Token `surface-container`.
- **Mist (#EBF5F0):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Warm Charcoal 83% (#25221ED4):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Warm Charcoal 7% (#25221E12):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Warm Charcoal 18% (#25221E2E):** Borders and dividers, seen 6 times. Token `outline`.
- **Red (#E34432):** Primary buttons and calls to action, seen 10 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#0F66AE):** Most used accent color, seen 5 times. Token `secondary`.
- **Blue (#297ABC):** Most used accent color, seen 3 times. Token `tertiary`.
- **Vivid Red (#EE6449):** Errors and destructive states, seen 4 times. Token `error`.

## Typography

**Graphik** and **Inter** share the interface. Fallback stack: `Graphik-1bbd4a4c7a2fb472, Graphik-1bbd4a4c7a2fb472 fallback: Arial, Helvetica Neue, Helvetica`. Other loaded fonts: Inter-5486e50ce5a4efdf, Inter-5486e50ce5a4efdf fallback: Arial, Graphik-1bbd4a4c7a2fb472, Graphik-1bbd4a4c7a2fb472 fallback: Arial.

- **headline-display:** Graphik 55px at weight 600, line height 1.15, tracking -0.01em (37px on mobile). Page title (h1).
- **headline-lg:** Graphik 38px at weight 700, line height 1.28, tracking -0.005em. Section headings (h2).
- **body-md:** Graphik 16px at weight 400, line height 1. Body text.
- **body-lg:** Graphik 22px at weight 600, line height 1.28. Lead paragraphs.
- **body-sm:** Inter 14.5px at weight 400, line height 1.5, tracking 0.013em. Secondary and small text.
- **label-lg:** Inter 15.5px at weight 500, line height 1.35, tracking 0.01em. Large buttons and tabs.
- **label-md:** Inter 14.5px at weight 500, line height 1.5, tracking 0.013em. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 500, line height 1.5, tracking 0.025em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 48% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 9px, lg 24px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 376px, 768px, 1200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(37, 34, 30, 0.04) 0px 1px 0px 0px`
- `rgba(37, 34, 30, 0.07) 0px 14px 19px -9px, rgba(37, 34, 30, 0.18) 0px 10px 48px 0px`

Hairline rings and inset highlights also appear: `rgb(31, 96, 194) 0px 0px 0px 1px, rgb(220, 234, 255) 0px 0px 0px 4px`.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 160 elements.
- **md (10px):** 44 elements.
- **lg (15px):** 40 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for free”):** #E34432 fill, #FFFFFF text, 15.5px/600, 8px radius, padding 9px 14px.
- **button-primary-hover:** background #CF3520, text #FFFFFF on hover.
- **button-secondary (“Manage Preferences”):** #E44232 fill, #FFFFFF text, 15.5px/600, 8px radius, padding 9px 14px.
- **button-secondary-hover:** background #F85646, text #FFFFFF on hover.
- **button-ghost (“Close this consent banner”):** transparent fill, #6F6D6B text, 16px/400, 50% radius, padding 0px.
- **input-field (“Select your language”):** transparent fill, #25221E text, 14.5px/500, 8px radius, padding 7px 32px 7px 35px.
- **card:** transparent fill, #25221E text, 16px/400, 10px radius, padding 0px, shadow `rgba(37, 34, 30, 0.04) 0px 1px 0px 0px`.
- **link:** transparent fill, #25221EA8 text, padding 0px.

## Do's and Don'ts

- Do use #FEFDFC for the page and lift surfaces in small steps: #FFFFFF, #F9F7F6, #EBF5F0.
- Do keep text in 3 levels: #25221E, #000000, #6F6D6A.
- Do reserve #E34432 for primary actions and key highlights.
- Do set headlines in Graphik with tight tracking (-0.01em).
- Do reuse the measured spacing steps (8px, 9px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 10px and 15px.
- Don't introduce new font families beyond Graphik and Inter.
- Don't use #E34432 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.5s.

- **Easing:** `cubic-bezier(0.2, 0.8, 0.2, 1)`, `ease-out`, `linear(0 0%, 0.941 11.2%, 1.203 18.3%, 1.196 22.7%, 0.962 40.7%, 1.007 62.9%, 1 100%)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/todoist.com/), the free DESIGN.md generator.
