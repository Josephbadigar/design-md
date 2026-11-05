---
version: alpha
name: Gamma
description: "Light interface measured from gamma.app: ESBuild type with PPMori, dark blue accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#66666B"
  on-background: "#66666B"
  overlay: "#FFFFFFCC"
  outline: "#D0E6FE"
  primary: "#0540AD"
  on-primary: "#FFFFFF"
  secondary: "#002253"
  tertiary: "#0740DF"
typography:
  headline-display:
    fontFamily: ESBuild
    fontSize: 72px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: ESBuild
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.02em
  headline-md:
    fontFamily: PPMori
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: PPMori
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.5
  title-lg:
    fontFamily: PPMori
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.02em
  body-md:
    fontFamily: PPMori
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.2
  label-md:
    fontFamily: PPMori
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: PPMori
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: ESBuild
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.025em
rounded:
  sm: 6px
  md: 24px
  full: 9999px
spacing:
  base: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 96px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 32px
    height: 40px
  button-primary-hover:
    backgroundColor: "#0B2E79"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.secondary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 0px 32px
    height: 48px
  button-outline-hover:
    backgroundColor: "#EBF3FE"
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 16px
  link:
    textColor: "#FAF9F5"
---

# Gamma Design System

## Overview

Gamma describes itself as: “Design stunning presentations, websites, and more with Gamma—your all-in-one AI-powered design partner. No code or design experience needed.” The interface is light, built on **White (#FFFFFF)** with **Slate (#66666B)** text, and **Dark Blue (#0540AD)** as the main accent.

Type is set in **ESBuild** and **PPMori**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [gamma.app](https://gamma.app/) on November 4, 2026 at 1440×900 and 390×844 from 341 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles, plus gradient stops #D0E6FE.

- **White (#FFFFFF):** Page background, seen 7 times. Token `background`, CSS `--chakra-colors-white`.
- **Slate (#66666B):** Primary text and headings, seen 26 times. Token `on-surface`, CSS `--chakra-colors-gray-600`.
- **White 80% (#FFFFFFCC):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Pale Blue (#D0E6FE):** Borders and dividers, seen 4 times. Token `outline`.
- **Dark Blue (#0540AD):** Primary buttons and calls to action, seen 18 times. Token `primary`, CSS `--chakra-colors-blue-800`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Blue (#002253):** Accent on large areas, seen 54 times. Token `secondary`.
- **Vivid Blue (#0740DF):** Accent in text, fills and borders, seen 10 times. Token `tertiary`.

## Typography

**ESBuild** and **PPMori** share the interface. Fallback stack: `ESBuild, sans-serif`.

- **headline-display:** ESBuild 72px at weight 600, line height 1, tracking -0.025em (48px on mobile). Page title (h1).
- **headline-lg:** ESBuild 48px at weight 500, line height 1, tracking -0.02em. Section headings (h2).
- **headline-md:** PPMori 30px at weight 700, line height 1.1, tracking -0.02em. Sub-section headings.
- **headline-sm:** PPMori 24px at weight 500, line height 1.5. Card and feature titles.
- **title-lg:** PPMori 20px at weight 600, line height 1.1, tracking -0.02em. Small titles.
- **body-md:** PPMori 18px at weight 600, line height 1.2. Body text.
- **label-md:** PPMori 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** PPMori 14px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** sm 8px, md 12px, lg 24px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 425px, 426px, 550px, 600px, 640px, 767px, 768px, 896px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 20px 25px -5px, rgba(0, 0, 0, 0.04) 0px 10px 10px -5px`
- `rgba(255, 255, 255, 0.48) 0px 2px 4px 0px`
- `rgba(0, 34, 83, 0.15) 0px 2px 8px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (6px):** 192 elements.
- **full (9999px):** 100 elements.
- **md (24px):** 56 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for free”):** #0540AD fill, #FFFFFF text, 16px/500, 24px radius, padding 0px 32px.
- **button-primary-hover:** background #0B2E79, text #FFFFFF on hover.
- **button-outline (“Start for free”):** #FFFFFF fill, #002253 text, 18px/600, 9999px radius, padding 0px 32px, border 1px solid #D0E6FE, shadow `rgba(255, 255, 255, 0.48) 0px 2px 4px 0px`.
- **button-outline-hover:** background #EBF3FE, text #002253 on hover.
- **button-ghost (“Products”):** transparent fill, #FFFFFFCC text, 16px/500, 24px radius, padding 0px 16px.
- **link:** transparent fill, #FAF9F5 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do reserve #0540AD for primary actions and key highlights.
- Do set headlines in ESBuild with tight tracking (-0.025em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 6px corners.
- Don't introduce new font families beyond ESBuild and PPMori.
- Don't use #0540AD for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s. Longer ambient animations run 0.9s.

- **Easing:** `ease`, `cubic-bezier(0.22, 1, 0.36, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/gamma.app/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
