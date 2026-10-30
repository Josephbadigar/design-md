---
version: alpha
name: Radix UI
description: "Light monochrome interface measured from radix-ui.com: adobeTextPro type with system-ui, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1C2024"
  on-background: "#1C2024"
  on-surface-variant: "#60646C"
  overlay: "#0000330F"
  overlay-strong: "#00002F26"
  primary: "#1C2024"
  on-primary: "#FCFCFD"
  secondary: "#3E63DD"
  tertiary: "#CB1D63"
typography:
  headline-display:
    fontFamily: adobeTextPro
    fontSize: 78px
    fontWeight: 400
    lineHeight: 0.9
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: system-ui
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: -0.006em
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: untitledSans
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.44
    letterSpacing: -0.005em
  body-sm:
    fontFamily: untitledSans
    fontSize: 14px
    fontWeight: 400
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.38
  label-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: adobeTextPro
    fontSize: 38.5px
    fontWeight: 400
    lineHeight: 1.04
    letterSpacing: -0.02em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.lg}"
    padding: 0px 24px
    height: 48px
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.background}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 0px 2px
    height: 24px
  button-ghost:
    textColor: "#002BB7C5"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: 3px
    padding: 0px 0px 0.5px 0px
  link:
    textColor: "{colors.primary}"
---

# Radix UI Design System

## Overview

Radix UI describes itself as: “Components, icons, and colors for building high‑quality, accessible UI. Free and open-source.” The interface is light, built on **White (#FFFFFF)** with **Cool Charcoal (#1C2024)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **adobeTextPro** and **system-ui**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [radix-ui.com](https://www.radix-ui.com/) on October 29, 2026 at 1440×900 and 390×844 from 309 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles, plus gradient stops #3E63DD.

- **White (#FFFFFF):** Page background, seen 9 times. Token `background`, CSS `--blue-contrast`.
- **Cool Charcoal (#1C2024):** Primary text and headings, seen 56 times. Token `on-surface`.
- **Cool Slate (#60646C):** Secondary text, seen 19 times. Token `on-surface-variant`.
- **Deep Indigo 6% (#0000330F):** Translucent fill for cards and controls, seen 10 times. Token `overlay`, CSS `--slate-a3`.
- **Deep Indigo 15% (#00002F26):** Stronger translucent fill, seen 7 times. Token `overlay-strong`.
- **Cool Charcoal (#1C2024):** Primary buttons and calls to action, seen 71 times. Token `primary`.
- **Snow (#FCFCFD):** Text and icons on primary. Token `on-primary`.
- **Blue (#3E63DD):** Accent in text, fills and borders, seen 8 times. Token `secondary`.
- **Pink (#CB1D63):** Accent in text, fills and borders, seen 6 times. Token `tertiary`.

## Typography

**adobeTextPro**, **system-ui** and **untitledSans** share the interface. Fallback stack: `adobeTextPro, adobeTextPro Fallback, serif`. Other loaded fonts: soehneMono.

- **headline-display:** adobeTextPro 78px at weight 400, line height 0.9, tracking -0.05em (38.5px on mobile). Page title (h1).
- **headline-lg:** system-ui 24px at weight 700, line height 1.25, tracking -0.006em. Section headings (h2).
- **body-md:** system-ui 16px at weight 400, line height 1.5. Body text.
- **body-lg:** untitledSans 18px at weight 500, line height 1.44, tracking -0.005em. Lead paragraphs.
- **body-sm:** untitledSans 14px at weight 400. Secondary and small text.
- **label-md:** system-ui 16px at weight 700, line height 1.38. Buttons, navigation and labels.
- **label-sm:** system-ui 14px at weight 400, line height 1.43. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 67% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 350px, 365px, 369px, 370px, 440px, 519px, 520px, 767px, 768px, 900px, 1024px, 1200px, 1280px, 1440px, 1640px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.05) 0px 2px 4px -1px, rgba(0, 0, 0, 0.05) 0px 0px 0px 1px, rgba(0, 68, 255, 0.118) 0px 0px 0px 1px, rgba(0, 0, 0, 0.1) -1px 0px 1px 0px`
- `rgba(0, 0, 0, 0.1) 0px 0px 1px 1px, rgba(0, 0, 0, 0.05) 0px 1px 1px 0px, rgba(0, 0, 0, 0.05) 0px 2px 4px -1px`

Hairline rings and inset highlights also appear: `rgba(0, 52, 220, 0.447) 0px 0px 0px 1px inset`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (4px):** 128 elements.
- **full (9999px):** 56 elements.
- **md (6px):** 28 elements.
- **lg (8px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #1C2024 fill, #FCFCFD text, 18px/500, 8px radius, padding 0px 24px.
- **button-secondary (“Themes”):** #1C2024 fill, #FFFFFF text, 14px/400, 999px radius, padding 0px 2px.
- **button-ghost (“Downgrade”):** transparent fill, #002BB7C5 text, 14px/500, 4px radius, padding 0px 12px, shadow `rgba(0, 52, 220, 0.447) 0px 0px 0px 1px inset`.
- **input-field (“Email address”):** transparent fill, #1C2024 text, 14px/400, 3px radius, padding 0px 0px 0.5px 0px.
- **link:** transparent fill, #1C2024 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #1C2024, #60646C.
- Do let contrast carry emphasis; primary actions use #1C2024 on #FFFFFF.
- Do set headlines in adobeTextPro with tight tracking (-0.05em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't introduce new font families beyond adobeTextPro, system-ui and untitledSans.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.14s.

## Motion

Interface transitions are quick: 0.14s.

- **Easing:** `cubic-bezier(0.45, 0.05, 0.55, 0.95)`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/radix-ui.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
