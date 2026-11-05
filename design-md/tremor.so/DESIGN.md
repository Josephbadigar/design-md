---
version: alpha
name: Tremor
description: "Light interface measured from tremor.so: GeistSans type, vivid blue accents, tonal surfaces and 6px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#101828"
  on-background: "#101828"
  on-surface-variant: "#364153"
  on-surface-muted: "#4A5565"
  on-surface-subtle: "#6A7282"
  surface-container-low: "#FFFFFFE6"
  surface-container: "#EFF6FF"
  surface-container-high: "#F3F4F6"
  surface-container-highest: "#E5E7EB"
  outline: "#D1D5DC"
  outline-variant: "#E5E7EB"
  primary: "#2B7FFF"
  on-primary: "#FFFFFF"
  inverse-surface: "#000000"
  secondary: "#E12AFB"
  tertiary: "#1C398E"
typography:
  headline-display:
    fontFamily: GeistSans
    fontSize: 60px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: GeistSans
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.11
  headline-md:
    fontFamily: GeistSans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.4
  body-md:
    fontFamily: GeistSans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: GeistSans
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.56
  body-sm:
    fontFamily: GeistSans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: GeistSans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: GeistSans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: GeistSans
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.11
    letterSpacing: -0.035em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
  xl: 12px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 32px
  section: 64px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px
    height: 40px
  button-secondary:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 10px 20px
    height: 44px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 4px 12px
    height: 28px
  button-ghost:
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 0px 12px 8px 12px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Tremor Design System

## Overview

Tremor describes itself as: “Open-source, accessible React UI components styled with Tailwind CSS to build charts and dashboards.” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#101828)** text, and **Vivid Blue (#2B7FFF)** as the main accent.

Type is set in **GeistSans**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 6px.

Measured from [tremor.so](https://www.tremor.so/) on November 4, 2026 at 1440×900 and 390×844 from 341 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #101828, #364153, #2B7FFF, #155DFC.

- **White (#FFFFFF):** Page background, seen 24 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Deep Blue (#101828):** Primary text and headings, seen 62 times. Token `on-surface`.
- **Dark Blue (#364153):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Dark Blue (#4A5565):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **Blue (#6A7282):** Subtle text and placeholders, seen 21 times. Token `on-surface-subtle`.
- **White 90% (#FFFFFFE6):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Cool Snow (#EFF6FF):** Cards and panels, seen 3 times. Token `surface-container`.
- **Snow (#F3F4F6):** Hover and pressed fills, seen 2 times. Token `surface-container-high`.
- **Cool Mist (#E5E7EB):** Highest raised elements, seen 2 times. Token `surface-container-highest`.
- **Cool Silver (#D1D5DC):** Borders and dividers, seen 10 times. Token `outline`.
- **Cool Mist (#E5E7EB):** Secondary dividers, seen 4 times. Token `outline-variant`.
- **Vivid Blue (#2B7FFF):** Primary buttons and calls to action, seen 18 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000000):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Vivid Purple (#E12AFB):** Accent on large areas, seen 3 times. Token `secondary`.
- **Dark Blue (#1C398E):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.

## Typography

**GeistSans** carries the whole interface. Fallback stack: `__GeistSans_fb8f2c, __GeistSans_Fallback_fb8f2c`. Other loaded fonts: __GeistSans_fb8f2c.

- **headline-display:** GeistSans 60px at weight 700, line height 1, tracking -0.035em (36px on mobile). Page title (h1).
- **headline-lg:** GeistSans 36px at weight 700, line height 1.11. Section headings (h2).
- **headline-md:** GeistSans 20px at weight 600, line height 1.4. Sub-section headings.
- **body-md:** GeistSans 16px at weight 400, line height 1.5. Body text.
- **body-lg:** GeistSans 18px at weight 600, line height 1.56. Lead paragraphs.
- **body-sm:** GeistSans 12px at weight 400, line height 1.33. Secondary and small text.
- **label-md:** GeistSans 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** GeistSans 14px at weight 400, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (89% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 40px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 32px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0 0 0 / 0.05) 0px 0px 0px 1px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0.03) 0px 0px 0px 1px, rgba(0, 0, 0, 0.05) 0px 2px 4px 0px, rgba(0, 0, 0, 0.05) 0px 12px 24px 0px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.623 -0.0378409 -0.210628 / 0.3) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 64 elements.
- **sm (4px):** 56 elements.
- **lg (8px):** 52 elements.
- **xl (12px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Hover me”):** #2B7FFF fill, #FFFFFF text, 16px/400, 8px radius, padding 0px.
- **button-secondary (“Get started”):** transparent fill, #FFFFFF text, 16px/500, 6px radius, padding 10px 20px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`.
- **button-outline (“Overview”):** #FFFFFF fill, #101828 text, 14px/500, 4px radius, padding 4px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`.
- **button-ghost (“Europe”):** transparent fill, 14px/500, padding 0px 12px 8px 12px.
- **link:** transparent fill, #4A5565 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FFFFFFE6, #EFF6FF, #F3F4F6, #E5E7EB.
- Do keep text in 4 levels: #101828, #364153, #4A5565, #6A7282.
- Do reserve #2B7FFF for primary actions and key highlights.
- Do set headlines in GeistSans with tight tracking (-0.035em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 6px corners on most elements; larger surfaces also use 4px, 8px and 12px.
- Don't introduce new font families beyond GeistSans.
- Don't use #2B7FFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s, 0.1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/tremor.so/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
