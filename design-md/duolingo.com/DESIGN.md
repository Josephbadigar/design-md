---
version: alpha
name: Duolingo
description: "Light interface measured from duolingo.com: feather type with duolingo-sans, lime accents, flat surfaces and 12px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#4B4B4B"
  on-background: "#4B4B4B"
  on-surface-variant: "#777777"
  outline: "#E5E5E5"
  primary: "#58CC02"
  on-primary: "#FFFFFF"
  secondary: "#A5ED6E"
  tertiary: "#1CB0F6"
typography:
  headline-display:
    fontFamily: feather
    fontSize: 64px
    fontWeight: 700
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: feather
    fontSize: 48px
    fontWeight: 700
  body-md:
    fontFamily: duolingo-sans
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.18
  label-md:
    fontFamily: duolingo-sans
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.47
  label-sm:
    fontFamily: duolingo-sans
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.23
  headline-display-mobile:
    fontFamily: feather
    fontSize: 36px
    fontWeight: 700
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: feather
    fontSize: 36px
    fontWeight: 700
rounded:
  md: 12px
spacing:
  sm: 8px
  md: 12px
  lg: 30px
  gutter: 101px
  section: 96px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 16px
    height: 50px
  button-ghost:
    textColor: "#AFAFAF"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.secondary}"
---

# Duolingo Design System

## Overview

Duolingo describes itself as: “Free, fun, and effective courses in languages and more. Learn with quick, science-based lessons personalized to you.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#4B4B4B)** text, and **Lime (#58CC02)** as the main accent.

Type is set in **feather** and **duolingo-sans**. Headlines run large with tight negative tracking; body text is 17px. The surface language is flat. Corners are mostly 12px.

Measured from [duolingo.com](https://www.duolingo.com/) on October 29, 2026 at 1440×900 and 390×844 from 392 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **White (#FFFFFF):** Page background, seen 6 times. Token `background`.
- **Graphite (#4B4B4B):** Primary text and headings, seen 5 times. Token `on-surface`.
- **Slate (#777777):** Secondary text, seen 47 times. Token `on-surface-variant`.
- **Mist (#E5E5E5):** Borders and dividers, seen 4 times. Token `outline`.
- **Lime (#58CC02):** Primary buttons and calls to action, seen 9 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Lime (#A5ED6E):** Links and interactive text, seen 48 times. Token `secondary`.
- **Vivid Cyan (#1CB0F6):** Accent in text, fills and borders, seen 5 times. Token `tertiary`.

## Typography

**feather** and **duolingo-sans** share the interface. Fallback stack: `feather, sans-serif`.

- **headline-display:** feather 64px at weight 700, tracking -0.02em (36px on mobile). Page title (h1).
- **headline-lg:** feather 48px at weight 700 (36px on mobile). Section headings (h2).
- **body-md:** duolingo-sans 17px at weight 400, line height 1.18. Body text.
- **label-md:** duolingo-sans 15px at weight 700, line height 1.47, uppercase. Buttons, navigation and labels.
- **label-sm:** duolingo-sans 13px at weight 700, line height 1.23. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (80% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** sm 8px, md 12px, lg 30px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 101px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 426px, 530px, 550px, 600px, 896px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #E5E5E5 borders.

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **md (12px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“GET STARTED”):** #58CC02 fill, #FFFFFF text, 15px/700, 12px radius, padding 0px 16px.
- **button-ghost (“SITE LANGUAGE: ENGLISH”):** transparent fill, #AFAFAF text, 15px/700, padding 0px.
- **link:** transparent fill, #A5ED6E text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #4B4B4B, #777777.
- Do reserve #58CC02 for primary actions and key highlights.
- Do set headlines in feather with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 30px).
- Do use 12px corners on most elements.
- Don't use #777777 for body text; it reaches 4.48:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond feather and duolingo-sans.
- Don't use #58CC02 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/duolingo.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
