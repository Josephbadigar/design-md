---
version: alpha
name: Bubble
description: "Light interface measured from bubble.io: Manrope type with Open Sans, dark indigo accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1A1A1A"
  on-background: "#1A1A1A"
  on-surface-variant: "#525252"
  surface-container-low: "#F5FAFF"
  outline: "#E4EAF1"
  outline-variant: "#AFC0D4"
  primary: "#0C29AB"
  on-primary: "#FFFFFF"
  secondary: "#FED39C"
  tertiary: "#DBA5DE"
typography:
  headline-display:
    fontFamily: Manrope
    fontSize: 51px
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Manrope
    fontSize: 40px
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.031em
  headline-sm:
    fontFamily: Manrope
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.2
  body-md:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Manrope
    fontSize: 19px
    fontWeight: 600
    lineHeight: 1.5
  label-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
  label-sm:
    fontFamily: Open Sans
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1.33
  headline-lg-mobile:
    fontFamily: Manrope
    fontSize: 35px
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: -0.029em
  headline-md-mobile:
    fontFamily: Manrope
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.036em
rounded:
  sm: 4px
  md: 100px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 60px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px
    height: 32px
  button-primary-hover:
    backgroundColor: "#091E7C"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 4px 12px
    height: 30px
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.primary}"
    typography: "{typography.label-sm}"
    rounded: 3px
    padding: 7px 8px
    height: 30px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 16px
  card:
    backgroundColor: "{colors.background}"
    textColor: "#000000"
    typography: "{typography.label-md}"
    rounded: 8px
    padding: 0px
---

# Bubble Design System

## Overview

Bubble describes itself as: “Build with AI when you want speed, edit visually when you want precision — design, database, logic, and privacy rules. Go from idea to launched app fast.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1A1A1A)** text, and **Dark Indigo (#0C29AB)** as the main accent.

Type is set in **Manrope** and **Open Sans**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [bubble.io](https://bubble.io/) on November 4, 2026 at 1440×900 and 390×844 from 174 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 9 times. Token `background`, CSS `--cc-primary_contrast`.
- **Charcoal (#1A1A1A):** Primary text and headings, seen 29 times. Token `on-surface`.
- **Slate (#525252):** Secondary text, seen 4 times. Token `on-surface-variant`, CSS `--color_coIvQ4_default`.
- **Cool Snow (#F5FAFF):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--cc-cobalt-10`.
- **Cool Mist (#E4EAF1):** Borders and dividers, seen 4 times. Token `outline`.
- **Light Blue (#AFC0D4):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--cc-livid-40`.
- **Dark Indigo (#0C29AB):** Primary buttons and calls to action, seen 8 times. Token `primary`, CSS `--color_coIJl2_default`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Orange (#FED39C):** Accent in logos and imagery. Token `secondary`.
- **Light Purple (#DBA5DE):** Accent in logos and imagery. Token `tertiary`.

## Typography

**Manrope** and **Open Sans** share the interface. Fallback stack: `Manrope`. Other loaded fonts: Reddit Mono, founders grotesk medium, founders grotesk regular, founders grotesk semibold.

- **headline-display:** Manrope 51px at weight 800, line height 1.2, tracking -0.02em. Page title (h1).
- **headline-lg:** Manrope 40px at weight 800, line height 1.2, tracking -0.025em (35px on mobile). Section headings (h2).
- **headline-md:** Manrope 32px at weight 700, line height 1.2, tracking -0.031em (28px on mobile). Sub-section headings.
- **headline-sm:** Manrope 20px at weight 600, line height 1.2. Card and feature titles.
- **body-md:** Manrope 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Manrope 19px at weight 600, line height 1.5. Lead paragraphs.
- **label-md:** Manrope 16px at weight 700, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Open Sans 12px at weight 600, line height 1.33. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (87% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 60px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 500px, 630px, 768px, 992px, 993px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.03) 2px 4px 6px 0px`
- `rgba(0, 0, 0, 0.06) 2px 4px 16px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 112 elements.
- **md (100px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start building”):** #0C29AB fill, #FFFFFF text, 12px/600, 4px radius, padding 8px.
- **button-primary-hover:** background #091E7C, text #FFFFFF on hover.
- **button-outline (“SaaS platform”):** #FFFFFF fill, #1A1A1A text, 14px/400, 4px radius, padding 4px 12px, border 1px solid #E4EAF1, shadow `rgba(0, 0, 0, 0.03) 2px 4px 6px 0px`.
- **button-ghost (“Web”):** #F5FAFF fill, #0C29AB text, 12px/600, 3px radius, padding 7px 8px.
- **input-field (“An internal tool to manage my te”):** transparent fill, #1A1A1A text, 14px/400, padding 16px.
- **card:** #FFFFFF fill, #000000 text, 16px/400, 8px radius, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5FAFF.
- Do keep text in 2 levels: #1A1A1A, #525252.
- Do reserve #0C29AB for primary actions and key highlights.
- Do set headlines in Manrope with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 4px corners on most elements; larger surfaces also use 100px.
- Don't introduce new font families beyond Manrope and Open Sans.
- Don't use #0C29AB for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s. Longer ambient animations run 0.9s, 0.8s.

- **Easing:** `ease`, `cubic-bezier(0.2, 0.7, 0.2, 1)`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/bubble.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
