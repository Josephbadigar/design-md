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
  surface-container: "#F4FBF7"
  surface-container-high: "#F9F7F6"
  surface-container-highest: "#FFEFE5"
  overlay: "#25221E12"
  outline: "#25221E2E"
  outline-variant: "#25221E1F"
  primary: "#E34432"
  on-primary: "#FFFFFF"
  secondary: "#0F66AE"
  tertiary: "#297ABC"
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
    fontWeight: 600
    lineHeight: 1.28
    letterSpacing: -0.005em
  headline-md:
    fontFamily: Graphik
    fontSize: 22px
    fontWeight: 600
    lineHeight: 1.28
  body-md:
    fontFamily: Graphik
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.75
    letterSpacing: 0.005em
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: 0.01em
  label-md:
    fontFamily: Inter
    fontSize: 15.5px
    fontWeight: 500
    lineHeight: 1.35
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Inter
    fontSize: 14.5px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.013em
  headline-display-mobile:
    fontFamily: Graphik
    fontSize: 37px
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Graphik
    fontSize: 28px
    fontWeight: 600
    lineHeight: 1.28
    letterSpacing: -0.005em
  headline-md-mobile:
    fontFamily: Graphik
    fontSize: 19px
    fontWeight: 600
    lineHeight: 1.28
rounded:
  sm: 8px
  md: 10px
  lg: 15px
spacing:
  xs: 4px
  sm: 7px
  md: 9px
  lg: 24px
  xl: 48px
  gutter: 12px
  margin: 24px
  container: 1312px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 9px 14px
    height: 39px
  button-primary-hover:
    backgroundColor: "#CF3520"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 9px 14px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 7px 32px 7px 35px
  card:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 24px 24px 12px 24px
  link:
    textColor: "#25221EA8"
---

# Todoist Design System

## Overview

Todoist describes itself as: “Trusted by 30 million people and teams. Todoist is the world's favorite task manager and to-do list app. Finally become focused, organized and calm.” The interface is light, built on **Snow (#FEFDFC)** with **Warm Charcoal (#25221E)** text, and **Red (#E34432)** as the main accent.

Type is set in **Graphik** and **Inter**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [todoist.com](https://www.todoist.com/) on October 29, 2026 at 1440×900 and 390×844 from 399 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles, plus gradient stops #EE6449.

- **Snow (#FEFDFC):** Page background, seen 1 time. Token `background`.
- **Warm Charcoal (#25221E):** Primary text and headings, seen 49 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 9 times. Token `on-surface-strong`.
- **Slate (#6F6D6A):** Secondary text, seen 28 times. Token `on-surface-variant`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 19 times. Token `surface-container-low`.
- **Snow (#F4FBF7):** Cards and panels, seen 1 time. Token `surface-container`.
- **Snow (#F9F7F6):** Hover and pressed fills, seen 6 times. Token `surface-container-high`.
- **Pale Orange (#FFEFE5):** Highest raised elements, seen 3 times. Token `surface-container-highest`.
- **Warm Charcoal 7% (#25221E12):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Warm Charcoal 18% (#25221E2E):** Borders and dividers, seen 20 times. Token `outline`.
- **Warm Charcoal 12% (#25221E1F):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Red (#E34432):** Primary buttons and calls to action, seen 10 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#0F66AE):** Accent in text, fills and borders, seen 8 times. Token `secondary`.
- **Blue (#297ABC):** Accent in text, fills and borders, seen 2 times. Token `tertiary`.

## Typography

**Graphik** and **Inter** share the interface. Fallback stack: `Graphik-1bbd4a4c7a2fb472, Graphik-1bbd4a4c7a2fb472 fallback: Arial, Helvetica Neue, Helvetica`. Other loaded fonts: Inter-5486e50ce5a4efdf, Graphik-1bbd4a4c7a2fb472, Shantell Sans-5a9740f6b2ed8488.

- **headline-display:** Graphik 55px at weight 600, line height 1.15, tracking -0.01em (37px on mobile). Page title (h1).
- **headline-lg:** Graphik 38px at weight 600, line height 1.28, tracking -0.005em (28px on mobile). Section headings (h2).
- **headline-md:** Graphik 22px at weight 600, line height 1.28 (19px on mobile). Sub-section headings.
- **body-md:** Graphik 16px at weight 400, line height 1. Body text.
- **body-lg:** Inter 18px at weight 500, line height 1.75, tracking 0.005em. Lead paragraphs.
- **label-lg:** Inter 16px at weight 500, line height 1.6, tracking 0.01em. Large buttons and tabs.
- **label-md:** Inter 15.5px at weight 500, line height 1.35, tracking 0.01em. Buttons, navigation and labels.
- **label-sm:** Inter 14.5px at weight 500, line height 1.5, tracking 0.013em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 51% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 7px, md 9px, lg 24px, xl 48px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1312px.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 376px, 768px, 1200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(37, 34, 30, 0.04) 0px 1px 0px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 200 elements.
- **md (10px):** 80 elements.
- **lg (15px):** 80 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for free”):** #E34432 fill, #FFFFFF text, 15.5px/600, 8px radius, padding 9px 14px.
- **button-primary-hover:** background #CF3520, text #FFFFFF on hover.
- **button-ghost (“Personal”):** transparent fill, #25221E text, 15.5px/500, 8px radius, padding 9px 14px.
- **input-field (“Select your language”):** transparent fill, #25221E text, 14.5px/500, 8px radius, padding 7px 32px 7px 35px.
- **card:** transparent fill, #25221E text, 16px/400, 10px radius, padding 24px 24px 12px 24px.
- **link:** transparent fill, #25221EA8 text, padding 0px.

## Do's and Don'ts

- Do use #FEFDFC for the page and lift surfaces in small steps: #FFFFFF, #F4FBF7, #F9F7F6, #FFEFE5.
- Do keep text in 3 levels: #25221E, #000000, #6F6D6A.
- Do reserve #E34432 for primary actions and key highlights.
- Do set headlines in Graphik with tight tracking (-0.01em).
- Do reuse the measured spacing steps (7px, 9px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 10px and 15px.
- Don't introduce new font families beyond Graphik and Inter.
- Don't use #E34432 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.5s.

- **Easing:** `cubic-bezier(0.2, 0.8, 0.2, 1)`, `linear(0 0%, 0.941 11.2%, 1.203 18.3%, 1.196 22.7%, 0.962 40.7%, 1.007 62.9%, 1 100%)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/todoist.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
