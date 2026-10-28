---
version: alpha
name: Headspace
description: "Light interface measured from headspace.com: Headspace Apercu type, vivid blue accents, tonal surfaces and 32px corners."
colors:
  background: "#F9F4F2"
  surface: "#F9F4F2"
  on-surface: "#2D2C2B"
  on-background: "#2D2C2B"
  on-surface-variant: "#44423F"
  on-surface-muted: "#4B4C4D"
  on-surface-subtle: "#63605D"
  surface-container-low: "#FFFFFF"
  outline: "#C6C1B9"
  outline-variant: "#E2DED9"
  primary: "#0061EF"
  on-primary: "#FFFFFF"
  secondary: "#1A0C54"
  tertiary: "#FF76B8"
  warning: "#FFCE00"
typography:
  headline-display:
    fontFamily: Headspace Apercu
    fontSize: 64px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Headspace Apercu
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Headspace Apercu
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: -0.03em
  headline-sm:
    fontFamily: Headspace Apercu
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.03em
  title-lg:
    fontFamily: Headspace Apercu
    fontSize: 29px
    fontWeight: 700
    lineHeight: 1.1
  body-md:
    fontFamily: Headspace Apercu
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  body-lg:
    fontFamily: Headspace Apercu
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.01em
  label-lg:
    fontFamily: Headspace Apercu
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.03em
  label-md:
    fontFamily: Headspace Apercu
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.1
  label-sm:
    fontFamily: Headspace Apercu
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.29
    letterSpacing: -0.01em
  headline-display-mobile:
    fontFamily: Headspace Apercu
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.03em
  headline-md-mobile:
    fontFamily: Headspace Apercu
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: -0.03em
rounded:
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 8px
  margin: 48px
  container: 1360px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 8px 16px 8px 24px
    height: 78px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 14px 20px
    height: 48px
  button-secondary-hover:
    backgroundColor: "#141313"
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 0px 24px
    height: 48px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#000000"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 24px 16px 8px 16px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Headspace Design System

## Overview

Headspace describes itself as: “Live a healthier, happier, more well-rested life in just a few minutes a day. Get the science-backed mental health app for every moment. Try for free.” The interface is light, built on **Warm Snow (#F9F4F2)** with **Graphite (#2D2C2B)** text, and **Vivid Blue (#0061EF)** as the main accent.

Type is set in **Headspace Apercu**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 32px.

Measured from [headspace.com](https://www.headspace.com/) on October 21, 2026 at 1440×900 and 390×844 from 408 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Warm Snow (#F9F4F2):** Page background, seen 15 times. Token `background`.
- **Graphite (#2D2C2B):** Primary text and headings, seen 91 times. Token `on-surface`.
- **Graphite (#44423F):** Secondary text, seen 24 times. Token `on-surface-variant`.
- **Graphite (#4B4C4D):** Muted text and metadata, seen 6 times. Token `on-surface-muted`.
- **Warm Slate (#63605D):** Subtle text and placeholders, seen 3 times. Token `on-surface-subtle`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 17 times. Token `surface-container-low`.
- **Warm Silver (#C6C1B9):** Borders and dividers, seen 7 times. Token `outline`.
- **Warm Silver (#E2DED9):** Secondary dividers, seen 6 times. Token `outline-variant`.
- **Vivid Blue (#0061EF):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Indigo (#1A0C54):** Accent, seen 8 times. Token `secondary`.
- **Light Pink (#FF76B8):** Accent, seen 3 times. Token `tertiary`.
- **Vivid Amber (#FFCE00):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**Headspace Apercu** carries the whole interface. Fallback stack: `Headspace Apercu, sans-serif`.

- **headline-display:** Headspace Apercu 64px at weight 700, line height 1, tracking -0.03em (40px on mobile). Page title (h1).
- **headline-lg:** Headspace Apercu 56px at weight 700, line height 1.1, tracking -0.03em. Section headings (h2).
- **headline-md:** Headspace Apercu 40px at weight 700, line height 1.15, tracking -0.03em (32px on mobile). Sub-section headings.
- **headline-sm:** Headspace Apercu 32px at weight 700, line height 1.2, tracking -0.03em. Card and feature titles.
- **title-lg:** Headspace Apercu 29px at weight 700, line height 1.1. Small titles.
- **body-md:** Headspace Apercu 16px at weight 400, line height 1.15. Body text.
- **body-lg:** Headspace Apercu 20px at weight 400, line height 1.5, tracking -0.01em. Lead paragraphs.
- **label-lg:** Headspace Apercu 18px at weight 700, line height 1.2, tracking -0.03em. Large buttons and tabs.
- **label-md:** Headspace Apercu 16px at weight 700, line height 1.1. Buttons, navigation and labels.
- **label-sm:** Headspace Apercu 14px at weight 500, line height 1.29, tracking -0.01em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (83% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 16px, lg 24px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1360px.
- **Page margin:** 48px on each side of full-width sections.
- **Breakpoints:** 400px, 425px, 426px, 428px, 476px, 550px, 600px, 768px, 769px, 890px, 896px, 897px, 1023px, 1024px, 1280px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(65, 61, 69, 0.2) 0px 2px 0px 0px`
- `rgba(20, 19, 19, 0.2) 0px 3.23px 6.45px 0px`

## Shapes

Most elements use 32px corners. Measured radii, most used first:

- **xl (32px):** 64 elements.
- **lg (24px):** 40 elements.
- **full (9999px):** 32 elements.
- **sm (8px):** 28 elements.
- **md (16px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Stress less”):** #FFFFFF fill, #4B4C4D text, 16px/400, 8px radius, padding 8px 16px 8px 24px, border 2px solid #E2DED9.
- **button-secondary (“Try for $0”):** #2D2C2B fill, #FFFFFF text, 16px/700, 32px radius, padding 14px 20px.
- **button-secondary-hover:** background #141313, text #FFFFFF on hover.
- **button-ghost (“Guided meditations”):** #F9F4F2 fill, #2D2C2B text, 18px/700, 24px radius, padding 0px 24px.
- **input-field (“email”):** #FFFFFF fill, #000000 text, 16px/400, 8px radius, padding 24px 16px 8px 16px, border 1px solid #D2D5DE.
- **link:** transparent fill, #44423F text, padding 0px.

## Do's and Don'ts

- Do use #F9F4F2 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 4 levels: #2D2C2B, #44423F, #4B4C4D, #63605D.
- Do reserve #0061EF for primary actions and key highlights.
- Do set headlines in Headspace Apercu with tight tracking (-0.03em).
- Do reuse the measured spacing steps (6px, 16px, 24px).
- Do use 32px corners on most elements; larger surfaces also use 24px, 8px and 16px.
- Don't introduce new font families beyond Headspace Apercu.
- Don't use #0061EF for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.4s.

- **Easing:** `cubic-bezier(0.32, 0.94, 0.6, 1)`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/headspace.com/), the free DESIGN.md generator.
