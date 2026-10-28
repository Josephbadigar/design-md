---
version: alpha
name: Basecamp
description: "Dark interface measured from basecamp.com: Graphik type, vivid blue accents, tonal surfaces and 2.42px corners."
colors:
  background: "#131F25"
  surface: "#131F25"
  on-surface: "#E1E5E8"
  on-background: "#E1E5E8"
  on-surface-variant: "#A8AFB3"
  on-surface-muted: "#828B8F"
  on-surface-subtle: "#475257"
  surface-container-low: "#0B151B"
  surface-container: "#1B2930"
  surface-container-high: "#35332A"
  surface-container-highest: "#23363F"
  overlay: "#117AF31A"
  overlay-strong: "#E1E5E80D"
  outline: "#E1E5E81A"
  outline-variant: "#475257"
  primary: "#117AF3"
  on-primary: "#FFFFFF"
  secondary: "#68A8F4"
  tertiary: "#775F30"
  error: "#EB7550"
typography:
  headline-display:
    fontFamily: Graphik
    fontSize: 42px
    fontWeight: 800
    lineHeight: 1.15
    letterSpacing: -0.026em
  headline-lg:
    fontFamily: Graphik
    fontSize: 30.5px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.014em
  body-md:
    fontFamily: Graphik
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.014em
  body-lg:
    fontFamily: Graphik
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.014em
  body-sm:
    fontFamily: Graphik
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: -0.006em
  caption:
    fontFamily: Graphik
    fontSize: 8.5px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.007em
  label-md:
    fontFamily: Graphik
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.014em
  headline-display-mobile:
    fontFamily: Graphik
    fontSize: 25px
    fontWeight: 800
    lineHeight: 1.15
    letterSpacing: -0.026em
  headline-lg-mobile:
    fontFamily: Graphik
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.014em
rounded:
  sm: 1.21px
  md: 2.42px
  lg: 4.84px
  xl: 13px
  full: 9999px
spacing:
  xs: 3.2px
  sm: 7.57px
  md: 12.06px
  lg: 19.15px
  xl: 45.96px
  gutter: 9.69px
  section: 71.81px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 13.79px 15.32px
    height: 37px
  button-primary-hover:
    backgroundColor: "#0067DE"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 13.79px 15.32px
    height: 37px
  button-outline-hover:
    backgroundColor: "{colors.surface-container}"
  button-secondary:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 19.15px 21.06px 19.15px 49.79px
    height: 45px
  button-ghost:
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 13.79px 15.32px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 9.69px
  link:
    textColor: "{colors.secondary}"
---

# Basecamp Design System

## Overview

Basecamp describes itself as: “Trusted by millions, Basecamp puts everything you need to get work done in one place. It’s the calm, organized way to manage projects, work with clients, and communicate company-wide.” The interface is dark, built on **Deep Blue (#131F25)** with **Cool Mist (#E1E5E8)** text, and **Vivid Blue (#117AF3)** as the main accent.

Type is set in **Graphik**. Headlines run large with tight negative tracking; body text is 17px. Depth comes from soft drop shadows. Corners are mostly 2.42px.

Measured from [basecamp.com](https://basecamp.com/) on October 21, 2026 at 1440×900 and 390×844 from 415 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 18 roles, plus gradient stops #0067DE, #146DC7, #E9CB6E, #E6BB46.

- **Deep Blue (#131F25):** Page background, seen 1 time. Token `background`, CSS `--color-ink-2`.
- **Cool Mist (#E1E5E8):** Primary text and headings, seen 80 times. Token `on-surface`.
- **Cool Gray (#A8AFB3):** Secondary text, seen 14 times. Token `on-surface-variant`.
- **Cool Gray (#828B8F):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Cool Slate (#475257):** Subtle text and placeholders, seen 4 times. Token `on-surface-subtle`.
- **Cool Charcoal (#0B151B):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Deep Blue (#1B2930):** Cards and panels, seen 37 times. Token `surface-container`.
- **Warm Graphite (#35332A):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Deep Cyan (#23363F):** Highest raised elements, seen 10 times. Token `surface-container-highest`.
- **Vivid Blue 10% (#117AF31A):** Translucent fill for cards and controls, seen 37 times. Token `overlay`.
- **Cool Mist 5% (#E1E5E80D):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Cool Mist 10% (#E1E5E81A):** Borders and dividers, seen 30 times. Token `outline`.
- **Cool Slate (#475257):** Secondary dividers, seen 14 times. Token `outline-variant`.
- **Vivid Blue (#117AF3):** Primary buttons and calls to action, seen 9 times. Token `primary`, CSS `--color-blue`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#68A8F4):** Links and interactive text, seen 33 times. Token `secondary`.
- **Dark Orange (#775F30):** Accent, seen 5 times. Token `tertiary`.
- **Red (#EB7550):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**Graphik** carries the whole interface. Fallback stack: `Graphik, sans-serif`.

- **headline-display:** Graphik 42px at weight 800, line height 1.15, tracking -0.026em (25px on mobile). Page title (h1).
- **headline-lg:** Graphik 30.5px at weight 400, line height 1.5, tracking -0.014em (20px on mobile). Section headings (h2).
- **body-md:** Graphik 17px at weight 400, line height 1, tracking -0.014em. Body text.
- **body-lg:** Graphik 19px at weight 400, line height 1.5, tracking -0.014em. Lead paragraphs.
- **body-sm:** Graphik 11px at weight 400, line height 1.33, tracking -0.006em. Secondary and small text.
- **caption:** Graphik 8.5px at weight 400, line height 1.5, tracking -0.007em. Captions and fine print.
- **label-md:** Graphik 15px at weight 500, line height 1, tracking -0.014em. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 0% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.2px, sm 7.57px, md 12.06px, lg 19.15px, xl 45.96px.
- **Sections:** 71.81px vertical padding between major sections.
- **Gaps:** 9.69px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `oklch(0 0 0 / 0.02) 0px 0px 0px 1px, oklch(0 0 0 / 0.1) 0px 6.12778px 61.2778px -36.7667px, oklch(0 0 0 / 0.2) 0px 12.2556px 85.7889px -42.8944px, oklch(0 0 0 / 0.3) 0px 12.2556px 36.7667px -49.0222px, oklch(0 0 0 / 0.4) 0px 24.5111px 49.0222px -67.4055px, oklch(0 0 0 / 0.5) 0px 36.7667px 61.2778px -79.6611px`
- `rgb(71, 82, 87) 0px 0px 0px 0.605469px inset, rgba(225, 229, 232, 0.1) 0px 0px 1.21094px 0px`
- `oklch(0 0 0 / 0.0625) 0px 0px 0px 1px, oklch(0 0 0 / 0.04) 0px 3.82986px 30.6389px -9.57465px, oklch(0 0 0 / 0.04) 0px 5.74479px 38.2986px -11.4896px, oklch(0 0 0 / 0.04) 0px 5.74479px 15.3194px -13.4045px, oklch(0 0 0 / 0.04) 0px 9.57465px 22.9792px -17.2344px, oklch(0 0 0 / 0.04) 0px 13.4045px 30.6389px -21.0642px`

Hairline rings and inset highlights also appear: `rgba(225, 229, 232, 0.1) 0px 0px 0px 0.605469px inset`.

## Shapes

Most elements use 2.42px corners. Measured radii, most used first:

- **md (2.42px):** 88 elements.
- **lg (4.84px):** 72 elements.
- **full (9999px):** 20 elements.
- **xl (13px):** 10 elements.
- **sm (1.21px):** 6 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Want an account? Sign up free”):** #117AF3 fill, #FFFFFF text, 15.3194px/500, padding 13.79px 15.32px.
- **button-primary-hover:** background #0067DE, text #FFFFFF on hover.
- **button-outline (“Have an account? Sign in”):** #131F25 fill, #E1E5E8 text, 15.3194px/500, padding 13.79px 15.32px.
- **button-outline-hover:** background #1B2930, text #E1E5E8 on hover.
- **button-secondary (“Try Basecamp free”):** transparent fill, #FFFFFF text, 19.1493px/500, padding 19.15px 21.06px 19.15px 49.79px, shadow `oklch(0 0 0 / 0.1) 0px 3.82986px 30.6389px -9.57465px, oklch(0 0 0 / 0.1) 0px 5.74479px 38.2986px -11.4896px, oklch(0 0 0 / 0.1) 0px 5.74479px 15.3194px -13.4045px, oklch(0 0 0 / 0.1) 0px 9.57465px 22.9792px -17.2344px, oklch(0 0 0 / 0.1) 0px 13.4045px 30.6389px -21.0642px`.
- **button-ghost (“Have an account? Sign in”):** transparent fill, 15.3194px/500, padding 13.79px 15.32px.
- **card:** #1B2930 fill, #E1E5E8 text, 7.26562px/400, 4.84375px radius, padding 9.69px.
- **link:** transparent fill, #68A8F4 text, padding 0px.

## Do's and Don'ts

- Do use #131F25 for the page and lift surfaces in small steps: #0B151B, #1B2930, #35332A, #23363F.
- Do keep text in 4 levels: #E1E5E8, #A8AFB3, #828B8F, #475257.
- Do reserve #117AF3 for primary actions and key highlights.
- Do set headlines in Graphik with tight tracking (-0.026em).
- Do reuse the measured spacing steps (7.57px, 12.06px, 19.15px).
- Do use 2.42px corners on most elements; larger surfaces also use 4.84px, 13px and 1.21px.
- Don't use #475257 for body text; it reaches 2.1:1 on #131F25. Keep it for large text or metadata.
- Don't introduce new font families beyond Graphik.
- Don't use #117AF3 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s.

- **Easing:** `ease`, `cubic-bezier(0.34, 1.2, 0.64, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/basecamp.com/), the free DESIGN.md generator.
