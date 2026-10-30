---
version: alpha
name: LottieFiles
description: "Light interface measured from lottiefiles.com: DM Sans LF type with Inter LF, dark teal accents, tonal surfaces and 16px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#09090B"
  on-background: "#09090B"
  on-surface-variant: "#71717B"
  surface-container-low: "#FAFAFA"
  surface-container: "#FFF8E5"
  surface-container-high: "#F4F4F5"
  surface-container-highest: "#E9E9E9"
  outline: "#E4E4E7"
  outline-variant: "#FFFFFF33"
  primary: "#019D91"
  on-primary: "#FAFAFA"
  inverse-surface: "#000000"
typography:
  headline-display:
    fontFamily: DM Sans LF
    fontSize: 96px
    fontWeight: 500
    lineHeight: 1.04
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: DM Sans LF
    fontSize: 64px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.04em
  headline-md:
    fontFamily: DM Sans LF
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.04em
  headline-sm:
    fontFamily: DM Sans LF
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.01em
  body-md:
    fontFamily: DM Sans LF
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: DM Sans LF
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.01em
  body-sm:
    fontFamily: DM Sans LF
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: Inter LF
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: DM Sans LF
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.04em
  headline-lg-mobile:
    fontFamily: DM Sans LF
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.03em
rounded:
  sm: 6px
  md: 12px
  lg: 16px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 64px
  gutter: 16px
  section: 224px
  margin: 32px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
    height: 36px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 16px
    height: 82px
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 6px 12px 6px 32px
    height: 36px
  link:
    textColor: "#9F9FA9"
---

# LottieFiles Design System

## Overview

LottieFiles describes itself as: “Effortlessly bring the smallest, free, ready-to-use motion graphics for the web, app, social, and designs. Create, edit, test, collaborate, and ship Lottie animations in no time!” The interface is light, built on **White (#FFFFFF)** with **Near Black (#09090B)** text, and **Dark Teal (#019D91)** as the main accent.

Type is set in **DM Sans LF** and **Inter LF**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 16px.

Measured from [lottiefiles.com](https://lottiefiles.com/) on October 29, 2026 at 1440×900 and 390×844 from 403 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 17 times. Token `background`, CSS `--cc-toggle-on-knob-bg`.
- **Near Black (#09090B):** Primary text and headings, seen 116 times. Token `on-surface`.
- **Cool Slate (#71717B):** Secondary text, seen 13 times. Token `on-surface-variant`.
- **Snow (#FAFAFA):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **Pale Amber (#FFF8E5):** Cards and panels, seen 3 times. Token `surface-container`.
- **Snow (#F4F4F5):** Hover and pressed fills, seen 37 times. Token `surface-container-high`.
- **Mist (#E9E9E9):** Highest raised elements, seen 3 times. Token `surface-container-highest`.
- **Mist (#E4E4E7):** Borders and dividers, seen 2 times. Token `outline`.
- **White 20% (#FFFFFF33):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Dark Teal (#019D91):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **Snow (#FAFAFA):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000000):** High-contrast fills, seen 12 times. Token `inverse-surface`, CSS `--cc-btn-primary-hover-border-color`.

## Typography

**DM Sans LF** and **Inter LF** share the interface. Fallback stack: `DM Sans LF, DM Sans, sans-serif`.

- **headline-display:** DM Sans LF 96px at weight 500, line height 1.04, tracking -0.05em (48px on mobile). Page title (h1).
- **headline-lg:** DM Sans LF 64px at weight 500, line height 1.15, tracking -0.04em (32px on mobile). Section headings (h2).
- **headline-md:** DM Sans LF 48px at weight 500, line height 1.15, tracking -0.04em. Sub-section headings.
- **headline-sm:** DM Sans LF 24px at weight 500, line height 1.12, tracking -0.01em. Card and feature titles.
- **body-md:** DM Sans LF 16px at weight 400, line height 1.5. Body text.
- **body-lg:** DM Sans LF 20px at weight 400, line height 1.4, tracking -0.01em. Lead paragraphs.
- **body-sm:** DM Sans LF 14px at weight 400, line height 1.43. Secondary and small text.
- **label-md:** Inter LF 16px at weight 400, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 64px.
- **Sections:** 224px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 640px, 1024px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **lg (16px):** 328 elements.
- **sm (6px):** 36 elements.
- **md (12px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #019D91 fill, #FAFAFA text, 14px/500, 6px radius, padding 8px 16px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`.
- **button-outline (“Tiny file format but mighty”):** #FAFAFA fill, #09090B text, 16px/400, 16px radius, padding 16px.
- **button-ghost (“Search animations”):** #FAFAFA fill, #71717B text, 14px/400, 6px radius, padding 6px 12px 6px 32px.
- **link:** transparent fill, #9F9FA9 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAFAFA, #FFF8E5, #F4F4F5, #E9E9E9.
- Do keep text in 2 levels: #09090B, #71717B.
- Do reserve #019D91 for primary actions and key highlights.
- Do set headlines in DM Sans LF with tight tracking (-0.05em).
- Do keep spacing on the 4px grid.
- Do use 16px corners on most elements; larger surfaces also use 6px and 12px.
- Don't introduce new font families beyond DM Sans LF and Inter LF.
- Don't use #019D91 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/lottiefiles.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
