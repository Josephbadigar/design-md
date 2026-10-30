---
version: alpha
name: Grammarly
description: "Light interface measured from grammarly.com: matter type with Matter, dark teal accents, tonal surfaces and 6px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1F243C"
  on-background: "#1F243C"
  on-surface-strong: "#000000"
  on-surface-variant: "#0E101A"
  on-surface-muted: "#2E2E2E"
  surface-container-low: "#F5F5F5"
  outline: "#EBEBEB"
  outline-variant: "#C6CBDE"
  primary: "#027E6F"
  on-primary: "#FFFFFF"
  inverse-surface: "#1C1C1C"
  secondary: "#4285F4"
typography:
  display-hero:
    fontFamily: matter
    fontSize: 52px
    fontWeight: 670
    lineHeight: 1.12
    letterSpacing: -0.01em
  headline-display:
    fontFamily: matter
    fontSize: 46px
    fontWeight: 670
    lineHeight: 1.09
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: matter
    fontSize: 36px
    fontWeight: 670
    lineHeight: 1.11
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Matter
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.2
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
  body-lg:
    fontFamily: sans-serif
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.44
  body-sm:
    fontFamily: sans-serif
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: system-ui
    fontSize: 12px
    fontWeight: 400
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 700
  label-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
  headline-display-mobile:
    fontFamily: matter
    fontSize: 30px
    fontWeight: 670
    lineHeight: 1.13
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: matter
    fontSize: 28px
    fontWeight: 670
    lineHeight: 1.14
    letterSpacing: -0.01em
  display-hero-mobile:
    fontFamily: matter
    fontSize: 34px
    fontWeight: 670
    lineHeight: 1.12
    letterSpacing: -0.01em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 50px
  gutter: 8px
  margin: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 0px 8px
    height: 34px
  button-primary-hover:
    backgroundColor: "#014C43"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "#4D536E"
    rounded: "{rounded.md}"
    padding: 8px 16px
    height: 60px
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#545454"
    typography: "{typography.body-sm}"
    padding: 0px
    height: 48px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Grammarly Design System

## Overview

Grammarly describes itself as: “Grammarly makes AI writing convenient. Work smarter with personalized AI guidance and text generation on any app or website.” The interface is light, built on **White (#FFFFFF)** with **Deep Indigo (#1F243C)** text, and **Dark Teal (#027E6F)** as the main accent.

Type is set in **matter** and **Matter**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 6px.

Measured from [grammarly.com](https://www.grammarly.com/) on October 29, 2026 at 1440×900 and 390×844 from 378 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 17 times. Token `background`, CSS `--button-ghost-shortcut-text-active`.
- **Deep Indigo (#1F243C):** Primary text and headings, seen 74 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 10 times. Token `on-surface-strong`.
- **Cool Charcoal (#0E101A):** Secondary text, seen 9 times. Token `on-surface-variant`.
- **Graphite (#2E2E2E):** Muted text and metadata, seen 17 times. Token `on-surface-muted`, CSS `--origin-color-fill-base-inverse`.
- **Snow (#F5F5F5):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--origin-color-spot-illustration-fill-secondary`.
- **Mist (#EBEBEB):** Borders and dividers, seen 5 times. Token `outline`.
- **Light Blue (#C6CBDE):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Dark Teal (#027E6F):** Primary buttons and calls to action, seen 19 times. Token `primary`, CSS `--green-60`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#1C1C1C):** High-contrast fills, seen 1 time. Token `inverse-surface`, CSS `--button-pro-background-active`.
- **Vivid Blue (#4285F4):** Accent, seen 1 time. Token `secondary`.

## Typography

**matter**, **Matter**, **system-ui** and **sans-serif** share the interface. Fallback stack: `matter, sans-serif`. Other loaded fonts: Glyph.

- **display-hero:** matter 52px at weight 670, line height 1.12, tracking -0.01em (34px on mobile). Oversized hero statements.
- **headline-display:** matter 46px at weight 670, line height 1.09, tracking -0.01em (30px on mobile). Page title (h1).
- **headline-lg:** matter 36px at weight 670, line height 1.11, tracking -0.01em (28px on mobile). Section headings (h2).
- **headline-md:** Matter 20px at weight 600, line height 1.2. Sub-section headings.
- **body-md:** system-ui 16px at weight 400. Body text.
- **body-lg:** sans-serif 18px at weight 400, line height 1.44. Lead paragraphs.
- **body-sm:** sans-serif 14px at weight 400, line height 1.5. Secondary and small text.
- **caption:** system-ui 12px at weight 400. Captions and fine print.
- **label-md:** system-ui 16px at weight 700. Buttons, navigation and labels.
- **label-sm:** system-ui 14px at weight 400. Small labels and badges.

## Layout

Spacing follows a 4px grid: 98% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 50px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 48px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F5F5F5) and #EBEBEB borders.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 60 elements.
- **lg (8px):** 48 elements.
- **sm (4px):** 28 elements.
- **full (9999px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign Up It’s free”):** #027E6F fill, #FFFFFF text, 14px/400, 6px radius, padding 0px 8px.
- **button-primary-hover:** background #014C43, text #FFFFFF on hover.
- **button-outline (“Sign up with Google”):** #FFFFFF fill, #4D536E text, 13.3333px/400, 6px radius, padding 8px 16px, border 1px solid #6D758D.
- **button-ghost (“Next”):** #F5F5F5 fill, #545454 text, 14px/400, 50% radius, padding 0px, border 1px solid #545454.
- **card:** #FFFFFF fill, #000000 text, 13.3333px/400, 8px radius, padding 0px, border 1px solid #EBEBEB.
- **link:** transparent fill, #1F243C text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5F5F5.
- Do keep text in 4 levels: #1F243C, #000000, #0E101A, #2E2E2E.
- Do reserve #027E6F for primary actions and key highlights.
- Do set headlines in matter with tight tracking (-0.01em).
- Do keep spacing on the 4px grid.
- Do use 6px corners on most elements; larger surfaces also use 8px and 4px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond matter, Matter, system-ui and sans-serif.
- Don't use #027E6F for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s.

- **Easing:** `ease-out`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/grammarly.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
