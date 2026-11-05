---
version: alpha
name: React Native
description: "Light interface measured from reactnative.dev: Optimistic Display type, dark cyan accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1C1E21"
  on-background: "#1C1E21"
  on-surface-variant: "#404756"
  outline: "#DFE1E6"
  outline-variant: "#BCC1CD"
  primary: "#087EA4"
  on-primary: "#FFFFFF"
  inverse-surface: "#111317EE"
  secondary: "#357DA1"
  tertiary: "#72A1ED"
typography:
  display-hero:
    fontFamily: Optimistic Display
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.25
  headline-display:
    fontFamily: Optimistic Display
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.25
  body-md:
    fontFamily: Optimistic Display
    fontSize: 17px
    fontWeight: 300
    lineHeight: 1.65
  body-lg:
    fontFamily: Optimistic Display
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Optimistic Display
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.44
  display-hero-mobile:
    fontFamily: Optimistic Display
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.25
rounded:
  sm: 12px
  md: 32px
  full: 9999px
spacing:
  xs: 3px
  sm: 8px
  md: 16px
  lg: 17px
  xl: 34px
  gutter: 17px
  margin: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 10px 24px
    height: 50px
  button-primary-hover:
    backgroundColor: "#4E98B6"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "#969FAF"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 8px 0px 12px
    height: 36px
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 10px 24px
    height: 50px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px
  link:
    textColor: "{colors.secondary}"
---

# React Native Design System

## Overview

React Native describes itself as: “A framework for building native apps for Android, iOS, and more using React” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1C1E21)** text, and **Dark Cyan (#087EA4)** as the main accent.

Type is set in **Optimistic Display**. Headlines run large; body text is 17px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [reactnative.dev](https://reactnative.dev/) on November 4, 2026 at 1440×900 and 390×844 from 265 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 13 times. Token `background`, CSS `--ifm-background-surface-color`.
- **Charcoal (#1C1E21):** Primary text and headings, seen 20 times. Token `on-surface`, CSS `--ifm-blockquote-color`.
- **Dark Blue (#404756):** Secondary text, seen 14 times. Token `on-surface-variant`, CSS `--home-button-secondary-text`.
- **Cool Mist (#DFE1E6):** Borders and dividers, seen 10 times. Token `outline`.
- **Cool Silver (#BCC1CD):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Dark Cyan (#087EA4):** Primary buttons and calls to action, seen 2 times. Token `primary`, CSS `--logo`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Cool Charcoal 93% (#111317EE):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Blue (#357DA1):** Links and interactive text, seen 6 times. Token `secondary`, CSS `--ifm-link-hover-color`.
- **Blue (#72A1ED):** Accent (CSS variable). Token `tertiary`.

## Typography

**Optimistic Display** carries the whole interface. Fallback stack: `Optimistic Display, system-ui, -apple-system, sans-serif`.

- **display-hero:** Optimistic Display 48px at weight 700, line height 1.25 (40px on mobile). Oversized hero statements.
- **headline-display:** Optimistic Display 40px at weight 700, line height 1.25. Page title (h1).
- **body-md:** Optimistic Display 17px at weight 300, line height 1.65. Body text.
- **body-lg:** Optimistic Display 20px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** Optimistic Display 14px at weight 400, line height 1.44. Secondary and small text.

## Layout

Spacing does not follow a strict grid: 46% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 8px, md 16px, lg 17px, xl 34px.
- **Gaps:** 17px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.03) 0px 4px 8px 0px`
- `rgba(0, 0, 0, 0.1) 0px 1px 2px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (12px):** 28 elements.
- **md (32px):** 28 elements.
- **full (9999px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #087EA4 fill, #FFFFFF text, 17px/700, 1683px radius, padding 10px 24px.
- **button-primary-hover:** background #4E98B6, text #FFFFFF on hover.
- **button-outline (“Search Ctrl K”):** #FFFFFF fill, #969FAF text, 17px/400, 32px radius, padding 0px 8px 0px 12px, border 1px solid #373940.
- **button-ghost (“Learn the Basics”):** #FFFFFF fill, #404756 text, 17px/700, 1683px radius, padding 10px 24px, border 1px solid #BCC1CD.
- **card:** #FFFFFF fill, #1C1E21 text, 17px/300, 12px radius, padding 0px, border 1px solid #DFE1E6, shadow `rgba(0, 0, 0, 0.03) 0px 4px 8px 0px`.
- **link:** transparent fill, #357DA1 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #1C1E21, #404756.
- Do reserve #087EA4 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 17px).
- Do make buttons and chips fully rounded (9999px); most other elements use 12px corners.
- Don't introduce new font families beyond Optimistic Display.
- Don't use #087EA4 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s.

- **Easing:** `ease`, `cubic-bezier(0.08, 0.52, 0.52, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/reactnative.dev/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
