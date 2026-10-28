---
version: alpha
name: Plaid
description: "Light interface measured from plaid.com: Plaid Sans type with Cern, deep cyan accents, flat surfaces and 100px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#111111"
  on-background: "#111111"
  on-surface-variant: "#00172E"
  on-surface-muted: "#232424"
  on-surface-subtle: "#5C7695"
  outline: "#A3A3FF"
  primary: "#034049"
  on-primary: "#FFFFFF"
  secondary: "#05565C"
  tertiary: "#CCF8FF"
  warning: "#F2D211"
typography:
  headline-display:
    fontFamily: Plaid Sans
    fontSize: 76px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.045em
  headline-lg:
    fontFamily: Plaid Sans
    fontSize: 70px
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: -0.04em
  headline-md:
    fontFamily: Cern
    fontSize: 36px
    fontWeight: 800
    lineHeight: 1.33
  body-md:
    fontFamily: Cern
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Plaid Sans
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.03em
  body-sm:
    fontFamily: Cern
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Cern
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.33
  label-sm:
    fontFamily: Cern
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Plaid Sans
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.04em
rounded:
  sm: 8px
  md: 24px
  lg: 100px
  full: 9999px
spacing:
  xs: 3px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 57.33px
  gutter: 10px
  section: 164px
  margin: 100px
components:
  button-primary:
    textColor: "#003E4A"
    rounded: 46px
    padding: 13px 32px
    height: 56px
  button-primary-hover:
    textColor: "#0F0F0F"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 12px 24px
    height: 40px
  button-tertiary:
    backgroundColor: "#10D1B7"
    textColor: "#111112"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 12px 24px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 12px 16px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "#4B4B4B"
    rounded: "{rounded.sm}"
    padding: 8px 8px 8px 16px
  link:
    textColor: "{colors.on-primary}"
---

# Plaid Design System

## Overview

Plaid describes itself as: “Plaid helps all companies build fintech solutions by making it easy, safe and reliable for people to connect their financial data to apps and services.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#111111)** text, and **Deep Cyan (#034049)** as the main accent.

Type is set in **Plaid Sans** and **Cern**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 100px.

Measured from [plaid.com](https://plaid.com/) on October 21, 2026 at 1440×900 and 390×844 from 450 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles, plus gradient stops #FFC728, #6748D8, #B14EDB, #86EF5A.

- **White (#FFFFFF):** Page background, seen 7 times. Token `background`, CSS `--t5-button-text-solid-resting`.
- **Charcoal (#111111):** Primary text and headings, seen 11 times. Token `on-surface`, CSS `--color-border-state-filled`.
- **Deep Blue (#00172E):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Charcoal (#232424):** Muted text and metadata, seen 8 times. Token `on-surface-muted`, CSS `--t5-button-icon-ghost-loading`.
- **Blue (#5C7695):** Subtle text and placeholders, seen 5 times. Token `on-surface-subtle`.
- **Light Indigo (#A3A3FF):** Borders and dividers, seen 5 times. Token `outline`.
- **Deep Cyan (#034049):** Brand color on large areas. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Cyan (#05565C):** Secondary buttons, seen 36 times. Token `secondary`.
- **Pale Cyan (#CCF8FF):** Secondary buttons, seen 30 times. Token `tertiary`.
- **Vivid Amber (#F2D211):** Warnings and highlights, seen 3 times. Token `warning`, CSS `--yellow800`.

## Typography

**Plaid Sans** and **Cern** share the interface. Fallback stack: `Plaid Sans, Cern, Avenir Next, Avenir`. Other loaded fonts: Bowery Street, Inconsolata.

- **headline-display:** Plaid Sans 76px at weight 500, line height 1.12, tracking -0.045em (32px on mobile). Page title (h1).
- **headline-lg:** Plaid Sans 70px at weight 500, line height 1.08, tracking -0.04em. Section headings (h2).
- **headline-md:** Cern 36px at weight 800, line height 1.33. Sub-section headings.
- **body-md:** Cern 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Plaid Sans 30px at weight 500, line height 1.2, tracking -0.03em. Lead paragraphs.
- **body-sm:** Cern 13px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Cern 16px at weight 700, line height 1.33. Buttons, navigation and labels.
- **label-sm:** Cern 14px at weight 600, line height 1.43. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 67% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 8px, md 12px, lg 24px, xl 57.33px.
- **Sections:** 164px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Page margin:** 100px on each side of full-width sections.
- **Breakpoints:** 0px, 412px, 431px, 439.95px, 440px, 460px, 639.95px, 640px, 1023.95px, 1024px, 1280px, 1439.95px, 1440px, 1727px, 1730px, 1731px, 1919px, 2560px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.2) 0px 0px 5px 0px`
- `rgba(0, 0, 0, 0.14) 0px 1px 16.5px 0px`
- `rgba(0, 0, 0, 0.15) 0px 1px 5px 0px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0.15) 0px 1px 5px 0px inset`.

## Shapes

Most elements use 100px corners. Measured radii, most used first:

- **lg (100px):** 312 elements.
- **full (9999px):** 40 elements.
- **md (24px):** 28 elements.
- **sm (8px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Talk with our team”):** transparent fill, #003E4A text, 20px/600, 46px radius, padding 13px 32px, shadow `rgba(0, 0, 0, 0.15) 0px 1px 5px 0px inset`.
- **button-primary-hover:** background #00000000, text #0F0F0F on hover.
- **button-secondary (“Manage”):** #05565C fill, #FFFFFF text, 13.008px/600, 1000px radius, padding 12px 24px.
- **button-tertiary (“Ok”):** #10D1B7 fill, #111112 text, 13.008px/600, 1000px radius, padding 12px 24px.
- **button-ghost (“Products”):** transparent fill, #232424 text, 16px/400, 999px radius, padding 12px 16px.
- **input-field:** #FFFFFF fill, #4B4B4B text, 16.5px/400, 8px radius, padding 8px 8px 8px 16px, border 1px solid #02294B.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 4 levels: #111111, #00172E, #232424, #5C7695.
- Do use #034049 as the brand accent: header, logo and key highlights.
- Do set headlines in Plaid Sans with tight tracking (-0.045em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 100px corners on most elements; larger surfaces also use 24px and 8px.
- Don't introduce new font families beyond Plaid Sans and Cern.
- Don't use #034049 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.25s, 0.5s, 0.1s, 0.3s.

- **Easing:** `ease-in-out`, `ease`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/plaid.com/), the free DESIGN.md generator.
