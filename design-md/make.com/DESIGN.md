---
version: alpha
name: Make
description: "Light interface measured from make.com: Satoshi type, violet accents, tonal surfaces and 16px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#342237"
  on-background: "#342237"
  on-surface-strong: "#000000"
  on-surface-variant: "#69586C"
  surface-container-low: "#FAFAFA"
  outline: "#DAD4DA"
  outline-variant: "#E9E6E9"
  primary: "#8F4BD2"
  on-primary: "#FFFFFF"
  secondary: "#E1B9F9"
  tertiary: "#CF8BF5"
typography:
  headline-display:
    fontFamily: Satoshi
    fontSize: 60px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Satoshi
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.22
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Satoshi
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.27
  headline-sm:
    fontFamily: Satoshi
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
  title-lg:
    fontFamily: Satoshi
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
  body-md:
    fontFamily: Satoshi
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Satoshi
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  label-md:
    fontFamily: Satoshi
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Satoshi
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Satoshi
    fontSize: 41.5px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Satoshi
    fontSize: 28.5px
    fontWeight: 500
    lineHeight: 1.22
    letterSpacing: -0.02em
  headline-sm-mobile:
    fontFamily: Satoshi
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.33
rounded:
  sm: 8px
  md: 16px
  lg: 24px
spacing:
  sm: 8px
  md: 10.5px
  lg: 32px
  xl: 64px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 10.5px 18px
    height: 47px
  button-secondary:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 12px 20px
    height: 52px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "#58475A"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 12px 20px
    height: 50px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Make Design System

## Overview

Make describes itself as: “Automate your work. Make allows you to visually build, scale and automate AI and agentic workflows. User friendly no-code integration tool. Try it now for free!” The interface is light, built on **White (#FFFFFF)** with **Deep Purple (#342237)** text, and **Violet (#8F4BD2)** as the main accent.

Type is set in **Satoshi**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 16px.

Measured from [make.com](https://www.make.com/) on October 21, 2026 at 1440×900 and 390×844 from 318 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles, plus gradient stops #8F4BD2.

- **White (#FFFFFF):** Page background, seen 21 times. Token `background`, CSS `--_theme---button-primary--text-hover`.
- **Deep Purple (#342237):** Primary text and headings, seen 30 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 4 times. Token `on-surface-strong`.
- **Purple (#69586C):** Secondary text, seen 26 times. Token `on-surface-variant`.
- **Snow (#FAFAFA):** Raised areas one step from the page, seen 9 times. Token `surface-container-low`.
- **Silver (#DAD4DA):** Borders and dividers, seen 7 times. Token `outline`, CSS `--_theme---feature-card--border-outer`.
- **Mist (#E9E6E9):** Secondary dividers, seen 4 times. Token `outline-variant`, CSS `--_theme---hero-center-frame-inner`.
- **Violet (#8F4BD2):** Primary buttons and calls to action, seen 18 times. Token `primary`, CSS `--_theme---button-primary--border`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Violet (#E1B9F9):** Brand accent (CSS variable), seen 24 times. Token `secondary`.
- **Light Violet (#CF8BF5):** Brand accent (CSS variable), seen 12 times. Token `tertiary`.

## Typography

**Satoshi** carries the whole interface. Fallback stack: `Satoshi, Arial, sans-serif`.

- **headline-display:** Satoshi 60px at weight 500, line height 1.2, tracking -0.02em (41.5px on mobile). Page title (h1).
- **headline-lg:** Satoshi 36px at weight 500, line height 1.22, tracking -0.02em (28.5px on mobile). Section headings (h2).
- **headline-md:** Satoshi 30px at weight 500, line height 1.27. Sub-section headings.
- **headline-sm:** Satoshi 24px at weight 500, line height 1.33 (20px on mobile). Card and feature titles.
- **title-lg:** Satoshi 20px at weight 400, line height 1.5. Small titles.
- **body-md:** Satoshi 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Satoshi 18px at weight 400, line height 1.56. Lead paragraphs.
- **label-md:** Satoshi 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Satoshi 14px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 69% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 8px, md 10.5px, lg 32px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 425px, 426px, 479px, 480px, 500px, 550px, 600px, 767px, 768px, 769px, 896px, 991px, 1919px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(10, 13, 18, 0.05) 0px 1px 2px 0px, rgba(10, 13, 18, 0.05) 0px -2px 0px 0px inset, rgba(10, 13, 18, 0.18) 0px 0px 0px 1px inset, rgba(255, 255, 255, 0.12) 0px 0px 0px 2px inset`
- `rgba(10, 13, 18, 0.05) 0px 1px 2px 0px, rgba(10, 13, 18, 0.05) 0px -2px 0px 0px inset`
- `rgba(0, 0, 0, 0.05) 0px 1px 2px 0px, rgba(0, 0, 0, 0.05) 0px -1px 0px 0px inset`

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **md (16px):** 72 elements.
- **sm (8px):** 64 elements.
- **lg (24px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try it free”):** #8F4BD2 fill, #FFFFFF text, 16px/400, 8px radius, padding 10.5px 18px, border 1px solid #8F4BD2, shadow `rgba(10, 13, 18, 0.05) 0px 1px 2px 0px, rgba(10, 13, 18, 0.05) 0px -2px 0px 0px inset, rgba(10, 13, 18, 0.18) 0px 0px 0px 1px inset, rgba(255, 255, 255, 0.12) 0px 0px 0px 2px inset`.
- **button-secondary (“Understood”):** transparent fill, #FFFFFF text, 16px/500, 8px radius, padding 12px 20px, shadow `rgba(0, 0, 0, 0.05) 0px 1px 2px 0px, rgba(0, 0, 0, 0.05) 0px -2px 0px 0px inset, rgba(0, 0, 0, 0.18) 0px 0px 0px 1px inset`.
- **button-outline (“Select Cookies Settings”):** #FFFFFF fill, #58475A text, 16px/500, 8px radius, padding 12px 20px, border 1px solid #DAD4DA, shadow `rgba(0, 0, 0, 0.05) 0px 1px 2px 0px, rgba(0, 0, 0, 0.05) 0px -1px 0px 0px inset`.
- **button-ghost (“What is Make?”):** transparent fill, #342237 text, 16px/500, padding 0px.
- **link:** transparent fill, #69586C text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAFAFA.
- Do keep text in 3 levels: #342237, #000000, #69586C.
- Do reserve #8F4BD2 for primary actions and key highlights.
- Do set headlines in Satoshi with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 10.5px, 32px).
- Do use 16px corners on most elements; larger surfaces also use 8px and 24px.
- Don't introduce new font families beyond Satoshi.
- Don't use #8F4BD2 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.001s, 0.3s, 0.15s, 0.6s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.33, 1, 0.68, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/make.com/), the free DESIGN.md generator.
