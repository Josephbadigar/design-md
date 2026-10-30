---
version: alpha
name: Basecamp
description: "Light interface measured from basecamp.com: Graphik type, vivid blue accents, tonal surfaces and 2.42px corners."
colors:
  background: "#FFF9F5"
  surface: "#FFF9F5"
  on-surface: "#29353C"
  on-background: "#29353C"
  on-surface-variant: "#6D767B"
  on-surface-muted: "#9A9FA2"
  surface-container-low: "#FCF8F3"
  surface-container: "#FCF9E7"
  surface-container-high: "#FEFBFD"
  overlay: "#117AF31A"
  overlay-strong: "#29353C0D"
  outline: "#29353C1A"
  outline-variant: "#E3E5E5"
  primary: "#117AF3"
  on-primary: "#FFFFFF"
  secondary: "#146DC7"
  tertiary: "#2377D2"
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
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 13.79px 15.32px
    height: 37px
  button-ghost:
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 13.79px 15.32px
  card:
    backgroundColor: "{colors.on-primary}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 9.69px
  link:
    textColor: "{colors.secondary}"
---

# Basecamp Design System

## Overview

Basecamp describes itself as: “Trusted by millions, Basecamp puts everything you need to get work done in one place. It’s the calm, organized way to manage projects, work with clients, and communicate company-wide.” The interface is light, built on **Warm Snow (#FFF9F5)** with **Deep Blue (#29353C)** text, and **Vivid Blue (#117AF3)** as the main accent.

Type is set in **Graphik**. Headlines run large with tight negative tracking; body text is 17px. Depth comes from soft drop shadows. Corners are mostly 2.42px.

Measured from [basecamp.com](https://basecamp.com/) on October 29, 2026 at 1440×900 and 390×844 from 418 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles, plus gradient stops #0067DE, #146DC7, #FFE88B, #F9D45E.

- **Warm Snow (#FFF9F5):** Page background, seen 1 time. Token `background`.
- **Deep Blue (#29353C):** Primary text and headings, seen 80 times. Token `on-surface`, CSS `--color-ink-inverted`.
- **Cool Slate (#6D767B):** Secondary text, seen 14 times. Token `on-surface-variant`.
- **Cool Gray (#9A9FA2):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Warm Snow (#FCF8F3):** Raised areas one step from the page, seen 10 times. Token `surface-container-low`.
- **Pale Amber (#FCF9E7):** Cards and panels, seen 1 time. Token `surface-container`.
- **Snow (#FEFBFD):** Hover and pressed fills, seen 41 times. Token `surface-container-high`.
- **Vivid Blue 10% (#117AF31A):** Translucent fill for cards and controls, seen 37 times. Token `overlay`.
- **Deep Blue 5% (#29353C0D):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Deep Blue 10% (#29353C1A):** Borders and dividers, seen 30 times. Token `outline`.
- **Mist (#E3E5E5):** Secondary dividers, seen 14 times. Token `outline-variant`.
- **Vivid Blue (#117AF3):** Primary buttons and calls to action, seen 9 times. Token `primary`, CSS `--color-blue`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#146DC7):** Links and interactive text, seen 47 times. Token `secondary`.
- **Blue (#2377D2):** Accent in text, fills and borders, seen 10 times. Token `tertiary`.

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
- `rgb(227, 229, 229) 0px 0px 0px 0.605469px inset, rgba(41, 53, 60, 0.1) 0px 0px 1.21094px 0px`
- `oklch(0 0 0 / 0.0625) 0px 0px 0px 1px, oklch(0 0 0 / 0.04) 0px 3.82986px 30.6389px -9.57465px, oklch(0 0 0 / 0.04) 0px 5.74479px 38.2986px -11.4896px, oklch(0 0 0 / 0.04) 0px 5.74479px 15.3194px -13.4045px, oklch(0 0 0 / 0.04) 0px 9.57465px 22.9792px -17.2344px, oklch(0 0 0 / 0.04) 0px 13.4045px 30.6389px -21.0642px`

Hairline rings and inset highlights also appear: `rgba(41, 53, 60, 0.1) 0px 0px 0px 0.605469px inset`.

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
- **button-outline (“Have an account? Sign in”):** #FFF9F5 fill, #29353C text, 15.3194px/500, padding 13.79px 15.32px.
- **button-ghost (“Have an account? Sign in”):** transparent fill, 15.3194px/500, padding 13.79px 15.32px.
- **card:** #FFFFFF fill, #29353C text, 7.26562px/400, 4.84375px radius, padding 9.69px.
- **link:** transparent fill, #146DC7 text, padding 0px.

## Do's and Don'ts

- Do use #FFF9F5 for the page and lift surfaces in small steps: #FCF8F3, #FCF9E7, #FEFBFD.
- Do keep text in 3 levels: #29353C, #6D767B, #9A9FA2.
- Do reserve #117AF3 for primary actions and key highlights.
- Do set headlines in Graphik with tight tracking (-0.026em).
- Do reuse the measured spacing steps (7.57px, 12.06px, 19.15px).
- Do use 2.42px corners on most elements; larger surfaces also use 4.84px, 13px and 1.21px.
- Don't use #6D767B for body text; it reaches 4.44:1 on #FFF9F5. Keep it for large text or metadata.
- Don't use #9A9FA2 for body text; it reaches 2.56:1 on #FFF9F5. Keep it for large text or metadata.
- Don't introduce new font families beyond Graphik.
- Don't use #117AF3 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s.

- **Easing:** `ease`, `cubic-bezier(0.34, 1.2, 0.64, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/basecamp.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
